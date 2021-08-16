---
title: Dynamics 365 — Dynamics 365 vienotā interfeisā tiek rādīts nepareizs informācijas panelis
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1484"
- "6200024"
ms.openlocfilehash: 1edb2a7e9e0c270c7e98eb43d2f6514d70c39a19ea97d189322ca387b6842a18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54101489"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Dynamics 365 vienotā interfeisā tiek rādīts nepareizs informācijas panelis

Ir vairāki iemesli, kāpēc informācijas panelis atšķiras no gaidītā:

## <a name="the-user-has-set-a-user-default-dashboard"></a>Lietotājs ir iestatījis lietotāja noklusējuma informācijas paneli 

Parasti lietotāja noklusējuma informācijas panelis tiek iestatīts, ja informācijas paneļa **komandjoslā** nav redzama poga Iestatīt kā noklusējumu. Lietotāja noklusējuma informācijas panelis ignorēs visus pārējos noklusējuma informācijas paneļus, pat ja lietotāja noklusējuma informācijas panelis nav pašreizējā programmā.

Izmantojiet tālāk norādīto risinājumu, lai atceltu noklusējuma informācijas paneļa iestatījumu.

1. Izveidojiet jaunu personisko informācijas paneli.

2. Iestatiet šo jauno informācijas paneli kā lietotāja noklusējuma informācijas paneli.

3. Izdzēsiet šo informācijas paneli.

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Informācijas panelis ir iestatīts vietnes kartē

Iespējams, esat iestatījis organizācijas noklusējuma informācijas paneli, atlasot informācijas paneli un sadaļā "Pielāgot sistēmu" izvēloties Iestatīt kā noklusējumu. Taču vietnes kartes noformētājā definētajam informācijas panelim būs prioritāte attiecībā pret šo informācijas paneli, ja lietotājam ir piekļuve šim informācijas panelim.

Lai lietotāji redzētu informācijas paneli, ko esat iestatījis kā organizācijas noklusējumu, varat:

* Šī informācijas paneļa iestatīšana vietnes kartē

* Noņemt piekļuvi vietnes kartes definētam informācijas panelim šiem lietotājiem
