---
title: Sinhronizēto lietotāju pārvaldīšana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 5a383bdd17c5fa055c35a923ca36e0e0f6d429e4
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35380512"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a><span data-ttu-id="c8981-102">Nevar iestatīt primāro e-pasta adresi vai mainīt lietotāja atribūtus</span><span class="sxs-lookup"><span data-stu-id="c8981-102">Unable to set primary email address or change user attributes</span></span>

<span data-ttu-id="c8981-103">Par savu vidi, aktivizējot direktoriju sinhronizācijas dažus lietotāju vai objekta atribūtus nevar mainīt, izmantojot administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="c8981-103">If directory synchronization is enabled for your environment some user or object attributes cannot be changed using the Admin Center.</span></span>
<span data-ttu-id="c8981-104">Pilnībā vadīt sinhronizēto lietotāju un to atribūtus, izmantojiet jūsu vietējā aktīvā direktorija lietotāji un grupas pārvaldības konsoli (adsiedit.msc).</span><span class="sxs-lookup"><span data-stu-id="c8981-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="c8981-105">Var arī mainīt atsevišķus lietotājus vai sinhronizēto lietotāju, izmantojot powershell, piemēram, norādīts piemēros kopīgas īpašības:</span><span class="sxs-lookup"><span data-stu-id="c8981-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- <span data-ttu-id="c8981-106">Kopa MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="c8981-106">Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com</span></span>
- <span data-ttu-id="c8981-107">Kopa MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test User" - LastName "Lietotājs"-nosaukums "Manager"-nodaļa "HR"</span><span class="sxs-lookup"><span data-stu-id="c8981-107">Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"</span></span>
- <span data-ttu-id="c8981-108">Noņemt MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com</span><span class="sxs-lookup"><span data-stu-id="c8981-108">Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com</span></span>