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
ms.openlocfilehash: 48634fad8f573e3a7c38cac299bb95ec90814f5c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331166"
---
# <a name="identify-when-external-email-forwarding-is-configured-on-mailboxes"></a>Noteikt, kad pastkastēs ir konfigurēta ārējā e-pasta pārsūtīšana

Kad lietotājs Microsoft 365 konfigurē pastkastē ārējo e-pasta pārsūtīšanu, darbība tiek auditēta kā daļa no **Set-Mailbox** cmdlet. Varat skatīt darbību, izmantojot meklēšanu audita žurnālā. Tālāk ir aprakstīts, kā to izdarīt.

1. Veiciet vienu no šīm darbībām:
   - Lapā Microsoft 365 atbilstības centrs <https://compliance.microsoft.com> uz **Solutions** \> **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://compliance.microsoft.com/auditlogsearch> .
   - Vietnes Microsoft 365 Defender dodieties <https://security.microsoft.com> uz **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://sip.security.microsoft.com/auditlogsearch> .

2. Lapā **Audits** pārbaudiet, vai ir atlasīta **cilne** Meklēšana, un pēc tam konfigurējiet šos iestatījumus:
   - Atlasiet datuma/laika diapazonu lodziņā **Sākums** **un** Beigas.
   - Pārbaudiet, **vai lodziņā** Darbības ir iekļauti rādīt rezultātus par visām **darbībām.**

3. Kad esat pabeidzis, noklikšķiniet uz **Meklēt.** Darbības tiek rādītas jaunajā **lapā Meklēšana audita** meklēšanā.

4. Rezultātos noklikšķiniet uz **Filtrēt rezultātus** un darbību filtra lodziņā ierakstiet **Set-Mailbox.**

5. Rezultātos atlasiet audita ierakstu. **Izlidošanas lodziņā** Detalizēta informācija noklikšķiniet uz **Papildinformācija.** Jums ir meklējiet detalizētu informāciju par katru audita ierakstu, lai noteiktu, vai darbība ir saistīta ar e-pasta pārsūtīšanu.

   - **ObjectId:** modificētās pastkastes aizstājvārda vērtība.
   - **Parametri:** _ForwardingSmtpAddress norāda_ mērķa e-pasta adresi.
   - **UserId:** lietotājs, kurš konfigurēja e-pasta pārsūtīšanu pastkastē **laukā ObjectId.**

Papildinformāciju skatiet rakstā [Noteikšana, kas iestatīja e-pasta pārsūtīšanu pastkastei.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
