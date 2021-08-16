---
title: Ārējo e-pasta pārsūtīšanas pastkastēs identificēšana audita žurnālos
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
ms.openlocfilehash: 1e80917a323128ba23175651cdf4d892d7815a89c1223b654812c1b456c787da
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028751"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Noteikt, kad pastkastēs ir konfigurēta ārējā e-pasta pārsūtīšana

Kad lietotājs Microsoft 365 konfigurē pastkastē ārējo e-pasta pārsūtīšanu, darbība tiek auditēta kā daļa no **Set-Mailbox** cmdlet. Darbības var skatīt, izmantojot meklēšanu audita žurnālā drošības & centrā.

1. Piesakieties [Microsoft 365 atbilstības centrā](https://protection.office.com/).

2. Dodieties uz **meklēšanas**  >  **audita žurnāla meklēšanas** lapu.

3. Atlasiet datumu diapazonu laukos **Sākuma datums** **un Beigu** datums. Lietotājvārds nav jānorāda. Pārbaudiet, **vai laukam** Darbības ir iestatīta **vērtība Rādīt visu darbību rezultātus.**

4. Noklikšķiniet **uz Meklēt.**

Rezultātos noklikšķiniet uz **Filtrēt rezultātus** un darbību filtra lodziņā ierakstiet **Set-Mailbox.** Rezultātos atlasiet audita ierakstu. **Izlidošanas lodziņā** Detalizēta informācija noklikšķiniet uz **Papildinformācija.** Lai noteiktu, vai darbība ir saistīta ar e-pasta pārsūtīšanu, ir meklējiet detalizētu informāciju par katru audita ierakstu.

- **ObjectId:** modificētās pastkastes aizstājvārda vērtība.

- **Parametri:** _ForwardingSmtpAddress norāda_ mērķa e-pasta adresi.

- **UserId:** lietotājs, kurš konfigurēja e-pasta pārsūtīšanu pastkastē **laukā ObjectId.**

Papildinformāciju skatiet rakstā [Noteikšana, kurš iestatījis e-pasta pārsūtīšanu pastkastei.](/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
