---
title: Ziņojuma dzēšanas notikumu identificēšana audita žurnālos
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: f5d6041fd80b4d5cae610e7d9248e45ed410a3d9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58317601"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Izdzēsto e-pasta ziņojumu auditēšanas žurnāli

Sākot ar 2019. gada janvāri, Microsoft pēc noklusējuma ieslēdz pastkastes audita reģistrēšanu. Pretējā gadījumā, lai pārskatītu ziņojuma dzēšanas notikumus konkrētam lietotājam, ir manuāli jāiespējo dzēšanas darbības auditēšanas vajadzībām. Ja pastkastes audita reģistrēšana jau ir iespējota jūsu organizācijai vai konkrētam lietotājam, veiciet tālāk norādītās darbības.

1. Piesakieties [Microsoft 365 atbilstības centrā](https://protection.office.com/)

2. Noklikšķiniet **uz Meklēšana un izpēte** un atlasiet Meklēšana **audita žurnālā.**

3. Atlasiet datumu diapazonu laukos **Sākuma datums** **un Beigu** datums. Norādiet tā lietotāja lietotājvārdu, kuru vēlaties izpētīt (lietotājs, kurš izdzēsa vienumus). Laukā **Darbības** atlasiet Izdzēstie **ziņojumi no mapes Izdzēstie vienumi un Pārvietoti** ziņojumi uz mapi **Izdzēstie vienumi.**

4. Noklikšķiniet **uz Meklēt.**

Rezultātos atlasiet audita ierakstu. Detalizētas informācijas izlidošanas lodziņā noklikšķiniet uz **Papildinformācija**. Papildinformācija par izdzēsto vienumu (piemēram, tēmas rindiņa un vienuma atrašanās vieta, kad tas tika izdzēsts) tiek rādīta **laukā AffectedItems.** Rekvizīts **ClientInfoString** tiek rādīts, ja dzēšana notika Outlook, Outlook tīmeklī (iepriekš tika dēvēta par Outlook Web App) vai jebkurā citā ierīcē.

Papildinformāciju skatiet rakstā [Noteikšana, kas iestatīja e-pasta pārsūtīšanu pastkastei.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items)

**Piezīme.** Izdzēstos vienumus nevar izgūt, izmantojot audita žurnāla līdzekli. Lai izgūtu izdzēstos ziņojumus Outlook tīmeklī, skatiet [rakstu Izdzēsto vienumu atkopšana Outlook Web App.](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4)
