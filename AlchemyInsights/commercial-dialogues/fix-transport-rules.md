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
ms.openlocfilehash: d89283dec427ba3d4f55fc1f180efc13da16ae15c3d5a6c0c06a696faa6df7f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034761"
---
# <a name="fix-transport-rules"></a>Transporta kārtulu labošana

Pielāgotu pasta plūsmas kārtulu ietekmējusi šo ziņojumu. Lai pārskatītu precīzu kārtulu, rīkojieties šādi:

1. Iesniegšanas rezultātu sadaļā **Papildinformācija atzīmējiet** **GUID** vai politikas **nosaukumu**.
2. Palaidiet Exchange pārvaldības čaulu. Papildinformāciju skatiet rakstā [Pārvaldības čaulas Exchange atvēršana.](https://go.microsoft.com/fwlink/?linkid=2101432)
3. Izpildiet šo komandu (izmantojot savu iesniegto guid):  **Get-TransportRule -identity "GUID" | fl * Description***
4. Pārskatiet aprakstu, lai skatītu konfigurētos nosacījumus, kas ietekmēja ziņojumu.

Papildinformāciju skatiet [rakstā Get-TransportRule](https://go.microsoft.com/fwlink/?linkid=2101523).
