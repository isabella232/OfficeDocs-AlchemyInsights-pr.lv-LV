---
title: Dzēst ziņojuma notikumu noskaidrošana audita žurnālos
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
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696520"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Izdzēsto e-pasta ziņojumu audita žurnāli

Sākot ar 2019. janvāri, Microsoft pēc noklusējuma ieslēdz pastkastes audita reģistrēšanu. Pretējā gadījumā, lai pārskatītu dzēst ziņojuma notikumus konkrētam lietotājam, ir manuāli jāiespējo dzēšanas darbības auditēšanai. Ja jums jau ir iespējota pastkastes audita reģistrēšana jūsu organizācijai vai konkrētam lietotājam, veiciet tālāk norādītās darbības.

1. Piesakieties [Microsoft 365 drošības & atbilstības centrā](https://protection.office.com/)

2. Noklikšķiniet uz **meklēšana un izpēte** un atlasiet **audita žurnālu meklēšana**.

3. Atlasiet datumu diapazonu lauku **sākuma datums** un **beigšanas datums** . Norādiet tā lietotāja lietotājvārdu, kuru vēlaties izpētīt (lietotāju, kurš izdzēsis šos vienumus). Laukā **aktivitātes** atlasiet **Izdzēstie ziņojumi no mapes** Izdzēstie vienumi un **pārvietoti ziņojumi uz mapi Izdzēstie vienumi**.

4. Noklikšķiniet uz **Meklēt**.

Rezultātos atlasiet audita ierakstu. Detalizētas informācijas izlidošanas sarakstā noklikšķiniet uz **Papildinformācija**. Papildinformāciju par izdzēsto vienumu (piemēram, tēmas rindiņu un vienuma atrašanās vietu, kad tas tika izdzēsts) tiek parādīta laukā **AffectedItems** . Rekvizīts **ClientInfoString** tiek parādīts, ja dzēšana notiek programmā Outlook, Outlook tīmeklī (iepriekš zināma kā Outlook Web App) vai jebkura cita ierīce.

Papildinformāciju skatiet rakstā [e-pasta pārsūtīšanas iestatīšana pastkastei](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Piezīme**. jūs nevarat izgūt izdzēstos vienumus, izmantojot audita žurnālu līdzekli. Lai izdzēstos ziņojumus izgūtu programmā Outlook tīmeklī, skatiet rakstu [izdzēsto vienumu atkopšana programmā Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
