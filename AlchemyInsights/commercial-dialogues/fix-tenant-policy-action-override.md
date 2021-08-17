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
ms.openlocfilehash: 157baa1f1e3f48b47ba07b8c6d446f8e081a4ad24b7d48f50c4fc5af5518cdd6
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57896082"
---
# <a name="fix-tenant-policy-action-override"></a>Nomnieka politikas labošana (darbības ignorēšana)

Kāda no jūsu pretsurogātpasta politikām ir ietekmējusi šo ziņojumu. Lai pārskatītu politikas, veiciet tālāk norādītās darbības.

1. Vietnes Microsoft 365 Defender dodieties uz <https://security.microsoft.com/>  \>  \>  \> **E-&**  un sadarbības politikas & Kārtulu pretsurogātpasta politikas sadaļā Politikas.

   Lai pārietu tieši uz **lapu Pretsurogātpasta** politikas, izmantojiet <https://security.microsoft.com/antispam> .

2. Lapā **Pretsurogātpasta** politikas atlasiet politiku, noklikšķinot uz politikas  nosaukuma **(Tips**  ir pielāgota pretsurogātpasta politika vai Nosaukums ir surogātpasta novēršanas politika **(noklusējums)**).
3. Parādītā detalizētas informācijas izlidošanas logā sadaļā **Darbības** **atlasiet Rediģēt** darbības.
4. Sadaļā Ziņojuma darbības **pārskatiet** surogātpasta **parametrus,** augstas kvalitātes surogātpastu, pikšķerēšanu un augstas uzticēšanās pikšķerēšanu, lai redzētu, vai ir atlasīta kāda no šīm vērtībām: 
   - **Pievienot galveni X**
   - **Tēmas rindiņas pievienošana tekstam**
   - **Novirzīt ziņojumu uz e-pasta adresi**
   - **Ziņojuma dzēšana**
   - **Nav darbību**

   Iespējams, ka standarta iestatījumi tiek **lietoti** visiem klientiem, Exchange Online Protection ietekmēti ar šo ziņojumu.

Papildinformāciju skatiet rakstā [Surogātpasta novēršanas politiku konfigurēšana rīkkopā EOP.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-your-spam-filter-policies)
