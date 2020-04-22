---
title: Nosakiet ārējo e-pasta pārsūtīšanu pastkastēm audita žurnālos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 156fd0044cdc42230ace0a5db16f49af572bb6fa
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716467"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Noteikt, kad ārējā e-pasta pārsūtīšana ir konfigurēta pastkastēm

Ja Microsoft 365 lietotājs konfigurē ārēju e-pasta ziņojumu pārsūtīšanu pastkastē, darbība tiek auditēta kā daļa no **Set-Mailbox** cmdlet. Darbību var skatīt, izmantojot audita žurnāla meklēšanu drošības & atbilstības centrā.

1. Piesakieties [Microsoft 365 drošības & atbilstības centrā](https://protection.office.com/).

2. Pārejiet **uz** > meklēšanas**audita žurnāla meklēšanas** lapu.

3. Laukā **sākuma datums** un **beigu datums** atlasiet datumu diapazonu. Jums nav nepieciešams norādīt lietotājvārdu. Pārbaudiet, vai lauks **darbības** ir iestatīts, lai **rādītu visu aktivitāšu rezultātus**.

4. Noklikšķiniet uz **Meklēt**.

Rezultātos noklikšķiniet uz **filtrēt rezultātus** un tips **Set-pastkaste** lodziņā darbības filtrs. Atlasiet audita ierakstu rezultātos. **Detalizētās** informācijas izlidošanas noklikšķiniet uz **Papildinformācija**. Jums ir aplūkot detalizētu informāciju par katru audita ierakstu, lai noteiktu, vai darbība ir saistīta ar e-pasta pārsūtīšanu.

- **ObjectId**: modificētās pastkastes aizstājvārda vērtība.

- **Parametri**: _ekspdingsmtpaddress_ norāda mērķa e-pasta adresi.

- **USERID**: lietotājs, kurš konfigurējis e-pasta pārsūtīšanu uz pastkasti laukā **ObjectId** .

Lai iegūtu papildinformāciju, skatiet [noteikt, kurš ir iestatījis e-pasta pārsūtīšanu pastkastei](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-who-set-up-email-forwarding-for-a-mailbox).
