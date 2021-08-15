---
title: Apple automātiskās ierīces reģistrācijas sinhronizācijas kļūdas
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
ms.openlocfilehash: 1664a26b313c4a38c9c6d78cdb89997749ba175fd3dd72f278e99bbd50b0ee84
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013755"
---
# <a name="apple-automatic-device-enrollment-sync-errors"></a>Apple automātiskās ierīces reģistrācijas sinhronizācijas kļūdas

"Mēs konstatējām, ka jums ir viens vai vairāki ADE/DEP marķieri, kas ir kļūdas stāvoklī. Līdz kļūdas stāvoklis nav atrisināts katrai ietekmētajam marķierim, ADE funkcionalitāte nedarbojas, kā paredzēts.".

Šī kļūda var rasties vairākos veidos, tostarp:

1. Ierīces, iespējams, netiek sinhronizētas no ABM/ASM uz Intune
2. Reģistrācijas profilu piešķiršana var būt neveiksmi
3. Ierīces, iespējams, nevar sekmīgi pabeigt ADE reģistrāciju

Pārbaudiet, vai sinhronizācijas kļūda uzrādīta Intune konsolē sadaļā Ierīces, > reģistrē ierīces > Apple reģistrācija **> reģistrācijas programmas marķieriem.**

Viens no biežākajiem sinhronizācijas kļūdas iemesliem ir pašreizējā marķiera derīguma beigas. Daudzos gadījumos problēma tiks novērsta, atjaunojot ietekmēto marķieri.

Ja ir beidzies viena vai vairākiem marķieriem derīgums, skatiet tālāk norādīto dokumentāciju, lai saņemtu atbilstošu palīdzību par atjaunošanu:

[Automatizētas ierīces reģistrācijas pilnvaras atjaunošana](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment-program-enroll-ios#renew-an-automated-device-enrollment-token)

Turklāt varat skatīt tālāk norādīto dokumentāciju, lai redzētu iespējamos koriģēšanu citām kļūdām, kas izraisa marķiera sinhronizācijas kļūmes:

[ABM/ASM sinhronizācijas kļūdas iOS/iPadOS un macOS automatizētajai ierīces reģistrācijas marķieriem](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#sync-token-errors-between-intune-and-ade-dep)







[ABM/ASM sinhronizācijas kļūdas iOS/iPadOS un macOS automatizētajai ierīces reģistrācijas marķieriem](https://docs.microsoft.com/mem/intune/enrollment/troubleshoot-ios-enrollment-errors#resolutions-when-syncing-tokens-between-intune-and-abmasm-for-automated-device-enrollment)
