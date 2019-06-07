---
title: Noteiktu dzēšanas ziņu notikumiem audita žurnālos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 0fb5d6aa0c99f7f68459c40302869bed69583b3f
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34755159"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Audita žurnālos, dzēstie e-pasta ziņojumiem

Sākot ar janvāra 2019, Microsoft ir pagrieziena pastkastes audita pieteikšanās pēc noklusējuma. Pretējā gadījumā pārskatīt dzēst ziņu notikumiem konkrētu lietotāju, ir jāiespējo manuāli dzēst darbības revīziju. Ja pastkastes audita reģistrēšana ar operatora palīdzību jau bijusi iespējota jūsu uzņēmumam vai noteiktam lietotājam, veiciet tālāk norādītās darbības.

1. [Office drošības 365 & atbilstību centra](https://protection.office.com/) pieteikties

2. Noklikšķiniet uz **meklēšanas un izmeklēšanas** un atlasiet **Audita žurnālu meklēšana**.

3. Atlasiet datumu diapazona **sākuma datums** un **beigu datums** laukos. Jānorāda lietotājvārds lietotājam, kuru vēlaties izpētīt (lietotājs, kurš Izdzēstie vienumi). **Darbības** lauks atlasiet **Izdzēstie ziņojumi no mapes Izdzēstie vienumi** un **Moved ziņojumus uz mapi Izdzēstie vienumi**.

4. Noklikšķiniet uz **Meklēt**.

Rezultātos atzīmējiet auditācijas ierakstu. Flyout detaļas, noklikšķiniet uz **Papildinformācija**. Papildu informāciju par dzēsto vienumu (piemēram, tēmas rindu un vienums, kad to dzēsa atrašanās vieta) ir rādīts laukā **AffectedItems** . **ClientInfoString** īpašuma rādīs, ja programmā Outlook, Outlook web (agrāk pazīstama kā Outlook Web App) vai kādu citu ierīci, radās dzēšanu.

Plašāku informāciju skatiet [noteikšana, kas izveido e-pasta pāradresācija uz pastkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).

**Piezīme**: izmantojot funkciju audita žurnāla izdzēsto vienumu nevar izgūt. Lai izgūtu izdzēstos ziņojumus Outlook Web, skatiet [Atkopt izdzēstos vienumus programmā Outlook tīmekļa lietojumprogramma](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
