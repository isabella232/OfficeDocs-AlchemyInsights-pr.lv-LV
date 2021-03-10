---
title: Savienojuma politikas labošana
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694169"
---
# <a name="fix-connection-policy"></a>Savienojuma politikas labošana

E-pasta ziņojums tika atzīmēts kā drošs un piegādāts lietotāja iesūtnei, jo sūtītāja IP adrese ir atzīmēta kā droša savienojuma filtra politikā. Lai pārskatītu politiku, veiciet tālāk norādītās darbības.

1. Dodieties uz [Office 365 drošības & atbilstības centru](https://go.microsoft.com/fwlink/p/?linkid=2077143)un pēc tam dodieties uz **Threat Management**  >  **Policy**  >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).
2. Cilnē **Pielāgota** atlasiet **savienojuma filtra politiku** un pēc tam atlasiet **Rediģēt politiku**.
3. Pārskatiet **IP atļauto** sarakstu. Pārbaudiet, vai ir iespējots **Drošais saraksts** .

    > [!NOTE]
    > Microsoft abonē trešo pušu uzticamo sūtītāju avotus. Ja **Drošais saraksts** ir iespējots, šie uzticamie sūtītāji nav kļūdaini atzīmēti kā mēstules. Iesakām atlasīt šo opciju, jo tādējādi tiks samazināts maldīgu pozitīvu darbību skaits (labs pasts, kas ir klasificēts kā surogātpasts), ko saņemat.
