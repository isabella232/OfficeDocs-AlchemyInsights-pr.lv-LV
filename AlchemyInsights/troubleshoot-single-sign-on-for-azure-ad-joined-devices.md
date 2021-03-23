---
title: Vienas pierakstīšanās pakalpojumam Azure AD savienotajām ierīcēm problēmu novēršana
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003246"
- "9327"
ms.openlocfilehash: d11c24719eb2db9e9fd87c158c80cec5cb75b946
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036173"
---
# <a name="troubleshoot-single-sign-on-for-azure-ad-joined-devices"></a><span data-ttu-id="42187-102">Vienas pierakstīšanās pakalpojumam Azure AD savienotajām ierīcēm problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="42187-102">Troubleshoot Single-sign on for Azure AD Joined Devices</span></span>

<span data-ttu-id="42187-103">Ja jums ir lokālā Active Directory (AD) vide un vēlaties pievienoties savam AD Domain-Joined datoriem Azure AD, varat to paveikt, veicot hibrīda Azure AD savienojumu.</span><span class="sxs-lookup"><span data-stu-id="42187-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="42187-104">[Kā: plānojiet Hibrīdā Azure Active Directory pievienošanas implementācijā](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) ir aprakstītas darbības, kas jāveic, lai nodrošinātu Hibrīdā Azure AD savienojumu savā vidē.</span><span class="sxs-lookup"><span data-stu-id="42187-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

<span data-ttu-id="42187-105">Papildinformāciju skatiet rakstā [AZURE ad savienoto ierīču konfigurēšana lokālajā Single-Sign, izmantojot Windows Hello darbam](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span><span class="sxs-lookup"><span data-stu-id="42187-105">For more information, see [Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business](https://docs.microsoft.com/windows/security/identity-protection/hello-for-business/hello-hybrid-aadj-sso-base).</span></span>

<span data-ttu-id="42187-106">**Primārās atsvaidzināšanas marķierierīces (PRT) problēmas**</span><span class="sxs-lookup"><span data-stu-id="42187-106">**Primary Refresh Token (PRT) issues**</span></span>

<span data-ttu-id="42187-107">Primārā atsvaidzināšanas pilnvara (PRT) ir Azure AD autentifikācijas galvenais artefakts operētājsistēmā Windows 10, Windows Server 2016 un jaunākās versijās, iOS un Android ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="42187-107">A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="42187-108">Tā ir JSON tīmekļa pilnvara (JWT), kas īpaši izsniegta Microsoft pirmās puses žetonu brokeriem, lai iespējotu vienotās pierakstīšanās (SSO) visās šajās ierīcēs lietotajās lietojumprogrammās.</span><span class="sxs-lookup"><span data-stu-id="42187-108">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="42187-109">Detalizētu informāciju par to, kā PRT tiek izsniegta, lietota un aizsargāta Windows 10 ierīcēs, skatiet rakstā [kas ir primārā atsvaidzināšanas pilnvara?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span><span class="sxs-lookup"><span data-stu-id="42187-109">For details on how a PRT is issued, used, and protected on Windows 10 devices, see [What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token).</span></span>

<span data-ttu-id="42187-110">**WamDefaultSet: Jā un AzureADPrt: Jā**</span><span class="sxs-lookup"><span data-stu-id="42187-110">**WamDefaultSet: YES and AzureADPrt: YES**</span></span>

<span data-ttu-id="42187-111">Šie lauki norāda, vai lietotājs, pierakstoties ierīcē, ir sekmīgi autentificējis Azure AD.</span><span class="sxs-lookup"><span data-stu-id="42187-111">These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="42187-112">Ja **vērtības ir tādas, tās iemesls** var būt:</span><span class="sxs-lookup"><span data-stu-id="42187-112">If the values are **NO**, it could be due to:</span></span>

- <span data-ttu-id="42187-113">Nederīga krātuves atslēga TPM, kas ir saistīts ar ierīci reģistrācijas laikā (pārbaudiet KeySignTest, kamēr darbojas paaugstināts)</span><span class="sxs-lookup"><span data-stu-id="42187-113">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated)</span></span>
- <span data-ttu-id="42187-114">Alternatīvā pieteikšanās ID</span><span class="sxs-lookup"><span data-stu-id="42187-114">Alternate Login ID</span></span>
- <span data-ttu-id="42187-115">HTTP starpniekserveris nav atrasts</span><span class="sxs-lookup"><span data-stu-id="42187-115">HTTP Proxy not found</span></span>

<span data-ttu-id="42187-116">Lai novērstu ierīces, kas izmanto komandu dsregcmd, skatiet sadaļu [SSO statuss](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span><span class="sxs-lookup"><span data-stu-id="42187-116">To troubleshoot devices using the dsregcmd command, see [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state).</span></span>
