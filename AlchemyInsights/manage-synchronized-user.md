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
# <a name="unable-to-set-primary-email-address-or-change-user-attributes"></a>Nevar iestatīt primāro e-pasta adresi vai mainīt lietotāja atribūtus

Par savu vidi, aktivizējot direktoriju sinhronizācijas dažus lietotāju vai objekta atribūtus nevar mainīt, izmantojot administrēšanas centrs.
Pilnībā vadīt sinhronizēto lietotāju un to atribūtus, izmantojiet jūsu vietējā aktīvā direktorija lietotāji un grupas pārvaldības konsoli (adsiedit.msc).  

Var arī mainīt atsevišķus lietotājus vai sinhronizēto lietotāju, izmantojot powershell, piemēram, norādīts piemēros kopīgas īpašības: 
- Kopa MsolUser - UserPrincipalName user@yourdomain.onmicrosoft.com - AlternateEmailAddresses user2@yourvanitydomain.onmicrosoft.com
- Kopa MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com" - DisplayName "Test User" - LastName "Lietotājs"-nosaukums "Manager"-nodaļa "HR"
- Noņemt MsolUser - UserPrincipalName "user@yourdomain.onmicrosoft.com