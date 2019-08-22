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
ms.openlocfilehash: a943c59d67c512e6326856dacd0053db121f6aa3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36542003"
---
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Nevar iestatīt primāro e-pasta adresi vai mainīt lietotāja atribūtus

Ja directory sinhronizācija ir iespējota jūsu vidē, dažus lietotāju vai objekta atribūtus nevar mainīt, izmantojot Microsoft 365 administrēšanas centrs.

Pilnībā vadīt sinhronizēto lietotāju un to atribūtus, izmantojiet jūsu vietējā aktīvā direktorija lietotāji un grupas pārvaldības konsoli (adsiedit.msc).  

Var arī mainīt atsevišķus lietotājus vai sinhronizēto lietotāju, izmantojot powershell, piemēram, norādīts piemēros kopīgas īpašības: 
- Kopa MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Kopa MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test User" - LastName "Lietotājs"-nosaukums "Manager"-nodaļa "HR"
- Noņemt MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com