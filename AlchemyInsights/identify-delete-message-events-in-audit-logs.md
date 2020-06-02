---
title: Identificētu dzēst ziņojumu notikumus audita žurnālos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508995"
---
# <a name="audit-logs-for-deleted-email-messages"></a>Audita žurnālus dzēstiem e-pasta ziņojumiem

Sākot ar 2019 janvārī, Microsoft ieslēdzot pastkastes audita reģistrēšanu pēc noklusējuma. Pretējā gadījumā, lai pārskatītu dzēst ziņojumu notikumus noteiktam lietotājam, ir manuāli jāiespējo dzēšanas darbības auditēšanai. Ja pastkastes audita reģistrēšana jau ir iespējota jūsu organizācijai vai noteiktam lietotājam, veiciet tālāk norādītās darbības.

1. Pieteikšanās [Microsoft 365 drošības & atbilstības centrs](https://protection.office.com/)

2. Noklikšķiniet uz **meklēšana un izmeklēšana** un atlasiet **audita žurnāla meklēšana**.

3. Laukā **sākuma datums** un **beigu datums** atlasiet datumu diapazonu. Norādiet tā lietotāja lietotājvārdu, kuru vēlaties izpētīt (lietotājs, kurš izdzēsis vienumus). Laukā **darbības** atlasiet **Izdzēstie ziņojumi no mapes Izdzēstie vienumi** un **mapē ziņojumi pārvietoti uz mapi Izdzēstie vienumi**.

4. Noklikšķiniet uz **Meklēt**.

Rezultātos atlasiet audita ierakstu. Detalizētās informācijas izlidošanas noklikšķiniet uz **Papildinformācija**. Laukā **Affecteditems** tiek parādīta papildinformācija par izdzēsto elementu (piemēram, tēmas rindiņa un vienuma atrašanās vieta, kad tā tika izdzēsta). Rekvizītā **Clientinfostring** tiks parādīts, ja programmā Outlook, Outlook Web (iepriekš pazīstams kā Outlook Web App) vai jebkuras citas ierīces dzēšanu.

Lai iegūtu papildinformāciju, skatiet [noteikt, kurš ir iestatījis e-pasta pārsūtīšanu pastkastei](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).

**Piezīme**: nevar izgūt izdzēstos vienumus, izmantojot audita žurnāla līdzekli. Lai izgūtu izdzēstos ziņojumus programmā Outlook tīmeklī, skatiet sadaļu [izdzēsto vienumu atkopšana programmā Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).
