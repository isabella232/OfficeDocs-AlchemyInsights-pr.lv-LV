---
title: 1332 OWA - iesūtnes kārtula ir nav izpildes pastkastes
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 12/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1332"
- "3700002"
ms.assetid: 383d1c77-5e4b-4a69-92d6-c404d890b6b7
ms.openlocfilehash: 218a05a8d321b76dd07345ea48d6b3e158cc120e
ms.sourcegitcommit: 77f704672b7c7de541899e25c022ff10c111e304
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2019
ms.locfileid: "36204067"
---
# <a name="an-inbox-rule-doesnt-work-as-expected"></a>Iesūtnes kārtulas nedarbojas, kā paredzēts

Pārbaudiet šos iestatījumus:

- Ziņojums var būt novirzīts, pārsūtīt vai atbildētu automātiski, pamatojoties uz iesūtnes kārtulas tikai vienu reizi. Novirzot kārtulu (iesūtnes kārtulu vai pasta plūsmas kārtula, pazīstams arī kā transporta kārtulu) var ne vairāk kā desmit pāradresācijas adresātu pievienošana ziņojumam. Papildinformāciju skatiet šeit: [Journal, transporta un iesūtnes kārtulu robežas](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits).

- Iesūtnes kārtulas nedarbojas uz alternatīvo journaling pastkasti. Papildinformāciju par alternatīvo journaling pastkasti, skatiet [alternatīvo journaling pastkastes](https://docs.microsoft.com/Exchange/security-and-compliance/journaling/journaling#alternate-journaling-mailbox).

Lai novērstu šo problēmu, skatiet [KB 2829319](https://support.microsoft.com/kb/2829319).

Ja iepriekšējie jautājumi neatbilst, palaidiet iesūtnes kārtulu diagnostikas pārskata pirms jūs izskatīt šo problēmu ar Microsoft Support:

1. Atvērt šo pastkasti programmā Outlook Web un noklikšķiniet uz <img src='data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAABIAAAASCAMAAABhEH5lAAAA51BMVEX6+fj6+fDr+fjK+fj69LRxsuj6+cjY+fi/+fin3ev6+ddMk81HdK5AaatHLn/ntXTrsW5cRmLOk0pAND5KNCl1NCOi3fiGwvjJ3fDBz+F6teFgpdt6stX68c314syTucirtchum8bjz8BQh7/6+b47fbrKtapiian63aFDaaHJuZJiQo36woVabH7ZtHiOQnTHm2wlKmqriWF/cFzVnVTFjlSyeUkrNEmBLkWfaUGsaT67fTrj9Pi19PjO8fiv5vj69OFWm9Pt3aZ1Qo0lNHQ1P2iYTWGOQmHcpV5kRlqvc0mrbERpPzMoEeekAAAAxElEQVQY03WQ5w6CUAyFy3Jv3HsrICoKqLj3fP/nsTcNakjsn9t+bW/OKfyL6iTCc49e/ktuRs2WEhE1U/qgQQfEzGkNyxzVXLdw0ASW+a7BZp3HpJ+cpovUjcv6PYtvSmKj4/SswTMaBgg9FQF5axWysKoson4cGMYCvlEAQDwK7XkZwEVbRBpDPC46ygbAbPl31p4Wvd8nwiRCLnIArJb1ZBD7KFWMkdQLSUVIhowsGaIwzzVHikfVV8lzHPv3OGTfTd4gnRNqGdZ49AAAAABJRU5ErkJggg==' />
 **Iestatījumi** > **Outlook iestatījumu skatīšana** > **Mail** > **noteikumiem**.

2. Lapas apakšdaļā noklikšķiniet uz **Ja kārtulas nedarbojas klikšķi šeit diagnostikas atskaites ģenerēšanai**.
