---
title: Labākās medību vaicājumu metodes lietošana
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
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746185"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a>Labākās medību vaicājumu metodes lietošana

Lai iegūtu rezultātus ātrāk un lai izvairītos no taimautiem, palaižot sarežģītus vaicājumus, lietojiet šīs paraugprakses:

- Mēģinot izveidot jaunus vaicājumus, vienmēr izmantojiet ierobežojumu, lai izvairītos no ļoti lielām rezultātu kopām. Izmantojiet arī, `count` lai veiktu sākotnējā rezultātu kopas lieluma novērtējumu.
- Vispirms izmantojiet laika filtrus. Ideāli ierobežojiet vaicājumus līdz septiņām dienām.
- Vaicājuma sākumā uzreiz pēc laika filtra pievienojiet filtrus, lai noņemtu lielāko daļu datu.
- Meklējot pilnas marķierierīces, izmantojiet `has` operatoru, nevis `contains` .
- Veiciet meklēšanu noteiktā kolonnā, nevis visās kolonnās.
- Savienojot tabulas, vispirms norādiet tabulu, kurā ir mazāk rindu.
- `project` tikai nepieciešamās tabulas no Savienotajām tabulām.

Lai uzzinātu vairāk, skatiet rakstu [papildu medību vaicājumu labākā prakse](https://go.microsoft.com/fwlink/?linkid=2144812).
