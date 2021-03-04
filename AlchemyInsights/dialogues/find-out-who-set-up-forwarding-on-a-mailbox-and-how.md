---
title: Noskaidrojiet, kurš iestatīja pārsūtīšanu pastkastē un kā
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
ms.openlocfilehash: 6a1a1376758024339939d10a7d17520faa8505ea
ms.sourcegitcommit: f4ba304b92ed01e35273ecda67e9dc3ad9d475c1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50429987"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Noskaidrojiet, kurš iestatīja pārsūtīšanu pastkastē un kā

Ja uz pastkastes ir iestatīta ārējā pārsūtīšana, aktivitāte tiek auditēta kā daļa no Set-Mailbox cmdlet. Tālāk ir aprakstīts, kā atrast aktivitāti audita žurnālfailā.

1. Dodieties uz [Office 365 drošības & atbilstības centru](https://go.microsoft.com/fwlink/p/?linkid=2077143).
1. Atlasiet **meklēšanas** >  **audita žurnālu meklēšana**.
    > [!NOTE]
    > Ja redzat paziņojumu par to, ka ir jāieslēdz auditēšana, pārejiet uz priekšu un ieslēdziet to tūlīt. Ja šis līdzeklis nav ieslēgts, meklēšanas rezultātos nevarēs paņemt datus no iepriekšējiem datumiem.
1. Pārliecinieties, vai lauks **aktivitātes** ir iestatīts uz **Rādīt rezultātus visās aktivitātēs** (noklusējums). Norādiet datumu diapazonu. Nav jānorāda lietotājvārds.
1. Atlasiet **Meklēt**. Darbības būs redzamas sadaļā **rezultāti**.
1. Atlasiet **filtra rezultāti** un pēc tam laukā **darbību** filtrs ievadiet **Set-pastkaste** . Tas atgriež visas **iestatītās pastkastes** darbības.
1. Lai skatītu detalizētu informāciju, atlasiet aktivitāti un pēc tam atlasiet **Papildinformācija**. Sadaļā **Parametri** varat redzēt pāradresēšanas e-pasta adresi, kas tika iestatīta pastkastē. Lietotāja **ID** norāda lietotāju, kurš ir iestatījis ārējo pārsūtīšanu pastkastē.
Lai uzzinātu vairāk, skatiet rakstu [meklēšana Office 365 audita žurnālu, lai novērstu raksturīgākos scenārijus](https://go.microsoft.com/fwlink/?linkid=2103944).