---
title: Diska vietas atbrīvošana operētājsistēmā Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036589"
---
# <a name="free-up-drive-space-in-windows-10"></a>Diska vietas atbrīvošana operētājsistēmā Windows 10

Tālāk ir divas iespējas, kā atbrīvot vietu diskā operētājsistēmā Windows.

- Atbrīvojiet vietu diskā operētājsistēmā Windows 10.
- Atbrīvojiet vietu Windows 10 atjauninājumiem ar ārējās krātuves ierīci.

Ja pēc diska tīrīšanas joprojām ir maz brīvas vietas, iespējams, ka jūsu Temp mape ir ātri piepildīta ar lietojumprogrammu (. Appx) failiem, ko izmanto Microsoft Store. Lai novērstu šo problēmu, atiestatiet veikalu, notīriet veikala kešatmiņu un pēc tam palaidiet Windows Update problēmu risinātāju. Pirms turpināt šīs darbības, pārliecinieties, vai Microsoft veikals ir aizvērts.

**1. darbība: Microsoft Store atiestatīšana**

**Piezīmes** Šī darbība neatgriezeniski izdzēš lietojumprogrammas datus ierīcē, ieskaitot jūsu preferences un pierakstīšanās informāciju.

1. Atlasiet **Sākt**  >  **iestatījumu**  >  **programmu**  >  **programmas & līdzekļus**.

1. Programmu sarakstā atrodiet un atlasiet Microsoft Store.

1. Atlasiet **Papildu opcijas**.

1. Ritiniet uz leju un atlasiet **Atiestatīt** un pēc tam **apstipriniet atiestatīšanu**.

**2. darbība: Microsoft Store kešatmiņas notīrīšana**

1. Nospiediet Windows logotipa taustiņu + R, lai atvērtu palaišanas dialoglodziņu.

1. Ierakstiet wsreset.exe un atlasiet **Labi**.

1. Tiek atvērts tukšs komandu uzvednes logs. Pēc aptuveni 10 sekundēm logs tiek aizvērts, un krātuve tiek atvērta automātiski.

**3. darbība: atiestatiet Windows Update**

1. Atlasiet **Sākt**  >  **iestatījumu**  >  **atjaunināšanu & drošības**  >  **problēmu novēršana**.

1. Ritiniet uz leju un sarakstā atlasiet **Windows Update** un atlasiet **palaist problēmu risinātāju**.

1. Restartējiet datoru un pārbaudiet, vai joprojām rodas problēma.

