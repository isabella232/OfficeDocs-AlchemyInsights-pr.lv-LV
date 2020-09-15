---
title: 646 kā konfigurēt AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 6327e42b74283d732247c9a847c68db72082c56a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47704496"
---
# <a name="configure-sync-features"></a>Sinhronizācijas līdzekļu konfigurēšana

Azure AD Connect ietver vairākus līdzekļus, kas ir iespējoti pēc noklusējuma, vai arī tos var iespējot vēlāk. Dažiem līdzekļiem ir nepieciešama papildu konfigurācija noteiktās vidēs.

- [Filtrēšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ierobežo objektu sinhronizēšanu ar Azure AD. Pēc noklusējuma tiek sinhronizēti visi lietotāji, kontaktpersonas, grupas un Windows 10 datora konti. Varat iekļaut vai izslēgt objektus atkarībā no domēniem, OU vai citiem atribūtiem.

- [Paroļu jaukšanas sinhronizācija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizē paroļu hash no lokālā Active Directory uz Azure AD. Tas nodrošina paroļu pārvaldību vienā atrašanās vietā, bet to pašu paroli izmanto gan lokālajā, gan mākoņa vidē. Tā kā Active Directory ir autoritatīvais avots, varat izmantot savas paroļu politikas.

- Pašapkalpošanās [paroles atiestatīšana (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ļauj lietotājiem atiestatīt savas paroles mākonī, vienlaikus pievienojot savu lokālo paroļu politiku.

- Izmantojot [ierīces arī atpakaļrakstīšanas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) , Azure AD reģistrētās ierīces tiek atveidotas atpakaļ uz lokālo Active Directory, lai tos varētu izmantot piekļuvei ar ierobežotu piekļuvi.

- Ja pēc noklusējuma ir iespējota [nejauša](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) izdzēšana, lai novērstu vairāku vienlaicīgu objektu dzēšanu (vairāk nekā 500 objekti uz sinhronizāciju). Jūs varat mainīt šo iestatījumu, lai apmierinātu savas organizācijas vajadzības.

- [Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) pēc noklusējuma ir iespējota Express instalācijām un palīdz nodrošināt, ka jūsu Azure AD Connect versija vienmēr ir aktuāla.
