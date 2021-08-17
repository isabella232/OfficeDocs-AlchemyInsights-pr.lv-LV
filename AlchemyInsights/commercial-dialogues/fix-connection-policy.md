---
title: Labot savienojuma politiku
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
ms.openlocfilehash: d27d570a7bc0f2c1081ba7fd52264a20bf25a453
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58314851"
---
# <a name="fix-connection-policy"></a>Labot savienojuma politiku

E-pasta ziņojums tika atzīmēts kā drošs un piegādāts lietotāja iesūtnē, jo avota IP adrese noklusējuma savienojuma filtra politikā tika atzīmēta kā droša. Lai pārskatītu politiku, veiciet šādas darbības:

1. Vietnes Microsoft 365 Defender dodieties uz Sadaļu <https://security.microsoft.com/>  \>  \>  \> **E-&**  un sadarbības politikas & Kārtulu pretsurogātpasta politikas sadaļā Politikas.

   Lai pārietu tieši uz **lapu Pretsurogātpasta** politikas, izmantojiet <https://security.microsoft.com/antispam> .

2. Lapā **Pretsurogātpasta** politikas atlasiet politiku ar nosaukumu Savienojuma filtra politika (noklusējums), noklikšķinot uz politikas nosaukuma. 

3. Parādītā detalizētas informācijas izlidošanas logā noklikšķiniet uz Rediģēt **savienojuma** filtra politiku **sadaļā Savienojuma filtrēšana.**

4. Pārskatiet ierakstus sadaļā Vienmēr **atļaut ziņojumus no** šādām IP adresēm vai adrešu diapazoniem un skatiet, vai ir atlasīta opcija Ieslēgt **drošo** sarakstu.

   **Piezīme.** Microsoft abonē uzticamu sūtītāju trešo pušu avotus. Ja drošais saraksts ir iespējots, šie uzticamie sūtītāji netiek kļūdas dēļ atzīmēti kā surogātpasts. Mēs iesakām atlasīt šo opciju, jo tādējādi tiks samazināts aplami pozitīvo ziņojumu skaits (labie e-pasta ziņojumi, kas tiek klasificēti kā surogātpasts).

Papildinformāciju skatiet rakstā [Savienojumu filtrēšanas konfigurēšana.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
