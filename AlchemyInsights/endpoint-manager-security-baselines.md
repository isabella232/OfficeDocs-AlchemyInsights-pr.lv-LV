---
title: EndPoint pārvaldnieks — drošības bāzes rādītāji
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421083"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint pārvaldnieks — drošības bāzes rādītāji

Drošības bāzes datu bāzes ir iepriekš konfigurētas Windows iestatījumu grupas, kas palīdz lietot atbilstošo drošības grupu ieteiktos drošības iestatījumus. Šos bāzes datu laukus var pielāgot, lai nodrošinātu tikai vajadzīgos iestatījumus un vērtības. Papildinformāciju par drošības bāzes datu bāzes datu skatiet rakstā Drošības bāzes datu [izmantošana Windows 10 ierīču konfigurēšanai intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Šiem produktiem pašlaik ir pieejami bāzes dati:

- Windows MDM drošības iestatījumi
- Microsoft Defender lietotājam EndPoint drošība
- Microsoft Edge

Katrs bāzes datu objekts tiek periodiski atjaunināts un izlaists inkrementālajās versijās. Katra versija pievieno un vai noņem iestatījumus no iepriekšējās versijas, lai nodrošinātu, ka bāzes datus atbilst pašreizējiem norādījumiem. Galapunkta drošības drošības konsolē var salīdzināt dažādas versijas, tādējādi kļūstot redzamas izmaiņas no versijas uz versiju.

Norādījumus par to, kā efektīvāk mainīt bāzes datu versiju, skatiet rakstā Drošības bāzlīniju profilu pārvaldība [programmā Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)

Pēc drošības bāzes datu izvietošanas varat pārraudzīt izvietošanas stāvokli un pārskatīt iestatījumus pa ierīcēm.

**Piezīme.** Var paiet līdz pat 24 stundām, līdz bāzes datu atskaites dati tiek parādīti no sākotnējās izvietošanas ierīcē, un var būt nepieciešamas līdz pat 6 stundām, lai iegūtu atjauninājumus. 

Visbiežākais bāzlīniju iestatījuma cēlonis, kas netiek lietots, ir tas pats iestatījums, kas tiek izmantots citā profilā. Šo scenāriju var izpētīt konkrētām ierīcēm, atlasot šo ierīci profila Drošības bāzlīnija mezglā Ierīces statuss. Detalizētu informāciju skatiet rakstā [Drošības bāzes datu konfliktu atrise.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)