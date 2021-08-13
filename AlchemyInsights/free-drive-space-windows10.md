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
ms.openlocfilehash: c7d29ab718be8dbdcde61a7de2f158fb3bbd722d2964d8b13cde9936dd1e5ee1
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53928088"
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

