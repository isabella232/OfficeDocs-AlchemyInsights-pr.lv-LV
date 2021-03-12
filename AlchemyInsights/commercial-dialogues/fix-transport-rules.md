---
title: Transporta kārtulu labošana
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
ms.openlocfilehash: 635009ed4b78d2b05b0eef1f3298765b10f86ede
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746734"
---
# <a name="fix-transport-rules"></a>Transporta kārtulu labošana

Šis ziņojums ietekmēja pielāgotu pasta plūsmas kārtulu. Lai pārskatītu precīzu kārtulu, veiciet tālāk norādītās darbības.

1. Iesniegšanas rezultātu sadaļā **Papildinformācija** pievērsiet uzmanību **GUID** vai **politikas nosaukumam**.
2. Palaidiet Exchange pārvaldības čaulu. Papildinformāciju skatiet rakstā [Exchange pārvaldības čaulas atvēršana](https://go.microsoft.com/fwlink/?linkid=2101432).
3. Izpildīt šo komandu (izmantojot jūsu iesniegto GUID):  **Get-TransportRule-Identity "GUID" | FL * apraksts***
4. Pārskatiet aprakstu, lai redzētu konfigurētos nosacījumus, kas ietekmēja ziņojumu.

Papildinformāciju skatiet rakstā [Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
