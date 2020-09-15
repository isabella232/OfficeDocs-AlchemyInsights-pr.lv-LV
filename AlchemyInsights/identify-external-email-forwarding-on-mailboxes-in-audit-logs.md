---
title: Ārējo e-pasta pārsūtīšanas noteikšana uz pastkastēm audita žurnālos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1369"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: d06ef83adcae1342173a6fe75f79525c7e1797ce
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696304"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>E-pasta pārsūtīšanas noteikšana pastkastēs

Ja Microsoft 365 lietotājs konfigurē ārējo e-pasta pārsūtīšanu pastkastē, darbība tiek auditēta kā daļa no **Set-Mailbox** cmdlet. Varat skatīt aktivitāti, izmantojot audita žurnālu meklēšanu drošības & atbilstības centrā.

1. Piesakieties [Microsoft 365 drošības & atbilstības centrā](https://protection.office.com/).

2. Dodieties **uz meklēšanas**  >  **audita žurnālu meklēšanas** lapā.

3. Atlasiet datumu diapazonu lauku **sākuma datums** un **beigšanas datums** . Nav jānorāda lietotājvārds. Pārbaudiet, vai lauks **aktivitātes** ir iestatīts uz **Rādīt rezultātus visās aktivitātēs**.

4. Noklikšķiniet uz **Meklēt**.

Rezultātos noklikšķiniet uz **filtrēt rezultātus** un ierakstiet **Set-pastkaste** lodziņā darbību filtrs. Rezultātos atlasiet audita ierakstu. **Detalizētas** informācijas izlidošanas sarakstā noklikšķiniet uz **Papildinformācija**. Jums ir jāaplūko detalizēta informācija par katru audita ierakstu, lai noteiktu, vai darbība ir saistīta ar e-pasta pārsūtīšanu.

- **ObjectId**: modificētās pastkastes aizstājvārda vērtība.

- **Parametri**: _ForwardingSmtpAddress_ norāda e-pasta adresi.

- Lietotāja **ID**: lietotājs, kurš ir konfigurējis e-pasta pārsūtīšanu pastkastē **ObjectId** laukā.

Papildinformāciju skatiet rakstā [e-pasta pārsūtīšanas iestatīšana pastkastei](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox).
