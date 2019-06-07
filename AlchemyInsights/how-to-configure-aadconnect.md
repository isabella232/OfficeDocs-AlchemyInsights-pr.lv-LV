---
title: 646 kā konfigurēt AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 646
ms.assetid: 599698ac-6709-477a-a66f-169b3165064e
ms.openlocfilehash: 2dc4ae7d6809c24ce599ac128570e9354c9f2b30
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34752568"
---
# <a name="configure-sync-features"></a>Konfigurēt sinhronizāciju līdzekļus

Debeszils AD Connect ir iekļauti vairāki līdzekļi, kas ir iespējoti pēc noklusējuma, vai varat aktivizēt vēlāk. Dažas funkcijas pieprasa papildu konfigurācijas noteiktu vidē.

- [Filtrēšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) robežas objekti tiek sinhronizēti ar debeszils reklāmu. Pēc noklusējuma, visi lietotāji, kontakti, grupas un Windows 10 datoru konti tiek sinhronizēti. Var iekļaut vai neiekļaut objektus, pamatojoties uz domēniem, OU vai citiem atribūtiem.

- [Parole hash sinhronizācijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizē paroli hash no lokālā Active Directory debeszils reklāmu. Tas ļauj paroles pārvaldība vienā atrašanās vietā, bet izmanto vienu un to pašu paroli abos telpās un mākonis vidēs. Tā kā Active Directory ir uzticams avots, var izmantot savas paroles politikas.

- [Pašapkalpošanās paroles atiestatīšanas (SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) ļauj lietotājiem atiestatīt savas paroles mākonis joprojām lietojot lokālā parole politika.

- [Writeback ierīce](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ļauj reģistrētajām ierīcēm debeszils reklāmu rakstīšanu atpakaļ lokālā Active Directory, tāpēc tos var izmantot, lai ierobežotu piekļuvi.

- [Novērst nejaušu dzēš](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) pēc noklusējuma ir iespējota, lai nepieļautu, ka pārāk daudz vienlaicīgas objektu dzēšanu (vairāk nekā 500 objekti vienā sinhronizācija). Jūs varat mainīt šo iestatījumu, lai atbilstu jūsu organizācijas prasībām.

- [Automātiska jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) tiek iespējota pēc noklusējuma izteikt instalācijām un palīdz nodrošināt Azure reklāmas, savienotu jūsu versija vienmēr ir pašreizējā.
