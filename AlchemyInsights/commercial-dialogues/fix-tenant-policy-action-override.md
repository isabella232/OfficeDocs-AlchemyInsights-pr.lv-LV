---
title: Nomnieka politikas labošana (darbības ignorēšana)
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
ms.openlocfilehash: ee45e86a143719914f7a7917730d7e840e90625f
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326804"
---
# <a name="fix-tenant-policy-action-override"></a>Nomnieka politikas labošana (darbības ignorēšana)

Kāda no jūsu pretsurogātpasta politikām ir ietekmējusi šo ziņojumu. Lai pārskatītu politikas, veiciet tālāk norādītās darbības.

1. Vietnes Microsoft 365 Defender dodieties uz Sadaļu <https://security.microsoft.com/>  \>  \>  \> **E-&**  un sadarbības politikas & Kārtulu pretsurogātpasta politikas sadaļā Politikas.

   Lai pārietu tieši uz **lapu Pretsurogātpasta** politikas, izmantojiet <https://security.microsoft.com/antispam> .

2. Lapā **Pretsurogātpasta** politikas atlasiet politiku, noklikšķinot uz politikas  nosaukuma **(Tips**  ir pielāgota pretsurogātpasta politika vai Nosaukums ir surogātpasta novēršanas politika **(noklusējums)**).
3. Parādītā detalizētas informācijas izlidošanas logā sadaļā **Darbības** **atlasiet Rediģēt** darbības.
4. Sadaļā Ziņojuma darbības **pārskatiet** surogātpasta **parametrus,** augstas kvalitātes surogātpastu, pikšķerēšanu un augstas uzticēšanās pikšķerēšanu, lai redzētu, vai ir atlasīta kāda no šīm vērtībām: 
   - **Pievienot galveni X**
   - **Tēmas rindiņas pievienošana tekstam**
   - **Novirzīt ziņojumu uz e-pasta adresi**
   - **Ziņojuma dzēšana**
   - **Nav darbību**

   Iespējams, ka standarta iestatījumi **visiem klientiem** Exchange Online Protection ietekmēti.

Papildinformāciju skatiet rakstā [Surogātpasta novēršanas politiku konfigurēšana rīkkopā EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
