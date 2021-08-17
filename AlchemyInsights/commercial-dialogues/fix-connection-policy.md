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
ms.openlocfilehash: 9094dcdc4507f52da1dd7c95f83aa98bab1446639d2d9f52eb3a7bc849dc183c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57888413"
---
# <a name="fix-connection-policy"></a>Labot savienojuma politiku

E-pasta ziņojums tika atzīmēts kā drošs un piegādāts lietotāja iesūtnē, jo avota IP adrese noklusējuma savienojuma filtra politikā tika atzīmēta kā droša. Lai pārskatītu politiku, veiciet šādas darbības:

1. Vietnes Microsoft 365 Defender dodieties uz <https://security.microsoft.com/>  \>  \>  \> **E-&**  un sadarbības politikas & Kārtulu pretsurogātpasta politikas sadaļā Politikas.

   Lai pārietu tieši uz **lapu Pretsurogātpasta** politikas, izmantojiet <https://security.microsoft.com/antispam> .

2. Lapā **Pretsurogātpasta** politikas atlasiet politiku ar nosaukumu Savienojuma filtra politika (noklusējums), noklikšķinot uz politikas nosaukuma. 

3. Parādītā detalizētas informācijas izlidošanas logā noklikšķiniet uz Rediģēt **savienojuma** filtra politiku **sadaļā Savienojuma filtrēšana.**

4. Pārskatiet ierakstus sadaļā Vienmēr **atļaut ziņojumus no** šādām IP adresēm vai adrešu diapazoniem un skatiet, vai ir atlasīta opcija Ieslēgt **drošo** sarakstu.

   > [!NOTE]
   > Microsoft abonē uzticamu sūtītāju trešo pušu avotus. Ja drošais saraksts ir iespējots, šie uzticamie sūtītāji netiek kļūdas dēļ atzīmēti kā surogātpasts. Mēs iesakām atlasīt šo opciju, jo tādējādi tiks samazināts aplami pozitīvo ziņojumu skaits (labie e-pasta ziņojumi, kas tiek klasificēti kā surogātpasts).

Papildinformāciju skatiet rakstā [Savienojumu filtrēšanas konfigurēšana.](https://docs.microsoft.com/microsoft-365/security/office-365-security/configure-the-connection-filter-policy)
