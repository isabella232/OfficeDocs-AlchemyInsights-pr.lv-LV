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
ms.openlocfilehash: 7746e44a0ee5a4442051900985aab339b09652f08e412b02a02429c93cc7c107
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895186"
---
# <a name="find-out-who-set-up-forwarding-on-a-mailbox-and-how"></a>Uzziniet, kuri lietotāju iestatīšanas pastkastē un kā

Ja pastkastē tika iestatīta ārējā pārsūtīšana, darbība tiek auditēta kā daļa no **Set-Mailbox** cmdlet. Tālāk ir aprakstīts, kā atrast darbību audita žurnālā.

1. Veiciet kādu no šīm darbībām:
   - Lapā Microsoft 365 atbilstības centrs <https://compliance.microsoft.com> uz **Solutions** \> **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://compliance.microsoft.com/auditlogsearch> .
   - Vietnes Microsoft 365 Defender dodieties <https://security.microsoft.com> uz **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://security.microsoft.com/auditlogsearch> .

   > [!NOTE]
   > Ja redzat paziņojumu, ka ir jāieslēdz auditēšana, turpiniet un ieslēdziet to. Ja šis līdzeklis nav ieslēgts, meklēšanas rezultāti nevarēs izvilkt datus no iepriekšējiem datumiem.

2. Lapā **Audits** pārbaudiet, vai ir atlasīta **cilne** Meklēšana, un pēc tam konfigurējiet šos iestatījumus:
   - Atlasiet datuma/laika diapazonu lodziņā **Sākums** **un** Beigas.
   - Pārbaudiet, **vai lodziņā** Darbības ir iekļauti rādīt rezultātus par visām **darbībām.**

3. Kad esat pabeidzis, noklikšķiniet uz **Meklēt.** Darbības tiek rādītas jaunajā **lapā Meklēšana audita** meklēšanā.

4. Rezultātos noklikšķiniet uz kolonnas **Darbības,** lai kārtotu rezultātus, un meklējiet **ierakstus Set-Mailbox.**

5. Atlasiet darbību rezultātos, lai atvērtu detalizētas informācijas izlidošanu. Lai noteiktu, vai darbība ir saistīta ar e-pasta pārsūtīšanu, ir meklējiet detalizētu informāciju par katru audita ierakstu.
   - **ObjectId:** modificētās pastkastes aizstājvārda vērtība.
   - **Parametri:** _ForwardingSmtpAddress norāda_ mērķa e-pasta adresi.
   - **UserId:** lietotājs, kurš konfigurēja e-pasta pārsūtīšanu pastkastē **laukā ObjectId.**

Papildinformāciju skatiet rakstā [Noteikšana, kurš iestatījis e-pasta pārsūtīšanu pastkastei.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-who-set-up-email-forwarding-for-a-mailbox)
