---
title: Grupas izveide
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
- "9003234"
- "7230"
ms.openlocfilehash: 4530abb3bf597458ea22441203a0db24b4b109f0760258310072891014c4b454
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53929312"
---
# <a name="create-a-group"></a>Grupas izveide

Šajā tēmā ir aprakstīta grupu izveide.

**Atļauja izveidot grupu**

Pārliecinieties, vai esat pilnvarots izveidot jaunu grupu. Globālie administratori var atspējot grupu izveidi Azure portālā vai piekļuves panelī. Iespējams, būs vajadzīgs administrators, lai izveidotu jaunu grupu jūsu vietā vai sniegtu jums atbilstošas atļaujas.

**Grupu izveides atļauju pārvaldība**

1. Globālie administratori var pārvaldīt grupu izveides atļaujas (ar drošību saistītu iemeslu dēļ) vai Office 365 grupas, kas izveidotas Azure portālā vai piekļuves panelī, izvēloties "Lietotāji var izveidot drošības grupas Azure portālā" vai "Lietotāji var izveidot Office 365 grupas Azure portālā" opcijas sadaļā Visu grupu vispārīgi  >  **(Iestatījumi)**.
2. Varat arī ierobežot grupu izveidi, lai atlasītu lietotāju grupu, ja jums ir Azure Active Directory P1 Premium licenci.

**Tiek atspējots paziņojums par esiet sveicināts Office 365 grupas dalībniekiem**

Sveiciena paziņojumu, kas tiek nosūtīts lietotājiem, kuri Office 365 grupām, var atspējot, Powershell iestatījumam **UnifiedGroupWelcomeMessageEnabled** iestatot vērtību False. Uzziniet par šo iestatījumu [šeit.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

