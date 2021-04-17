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
ms.openlocfilehash: ec74b7c098d302d3bdeb5a412fad41efe7b82b98
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816363"
---
# <a name="create-a-group"></a>Grupas izveide

Šajā tēmā ir aprakstīta grupu izveide.

**Atļauja izveidot grupu**

Pārliecinieties, vai esat pilnvarots izveidot jaunu grupu. Globālie administratori var atspējot grupu izveidi Azure portālā vai piekļuves panelī. Iespējams, būs vajadzīgs administrators, lai izveidotu jaunu grupu jūsu vietā vai sniegtu jums atbilstošas atļaujas.

**Grupu izveides atļauju pārvaldība**

1. Globālie administratori var pārvaldīt grupu izveides atļaujas (ar drošību saistītu iemeslu dēļ) vai Office 365 grupas, kas izveidotas Azure portālā vai piekļuves panelī, izvēloties "Lietotāji var izveidot drošības grupas Azure portālā" vai "Lietotāji var izveidot Office 365 grupas Azure portālā" opcijas Sadaļā Vispārīgi  >  **(Iestatījumi).**
2. Varat arī ierobežot grupu izveidi, lai atlasītu lietotāju grupu, ja jums ir Azure Active Directory P1 Premium licence.

**Tiek atspējots paziņojums par esiet sveicināts! jauniem Office 365 grupas dalībniekiem**

Lietotājiem, kuri ir pievienoti Office 365 grupām, nosūtīto sveiciena paziņojumu var atspējot, Powershell iestatījumam **UnifiedGroupWelcomeMessageEnabled** iestatot vērtību False. Uzziniet par šo iestatījumu [šeit.](https://docs.microsoft.com/powershell/module/exchange/set-unifiedgroup?view=exchange-ps&preserve-view=true)

