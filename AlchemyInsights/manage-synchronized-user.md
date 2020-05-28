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
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nevar iestatīt primāro e-pasta adresi, mainīt lietotāja atribūtus vai noņemt/dzēst sinhronizēto lietotāju

Ja jūsu vidē ir iespējota direktorija sinhronizēšana, dažas lietotāja vai objekta atribūtus nevar mainīt, izmantojot Microsoft 365 administrēšanas centrs.

Lai pilnībā pārvaldītu sinhronizētos lietotājus un visus to atribūtus, izmantojiet lokālo Active Directory lietotāju un grupu pārvaldības konsoli (ADSIEDIT. msc).  

Alternatīvi, jūs varat mainīt atsevišķus lietotājus vai atribūtus sinhronizēto lietotājiem, izmantojot PowerShell, piemēram, kā parādīts šajos kopējos piemēros: 
- `Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

- `Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

- `Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
