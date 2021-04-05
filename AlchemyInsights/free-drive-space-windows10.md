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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505363"
---
# <a name="free-up-drive-space-in-windows-10"></a>Diska vietas atbrīvošana operētājsistēmā Windows 10

Šeit ir divas opcijas, lai atbrīvotu diska vietu operētājsistēmā Windows 10:

- Diska vietas atbrīvošana operētājsistēmā Windows 10.
- Atbrīvojiet vietu operētājsistēmas Windows 10 atjauninājumiem, izmantojot ārējo krātuves ierīci.

Ja pēc diska tīrīšanas izmantošanas vēl joprojām ir maz vietas diskā, iespējams, ka mape Temp ātri tiek piepildīta ar programmas (.appx) failiem, kurus izmanto Microsoft Store. Lai novērstu šo problēmu, atiestatiet Microsoft Store, iztīriet tā kešatmiņu un pēc tam palaidiet Windows Update problēmu risinātāju. Pirms šo darbību veikšanas pārliecinieties, vai Microsoft Store ir aizvērts.

**1. darbība: Microsoft Store atiestatīšana**

**Piezīme** Tādējādi ierīcē tiks neatgriezeniski izdzēsti programmas dati, tostarp jūsu preferences un pierakstīšanās dati.

1. Atlasiet **Sākt** > **, Iestatījumi** > **, Programmas** > **,Programmas un līdzekļi**.

1. Programmu sarakstā atrodiet un atlasiet Microsoft Store.

1. Atlasiet **Papildu opcijas**.

1. Ritiniet uz leju un atlasiet **Atiestatīt** un pēc tam **Apstiprināt atiestatīšanu**.

**2. darbība: Microsoft Store kešatmiņas notīrīšana**

1. Nospiediet taustiņu kombināciju Windows logotipa taustiņš+R, lai atvērtu un palaistu dialoglodziņu.

1. Ierakstiet wsreset.exe un atlasiet **Labi**.

1. Atveras tukšs komandu uzvednes logs. Pēc aptuveni 10 sekundēm logs aizveras un Microsoft Store atveras automātiski.

**3. darbība: Windows Update atiestatīšana**

1. Atlasiet **Sākt** > **, Iestatījumi** > **, Atjauninājumi un drošība** > **, Problēmu novēršana**.

1. Ritiniet uz leju un sarakstā atlasiet **Windows Update** un pēc tam atlasiet **Palaist problēmu risinātāju**.

1. Restartējiet datoru un pārbaudiet, vai problēma joprojām pastāv.

