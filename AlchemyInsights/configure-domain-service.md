---
title: Domēna pakalpojuma konfigurēšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7931"
- "9004400"
ms.openlocfilehash: 51e0bd78240627876721cbce654188afac1ee365
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885682"
---
# <a name="unable-to-enable-aad-ds-or-deployment-is-failing"></a><span data-ttu-id="5cb88-102">Nevar iespējot AAD-DS vai izvietošanas kļūmi</span><span class="sxs-lookup"><span data-stu-id="5cb88-102">Unable to enable AAD-DS or deployment is failing</span></span>

<span data-ttu-id="5cb88-103">Lai atrisinātu Azure AD Domain Service (AAD-DS) problēmu, kas nav iespējota vai netiek izvietota, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="5cb88-103">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="5cb88-104">Ja izmantojat jau esošu virtuālo tīklu, atzīmējiet savu NSG, lai iegūtu kārtulas, kas bloķē portus, kas nepieciešami, lai sinhronizētu ar AAD-DS portālā https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="5cb88-104">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="5cb88-105">Pārbaudiet, vai jūsu kļūdas ziņojums ir atbildēts šajā rakstā pieejamā problēmu novēršanas rokasgrāmatā  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="5cb88-105">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="5cb88-106">Izmēģiniet Azure AD Domain pakalpojumu izvietošanu jaunā virtuālajā tīklā.</span><span class="sxs-lookup"><span data-stu-id="5cb88-106">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="5cb88-107">Izpildiet darba sākšanas rokasgrāmatu par to, kā izvietot AAD-DS: [izveidot un konfigurēt AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="5cb88-107">Follow the Getting Started guide on how to deploy AAD-DS: [Create and Configure AAD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="5cb88-108">Ja rodas problēmas saistībā ar Azure AD domēna pakalpojumu izvietošanu, skatiet rakstu [AZURE ad Domain Services problēmu novēršana](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , lai atrisinātu Biežākās kļūdas, kas palīdzēs paveikt darbu atkārtoti.</span><span class="sxs-lookup"><span data-stu-id="5cb88-108">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="5cb88-109">**Nevar atspējot AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="5cb88-109">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="5cb88-110">AAD-DS nevar pauzēt.</span><span class="sxs-lookup"><span data-stu-id="5cb88-110">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="5cb88-111">Ja vēlaties pārtraukt pārvaldītā domēna izmantošanu, tas ir jādzēš.</span><span class="sxs-lookup"><span data-stu-id="5cb88-111">If you wish to stop using your managed domain, it must be deleted.</span></span>
<span data-ttu-id="5cb88-112">Lai dzēstu pārvaldīto domēnu, skatiet rakstu [AAD Domain Service DELETE](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span><span class="sxs-lookup"><span data-stu-id="5cb88-112">To delete your Managed domain, see [Delete AAD Domain Service](https://docs.microsoft.com/azure/active-directory-domain-services/delete-aadds).</span></span>



