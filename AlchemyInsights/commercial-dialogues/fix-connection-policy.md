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
ms.openlocfilehash: 7eae77358b0305582f53c411a092e3d2f1dbe17fd58ceac1ac00d5c07b3dd202
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988121"
---
# <a name="fix-connection-policy"></a>Labot savienojuma politiku

E-pasta ziņojums tika atzīmēts kā drošs un piegādāts lietotāja iesūtnē, jo sūtīšanas IP adrese savienojuma filtra politikā bija atzīmēta kā droša. Lai pārskatītu politiku, rīkojieties šādi:

1. Dodieties [uz Office 365 drošības & centru](https://go.microsoft.com/fwlink/p/?linkid=2077143)un pēc tam dodieties uz sadaļu Apdraudējumu **pārvaldības**  >  **politikas**  >  [pretsurogātpasta politika](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Cilnē **Pielāgota** atlasiet savienojuma filtra **politiku un pēc** tam atlasiet Rediģēt **politiku**.
3. Pārskatiet **atļauto IP adrešu** sarakstu. Pārbaudiet, **Seifs ir iespējots** šis saraksts.

    > [!NOTE]
    > Microsoft abonē uzticamu sūtītāju trešo pušu avotus. Ja **Seifs saraksts** ir iespējots, šie uzticamie sūtītāji netiek kļūdas dēļ atzīmēti kā surogātpasts. Es iesaku atlasīt šo opciju, jo šādi tiks samazināts aplami pozitīvo ziņojumu skaits (labie e-pasta ziņojumi, kas tiek klasificēti kā surogātpasts).
