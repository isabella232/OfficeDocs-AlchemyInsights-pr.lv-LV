---
title: Dynamics 365 — nepareizs informācijas panelis tiek rādīts Dynamics 365 vienotajā interfeisā
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
ms.openlocfilehash: 02e33c7dbdfe9b7d2ad7a04f154cf067fba0aab2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47711282"
---
# <a name="wrong-dashboard-shows-in-dynamics-365-unified-interface"></a>Nepareizs informācijas panelis tiek rādīts Dynamics 365 vienotajā interfeisā

Pastāv vairāki iemesli, kāpēc, iespējams, redzēsit citu informācijas paneli, nevis vēlamo.

## <a name="the-user-has-set-a-user-default-dashboard"></a>Lietotājs ir iestatījis lietotāja noklusējuma informācijas paneli 

Parasti varat noteikt, ka lietotāja noklusējuma informācijas panelis ir iestatīts, ja nav redzama poga **Iestatīt kā noklusējumu** informācijas paneļa komandjoslā. Lietotāja noklusējuma informācijas panelī tiek ignorēti visi pārējie noklusējuma informācijas paneļi pat tad, ja lietotāja noklusējuma informācijas panelis nav pašreizējā lietojumprogrammā.

Izmantojiet tālāk norādītos risinājumus, lai atiestatītu noklusējuma informācijas paneli.

1. Izveidojiet jaunu personisko informācijas paneli.

2. Iestatiet šo jauno informācijas paneli kā lietotāja noklusējumu.

3. Dzēst šo informācijas paneli

## <a name="the-dashboard-is-set-in-the-sitemap"></a>Informācijas panelis ir iestatīts vietnes kartē

Iespējams, esat iestatījis organizācijas noklusējuma informācijas paneli, atlasot informācijas paneli un izvēloties "iestatīt kā noklusējumu" sadaļā sistēmas pielāgošana. Taču vietnes kartes noformētājā noteiktais informācijas panelis dominēs pār šo informācijas paneli, ja lietotājam tam ir piekļuve.

Lai lietotāji redzētu informācijas paneļa, ko esat iestatījis kā organizācijas noklusējumu, varat veikt kādu no tālāk norādītajām darbībām.

* Informācijas paneļa iestatīšana vietnes kartē

* Noņemt piekļuvi vietnes kartes definētam informācijas panelim šiem lietotājiem
