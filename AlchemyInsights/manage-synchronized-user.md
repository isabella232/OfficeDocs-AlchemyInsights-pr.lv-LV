---
title: Pārvaldīt sinhronizētu lietotāju
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000609"
- "2444"
ms.openlocfilehash: 0dc2ecfa0bb5703c619dc1b2d6b4d517f999da0d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823974"
---
# <a name="unable-to-set-primary-email-address-change-user-attributes-or-removedelete-a-synchronized-user"></a>Nevar iestatīt primāro e-pasta adresi, mainīt lietotāja atribūtus vai noņemt/dzēst sinhronizētu lietotāju

Ja jūsu vidē ir iespējota direktorija sinhronizēšana, dažus lietotāja vai objekta atribūtus nevar mainīt, izmantojot Microsoft 365 administrēšanas centru.

Lai pilnībā pārvaldītu sinhronizētos lietotājus un visus to atribūtus, izmantojiet lokālos Active Directory lietotājus un grupu pārvaldības konsoli (adsiedit.msc).  

Varat mainīt arī atsevišķus lietotājus vai atribūtus sinhronizētiem lietotājiem, kuri izmanto powershell, kā parādīts šajos bieži izmantotajos piemēros:

`Set-MsolUser -UserPrincipalName user@yourdomain.onmicrosoft.com -AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com`

`Set-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com" -DisplayName "Test User" -LastName "User" -Title "Manager" -Department "HR"`

`Remove-MsolUser -UserPrincipalName "user@yourdomain.onmicrosoft.com`
