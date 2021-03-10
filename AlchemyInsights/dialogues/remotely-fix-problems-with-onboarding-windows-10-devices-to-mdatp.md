---
title: Attālas problēmu novēršana saistībā ar Windows 10 ierīcēm, izmantojot Microsoft Defender Advanced Threat Protection
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 5473d090f6d4680f9a62f34f943ac6cea53b2079
ms.sourcegitcommit: 4883f1f89d4c6ca23161e9a43ff206ad21d4f09b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693652"
---
# <a name="remotely-fix-problems-with-onboarding-windows-10-devices-to-microsoft-defender-advanced-threat-protection"></a>Attālas problēmu novēršana saistībā ar Windows 10 ierīcēm, izmantojot Microsoft Defender Advanced Threat Protection

Ja varat piekļūt attālajam datoram, veiciet tālāk norādītās darbības.

1. Lejupielādējiet [klientu savienojamības analīzes](https://go.microsoft.com/fwlink/?linkid=2143466) diagnostikas rīku.
2. Izvilkt un palaist MDATPAnalyzer. cmd.
3. Atrodiet diagnostikas žurnālu mapē MDATPClientAnalyzerResult, kas ir tajā pašā mapē, kurā tika lejupielādēts analīzes rīks.
4. Lai atrastu problēmas ar savienojamības vai interneta starpniekservera iestatījumiem, pārskatiet žurnālfailu MDATPClientAnalyzer.txt.

Lai uzzinātu vairāk, skatiet rakstu [problēmas ar borta datoriem](https://go.microsoft.com/fwlink/?linkid=2143634).
