---
title: Grupas izveide
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003234"
- "7230"
ms.openlocfilehash: b8cb3f1de991bfe7197607d5e8964a018e31c122
ms.sourcegitcommit: 35e2c122d8a838d98d1f0851c29b16282261580f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/17/2020
ms.locfileid: "49088907"
---
# <a name="create-a-group"></a>Grupas izveide

Šajā tēmā ir aprakstīta grupas izveide.

**Atļauja izveidot grupu**

Pārliecinieties, vai jums ir atļauja izveidot jaunu grupu. Globālie administratori var atspējot grupu izveidi Azure portālā vai piekļuves panelī. Iespējams, ka jums ir nepieciešams administrators, lai izveidotu jaunu grupu vai piešķirtu atbilstošas atļaujas.

**Grupu izveides atļauju pārvaldība**

1. Globālie administratori var pārvaldīt grupu izveides atļaujas (ar drošību saistītus iemeslus) vai Office 365 grupas, kas izveidotas Azure portālā vai piekļuves panelī, izvēloties "lietotāji var izveidot drošības grupas Azure portāliem" vai "lietotāji var izveidot Office 365 grupas Azure portāli" opcijas visās **grupās**  >  **Vispārīgi (iestatījumi)**.
2. Varat arī ierobežot grupu izveidi, lai atlasītu lietotāju grupu, ja jums ir Azure Active Directory P1 Premium licence.

**Sveiciena paziņojuma par jauniem Office 365 grupas dalībniekiem atspējošana**

Sveiciena paziņojumu, kas nosūtīts lietotājiem, kuri tiek pievienoti Office 365 grupām, var atspējot, iestatot **UnifiedGroupWelcomeMessageEnabled** uz Aplams programmā PowerShell. Uzziniet par šo iestatījumu [šeit](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true).

