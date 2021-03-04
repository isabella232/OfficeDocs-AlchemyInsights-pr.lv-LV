---
title: Apple automātiskās ierīču reģistrācijas sinhronizācijas kļūdas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000654"
- "7256"
ms.openlocfilehash: 912c9e56b4c468fb333769f15bd7c212594dc11a
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50448929"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple automātiskās ierīču reģistrācijas sinhronizācijas kļūdas

"Mēs noteikuši, ka jums ir viena vai vairākas ADE/DEP marķierierīces, kas ir kļūdas stāvoklī. Līdz kļūdas stāvokļa atrisināšanai katrai ietekmētajai pilnvarai, funkcija ADE nedarbojas, kā paredzēts.

Šī kļūda var izpausties vairākos veidos, tostarp:

1. Ierīces var netikt sinhronizētas no ABM/ASM uz Intune
2. Reģistrācijas profila uzdevumi var neizdoties
3. Ierīces var neveiksmīgi pabeigt ADE pieteikšanos

Meklējiet sinhronizācijas kļūdu, kas tiek ziņota Intune konsolē sadaļā **ierīces > reģistrēt ierīces > Apple reģistrācijas > reģistrācijas programmas pilnvaras**.

Viens no biežākajiem sinhronizācijas kļūdas iemesliem ir pašreizējās marķierierīces derīguma termiņš. Daudzi gadījumi atrisinās ietekmētās marķierierīces problēmu.

Ja vienai vai vairākām pilnvarām ir beidzies derīgums, skatiet tālāk norādītās dokumentācijas, kas palīdzēs tās atjaunot, ja nepieciešams.

[Automātiskas reģistrācijas marķierierīces atjaunošana](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Turklāt varat skatīt tālāk norādīto dokumentāciju, lai skatītu iespējamās atrisināšanas iespējas citām kļūdām, kas izraisa marķiera sinhronizācijas kļūdas:

[ABM/ASM sinhronizācijas kļūdas iOS/iPadOS un macOS automatizētās ierīču reģistrācijas marķierierīcēs](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM sinhronizācijas kļūdas iOS/iPadOS un macOS automatizētās ierīču reģistrācijas marķierierīcēs](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
