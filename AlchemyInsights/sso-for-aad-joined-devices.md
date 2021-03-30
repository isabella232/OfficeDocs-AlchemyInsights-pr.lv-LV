---
title: Single-Sign azure Active Directory ierīcēs, kurās ir savienojums
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9891"
ms.openlocfilehash: f6426a3fb4addc24c5041196fe837134bf0d296b
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405049"
---
# <a name="single-sign-on-for-azure-active-directory-joined-devices"></a><span data-ttu-id="6b6bc-102">Vienotā pierakstīšanās Azure Active Directory ierīcēs, kas ir apvienotas ar jums</span><span class="sxs-lookup"><span data-stu-id="6b6bc-102">Single-sign on for Azure Active Directory Joined Devices</span></span>

<span data-ttu-id="6b6bc-103">Ja jums ir lokāla Active Directory (AD) vide un vēlaties savienot savus AD domēnu datorus ar Azure AD, varat to paveikt, veicot hibrīdu Azure AD savienojumu.</span><span class="sxs-lookup"><span data-stu-id="6b6bc-103">If you have an on-premises Active Directory (AD) environment and you want to join your AD domain-joined computers to Azure AD, you can accomplish this by doing hybrid Azure AD join.</span></span> <span data-ttu-id="6b6bc-104">[Kā: Plānojiet hibrīdo Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) savienojuma ieviešanu, kas nodrošina saistītās darbības, lai ieviestu hibrīdu Azure AD savienojumu jūsu vidē.</span><span class="sxs-lookup"><span data-stu-id="6b6bc-104">[How To: Plan your hybrid Azure Active Directory join implementation](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) provides you with the related steps to implement a hybrid Azure AD join in your environment.</span></span>

[<span data-ttu-id="6b6bc-105">Azure AD pievienoto ierīču konfigurēšana lokālajās ierīcēs un Single-Sign izmantojot Windows Hello darbam</span><span class="sxs-lookup"><span data-stu-id="6b6bc-105">Configure Azure AD joined devices for On-premises Single-Sign On using Windows Hello for Business</span></span>](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan) 

<span data-ttu-id="6b6bc-106">**Primārās atsvaidzināšanas pilnvaras (PRIMARY Refresh Token – PRT) problēmas** Primārā atsvaidzināšanas pilnvara (Primary Refresh Token — PRT) ir Azure AD autentifikācijas galvenā artefaktu sistēmā Windows 10, Windows Server 2016 un jaunākās versijās, iOS un Android ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="6b6bc-106">**Primary Refresh Token (PRT) issues** A Primary Refresh Token (PRT) is a key artifact of Azure AD authentication on Windows 10, Windows Server 2016 and later versions, iOS, and Android devices.</span></span> <span data-ttu-id="6b6bc-107">Tas ir JSON tīmekļa marķieris (JSON Web Token — JWT), kas ir īpaši izsniegts Microsoft pirmās puses marķieru vekseļi, lai iespējotu vienoto pierakstīšanu (single sign-on — SSO) visās lietojumprogrammās, kas tiek izmantotas šajās ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="6b6bc-107">It is a JSON Web Token (JWT) specially issued to Microsoft first party token brokers to enable single sign-on (SSO) across the applications used on those devices.</span></span> <span data-ttu-id="6b6bc-108">[Sadaļā Kas ir primārās atsvaidzināšanas pilnvara?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token)mēs sniedzsim detalizētu informāciju par PRT izrakstīšanu, lietošanu un aizsardzību Windows 10 ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="6b6bc-108">[In What is a Primary Refresh Token?](https://docs.microsoft.com/azure/active-directory/devices/concept-primary-refresh-token), we will provide details on how a PRT is issued, used, and protected on Windows 10 devices.</span></span>

<span data-ttu-id="6b6bc-109">**WamDefaultSet: YES un AzureADPrt: YES** Šie lauki norāda, vai lietotājs ir sekmīgi autentificējis Azure AD, pierakstoties ierīcē.</span><span class="sxs-lookup"><span data-stu-id="6b6bc-109">**WamDefaultSet: YES and AzureADPrt: YES** These fields indicate whether the user has successfully authenticated to Azure AD when signing in to the device.</span></span> <span data-ttu-id="6b6bc-110">Ja vērtības ir **NO**, tam varētu būt iemesls:</span><span class="sxs-lookup"><span data-stu-id="6b6bc-110">If the values are **NO**, it could be due:</span></span>

- <span data-ttu-id="6b6bc-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span><span class="sxs-lookup"><span data-stu-id="6b6bc-111">Bad storage key in the TPM associated with the device upon registration (check the KeySignTest while running elevated).</span></span>
- <span data-ttu-id="6b6bc-112">Alternatīvais pieteikšanās ID</span><span class="sxs-lookup"><span data-stu-id="6b6bc-112">Alternate Login ID</span></span>
- <span data-ttu-id="6b6bc-113">HTTP starpniekserveris nav atrasts</span><span class="sxs-lookup"><span data-stu-id="6b6bc-113">HTTP Proxy not found</span></span>

<span data-ttu-id="6b6bc-114">Problēmu novēršana ierīcēs, izmantojot komandu dsregcmd — [SSO stāvoklis](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span><span class="sxs-lookup"><span data-stu-id="6b6bc-114">Troubleshoot devices using the dsregcmd command - [SSO state](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-device-dsregcmd#sso-state)</span></span>
