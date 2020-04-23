---
title: 646 kā konfigurēt AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "646"
- "1300023"
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 713cda26e55f07f0438cb9ebe5aa9da86c4ebb3a
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43722570"
---
# <a name="configure-sync-features"></a>Sinhronizācijas līdzekļu konfigurēšana

Azure AD Connect ietver vairākus līdzekļus, kas ir iespējoti pēc noklusējuma vai kurus var iespējot vēlāk. Dažām funkcijām ir nepieciešama papildu konfigurācija konkrētās vidēs.

- [Filtrēšanas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ierobežojumi objekti tiek SINHRONIZĒTI Azure ad. Pēc noklusējuma tiek sinhronizēti visi lietotāji, kontaktpersonas, grupas un Windows 10 datora konti. Var iekļaut vai neiekļaut objektus, kuru pamatā ir domēni, OUs vai citi atribūti.

- [Paroļu jaukšanas sinhronizēšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizē paroli hash no lokālā Active Directory Azure ad. Tas ļauj pārvaldīt paroli vienā atrašanās vietā, bet izmantot vienu un to pašu paroli gan lokālas, gan mākoņa vidē. Tā kā Active Directory ir autoritatīvs avots, varat izmantot savas paroļu politikas.

- [Pašapkalpošanās paroles atiestatīšana (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ļauj lietotājiem atiestatīt savas paroles mākonī, joprojām lietojot lokālo paroļu politiku.

- [Ierīce arī atpakaļrakstīšanas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ļauj reģistrētas ierīces Azure ad jāraksta atpakaļ lokālā Active Directory, lai tos var izmantot ierobežotas piekļuves.

- [Novērst nejaušu dzēšanu](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) ir iespējota pēc noklusējuma, lai palīdzētu novērst pārāk daudz vienlaicīgu objektu dzēšanu (vairāk nekā 500 objektus katrā sinhronizācijā). Šo iestatījumu var mainīt, lai tas atbilstu jūsu organizācijas vajadzībām.

- [Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) ir iespējota pēc noklusējuma Express instalācijas un palīdz nodrošināt savu VERSIJU Azure ad savienojumu vienmēr ir spēkā.
