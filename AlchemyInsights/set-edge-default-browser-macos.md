---
title: Microsoft Edge iestatīšana par noklusējuma pārlūkprogrammu macOS ierīcē
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
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491557"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a>Microsoft Edge iestatīšana par noklusējuma pārlūkprogrammu macOS ierīcē

Izmantojiet vienu no šīm divām metodēm, lai iestatītu Microsoft Edge kā noklusējuma pārlūkprogrammu.

1. metode. Mirgo ierīce ar macOS attēlu, kurā Microsoft Edge jau ir iestatīta kā noklusējuma pārlūkprogramma.

2. metode. Iestatiet politiku DefaultBrowserSettingEnabled, lai piedāvātu lietotājam iestatīt Microsoft Edge kā noklusējuma pārlūkprogrammu.

Jebkura no metodēm sniedz lietotājam iespēju mainīt noklusējuma pārlūkprogrammu. Šī iemesla dēļ mēs iesakām izvietot politiku DefaultBrowserSettingEnabled pat tad, ja izmantojat 1. metodi. Ja lietotājs maina noklusējuma pārlūkprogrammu pēc politikas izvietošanas, politika aicina lietotāju iestatīt noklusējuma pārlūkprogrammu atpakaļ uz Microsoft Edge.
