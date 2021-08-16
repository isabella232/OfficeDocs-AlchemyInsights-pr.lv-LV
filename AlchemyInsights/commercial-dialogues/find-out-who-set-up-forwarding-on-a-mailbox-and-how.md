---
title: Uzziniet, kuri lietotāju iestatīšanas pastkastē un kā
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 6243e787bb6b51f26cf22782d9ec80f946430b864f53de7ea626b7166a674d2c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53988212"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Uzziniet, kuri lietotāju iestatīšanas pastkastē un kā

Ja pastkastē tika iestatīta ārējā pārsūtīšana, darbība tiek auditēta kā daļa no Set-Mailbox cmdlet. Tālāk ir aprakstīts, kā atrast darbību audita žurnālā.

1. Dodieties [uz Office 365 drošības & centru](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Atlasiet **Meklēt** >  **audita žurnāla meklēšanā**.
    > [!NOTE]
    > Ja redzat paziņojumu, ka ir jāieslēdz auditēšana, turpiniet un ieslēdziet to. Ja šis līdzeklis nav ieslēgts, meklēšanas rezultāti nevarēs izvilkt datus no iepriekšējiem datumiem.
1. Pārliecinieties, **vai laukam** Darbības ir **iestatīta vērtība Rādīt visu darbību rezultātus** (noklusējums). Norādiet datumu diapazonu. Lietotājvārds nav jānorāda.
1. Atlasiet **Meklēt**. Darbības tiek rādītas sadaļā **Rezultāti.**
1. Atlasiet **Filtrēt rezultātus** un pēc tam laukā Darbības filtrs **ievadiet** **Set-mailbox.** Tādējādi tiek atgrieztas visas **set-mailbox** darbības.
1. Lai skatītu detalizēto informāciju, atlasiet darbību un pēc tam atlasiet **Papildinformācija**. Sadaļā **Parametri** varat skatīt pastkastē iestatīto pārsūtīšanas e-pasta adresi. **UserID apzīmē** lietotāju, kurš iestata ārējo pārsūtīšanu pastkastē.
Papildinformāciju skatiet rakstā [Meklēšana audita Office 365, lai novērstu izplatītus scenārijus.](https://go.microsoft.com/fwlink/?linkid=2103944)