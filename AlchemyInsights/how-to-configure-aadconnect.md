---
title: 646 Kā konfigurēt AADConnect
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
ms.openlocfilehash: c5fa5fd7586f999698fe43554fb9a2b205be3e25740c20763254a38d41297e0c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53963650"
---
# <a name="configure-sync-features"></a>Sinhronizācijas līdzekļu konfigurēšana

Azure AD Savienošana iekļauti vairāki līdzekļi, kas ir iespējoti pēc noklusējuma vai kurus varat iespējot vēlāk. Dažiem līdzekļiem nepieciešama papildu konfigurācija konkrētā vidē.

- [Filtrēšanas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-configure-filtering) ierobežojumi. Objekti tiek sinhronizēti ar Azure AD. Pēc noklusējuma tiek sinhronizēti visi lietotāji, kontaktpersonas, Windows 10 un datora konti. Varat iekļaut vai izslēgt objektus, kuru pamatā ir domēni, OU vai citi atribūti.

- [Paroļu jaukšanas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-implement-password-hash-synchronization) sinhronizācija sinhronizē paroles jaukšanas objektu no lokālā Active Directory uz Azure AD. Tas ļauj paroļu pārvaldību vienā atrašanās vietā, bet vienu un to pašu paroli izmantot gan lokālajā, gan mākoņa vidē. Tā kā Active Directory ir autoritatīvs avots, varat izmantot savas paroļu politikas.

- [Pašapkalpošanās paroles atiestatīšana (Self-service password reset — SSPR)](https://docs.microsoft.com/azure/active-directory/authentication/quickstart-sspr) sniedz lietotājiem iespēju atiestatīt savas paroles mākonī, vienlaikus lietojot savu lokālo paroļu politiku.

- [Ierīces writeback](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-device-writeback) ļauj Azure AD reģistrētas ierīces ierakstīt atpakaļ lokālajā Active Directory, lai tās varētu izmantot nosacījuma piekļuvei.

- [Pēc noklusējuma ir iespējots](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-feature-prevent-accidental-deletes) novērst nejaušu dzēšanu, lai nepieļautu pārāk daudz vienlaicīgu objektu dzēšanu (vairāk nekā 500 objektu vienā sinhronizācijā). Šo iestatījumu varat mainīt, lai tas atbilstu jūsu organizācijas vajadzībām.

- [Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade) pēc noklusējuma ir iespējota ekspresinstalācijām un palīdz nodrošināt, ka jūsu Azure AD Savienošana vienmēr ir aktuāla.
