---
title: Dynamics 365-nepareiza informācijas paneļa parāda Dynamics 365 vienotā interfeisā
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 3d7258bdd7366f679b048e93926ab7dfe0b956d9
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "36528558"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Nepareizs informācijas panelis parāda Dynamics 365 vienotā interfeisā

Ir vairāki iemesli, kāpēc var tikt parādīts cits informācijas panelis, nekā paredzēts:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Lietotājs ir iestatījis lietotāja noklusējuma informācijas paneli 

Parasti var identificēt lietotāja noklusējuma informācijas paneli ir iestatīts, ja poga **Iestatīt kā noklusējumu** informācijas paneļa komandu joslā netiek rādīta. Lietotāja noklusējuma informācijas panelis ignorē visus pārējos noklusējuma informācijas paneļus, pat ja lietotāja noklusējuma informācijas panelis nav pašreizējā programmā.

Lai unset noklusējuma informācijas paneli, izmantojiet tālāk minēto metodi.

1. Izveidojiet jaunu personisko informācijas paneli.

2. Iestatiet jauno informācijas paneli kā lietotāja noklusējumu.

3. Dzēsiet šo informācijas paneli.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Informācijas panelis ir iestatīts vietnes kartē

Iespējams, esat iestatījis organizācijas noklusējuma informācijas paneli, atlasot informācijas paneli un izvēloties "iestatīt kā noklusējumu" sadaļā "sistēmas pielāgošana". Bet informācijas panelis noteikts sitemap dizainers būs priekšroka pār šo informācijas paneli, ja lietotājs var piekļūt.

Lai lietotāji redzētu informācijas paneli, kuru esat iestatījis kā organizācijas noklusējumu, varat:

* Iestatīt šo informācijas paneli vietnes kartē

* Noņemt piekļuvi vietnes karte definēts informācijas panelis tiem lietotājiem
