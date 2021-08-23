---
title: Brīdinājumi, kas trūkst cilnē Brīdinājumi
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 8/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9007647"
- "12732"
ms.openlocfilehash: 9fbd9a32e40d858f0ba49931c723a824478aaa12
ms.sourcegitcommit: 2be4a0352cb84a703ebf12966e1c17b64df07364
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/16/2021
ms.locfileid: "58454681"
---
# <a name="alerts-missing-from-alerts-tab"></a>Brīdinājumi, kas trūkst cilnē Brīdinājumi

Cilne Brīdinājumi darbojas, pamatojoties uz programmu pārvaldības portāla iestatīšanas un **aktivizēšanas** politikām jūsu nomniekā. Lai ļautu signālus plūst uz cilni Brīdinājumi, jāaktivizē arī programmu pārvaldības novīsto **politiku** iestatījumi. 

Apstipriniet, ka brīdinājums ir ģenerēts:

1. Dodieties uz programmu [pārvaldības politiku](https://compliance.microsoft.com/m365appprotection?viewid=policies) un apstipriniet, ka esat izveidojis vismaz vienu aktīvu vai audita politiku.

1. Atlasiet politiku un pēc tam atlasiet **Rediģēt** izlidošanas rūtī. 

1. Pārbaudiet politikas konfigurāciju, lai pārliecinātos, vai brīdinājumam jābūt ģenerētam, pamatojoties uz politikas notikumu, kas iniciēts vairāk nekā 24 stundas atpakaļ.

Papildinformāciju par brīdinājumiem lietojumprogrammu pārvaldībā skatiet [rakstā Darba sākšana ar programmu apdraudējumu noteikšanu un koriģēšanu.](https://docs.microsoft.com/microsoft-365/compliance/app-governance-detect-remediate-get-started)