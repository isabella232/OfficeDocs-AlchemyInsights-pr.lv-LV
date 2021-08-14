---
title: EndPoint Manager — drošības bāzes
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
- "10064"
- "9003771"
ms.openlocfilehash: c13bc161b19a5fef1352beb28bdcc20110111a9a61a47433d82e1e69aff7f88d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53978168"
---
# <a name="endpoint-manager---security-baselines"></a>EndPoint Manager — drošības bāzes

Drošības bāzes ir iepriekš konfigurētas Windows iestatījumu grupas, kas palīdz lietot atbilstošo drošības grupu ieteiktos drošības iestatījumus. Šīs bāzes var pielāgot, lai nodrošinātu tikai vajadzīgos iestatījumus un vērtības. Papildinformāciju par drošības bāzēm skatiet rakstā [Drošības bāžu izmantošana, lai konfigurētu Windows 10 ierīces Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).

Pašlaik ir pieejamas bāzes šiem produktiem:

- Windows MDM drošības iestatījumi
- Microsoft Defender galapunkta aizsardzībai
- Microsoft Edge

Katra bāze tiek periodiski atjaunināta un izlaista inkrementālās versijās. Katrā versijā tiek pievienoto vai noņemti iestatījumi no iepriekšējās versijas, lai nodrošinātu, ka bāze atbilst pašreizējiem norādījumiem. Drošības bāzes konsole Endpoint Security ļauj salīdzināt dažādas versijas, padarot redzamas izmaiņas no versijas uz versiju.

Norādījumus par to, kā efektīvāk mainīt to, kāda bāzes versija tiek izvietota, skatiet rakstā [Drošības bāzu profilu pārvaldība Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).

Pēc drošības bāzes izvietošanas varat pārraudzīt izvietošanas stāvokli un pārskatīt iestatījumus katru ierīci atsevišķi.

**Piezīme.** Bāzu atskaišu datu parādīšana var ilgt līdz pat 24 stundām no sākotnējās izvietošanas ierīcē un līdz pat 6 stundām papildu atjauninājumiem. 

Visbiežāk bāzes iestatījums netiek lietots tāpēc, ka tāds pats iestatījums tiek izmantots citā profilā. Šo scenāriju var izpētīt konkrētām ierīcēm, atlasot šo ierīci profila Drošības bāzes datu mezglā Ierīces statuss. Detalizētu informāciju skatiet rakstā [Konfliktu atrisināšana drošības bāzēm](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).