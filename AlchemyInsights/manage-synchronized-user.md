---
title: Pārvaldīt sinhronizēto lietotāju
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
ms.openlocfilehash: 84e337a7224fdd3c3ab7ad0f61240692fe007d5a
ms.sourcegitcommit: 82af227ac6d075e748e27c4ce6bdcf56628559cb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/28/2020
ms.locfileid: "44407357"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a><span data-ttu-id="e1fd4-102">Nevar iestatīt primāro e-pasta adresi, mainīt lietotāja atribūtus vai noņemt/dzēst sinhronizēto lietotāju</span><span class="sxs-lookup"><span data-stu-id="e1fd4-102">Unable to set primary email address, change user attributes, or remove/delete a synchronized user</span></span>

<span data-ttu-id="e1fd4-103">Ja jūsu vidē ir iespējota direktorija sinhronizēšana, dažas lietotāja vai objekta atribūtus nevar mainīt, izmantojot Microsoft 365 administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="e1fd4-103">If directory synchronization is enabled for your environment, some user or object attributes cannot be changed using the Microsoft 365 admin center.</span></span>

<span data-ttu-id="e1fd4-104">Lai pilnībā pārvaldītu sinhronizētos lietotājus un visus to atribūtus, izmantojiet lokālo Active Directory lietotāju un grupu pārvaldības konsoli (ADSIEDIT. msc).</span><span class="sxs-lookup"><span data-stu-id="e1fd4-104">To fully manage synchronized users and all their attributes, use your local active directory users and groups management console (adsiedit.msc).</span></span>  

<span data-ttu-id="e1fd4-105">Alternatīvi, jūs varat mainīt atsevišķus lietotājus vai atribūtus sinhronizēto lietotājiem, izmantojot PowerShell, piemēram, kā parādīts šajos kopējos piemēros:</span><span class="sxs-lookup"><span data-stu-id="e1fd4-105">Alternatively, you can change individual users or attributes for synchronized users using powershell such as shown in these common examples:</span></span> 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
