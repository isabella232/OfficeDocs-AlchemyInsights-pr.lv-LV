---
title: Ip adreses atrašana audita žurnālā
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
ms.openlocfilehash: 258e92368b8a33e8ea807f0cb9af90132c86ed5b
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58303584"
---
# <a name="find-the-ip-address-in-audit-log"></a>Ip adreses atrašana audita žurnālā

Audita žurnālos tiek rādīta IP adrese, kas atbilst lietotāja vai administratora veiktajai darbībai. Tiek reģistrēta arī klienta informācija. Lai noteiktu IP adresi, lūk, kā:

1. Veiciet kādu no šīm darbībām:
   - Lapā Microsoft 365 atbilstības centrs <https://compliance.microsoft.com> uz **Solutions** \> **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://compliance.microsoft.com/auditlogsearch> .
   - Vietnes Microsoft 365 Defender dodieties <https://security.microsoft.com> uz **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://security.microsoft.com/auditlogsearch> .

    **Piezīme.** Ja redzat paziņojumu, ka ir jāieslēdz auditēšana, turpiniet un ieslēdziet to. Ja šis līdzeklis nav iespējots, meklēšanas rezultāti nevarēs izvilkt datus no iepriekšējiem datumiem.

2. Lapā **Audits** pārbaudiet, vai ir atlasīta **cilne** Meklēšana, un pēc tam konfigurējiet šos iestatījumus:
   - **Datuma un laika diapazons:** atlasiet datuma/laika diapazonu lodziņā **Sākums** **un** Beigas.
   - **Darbības:** ja jūs interesē konkrēta darbība, atlasiet to sarakstā; pretējā gadījumā noklusējuma vērtība **Rādīt rezultātus visām darbībām** atgriež visas darbības tiks atgrieztas.. Ņemiet vērā, ka atlasei dažas darbības var nebūt pieejamas. tomēr šie audita vienumi tiks atgriezti, ja **būs atlasīts Rādīt rezultātus par visām** darbībām.
   - **Lietotāji:** akceptējiet tukšo noklusējuma vērtību, lai atgrieztu rezultātus visiem lietotājiem, vai ievadiet vienu vai vairākus lietotājus.

3. Kad esat pabeidzis, noklikšķiniet uz **Meklēt.** Darbības tiek rādītas jaunajā **lapā Meklēšana audita** meklēšanā.

4. Rezultātos noklikšķiniet uz **Filtrēt rezultātus** un darbību filtra lodziņā ierakstiet **Set-Mailbox.**

5. Atlasiet audita ierakstu rezultātos, lai atvērtu **detalizētas informācijas izlidošanas** logu.

Papildinformāciju skatiet rakstā [Meklēšana audita žurnālā, lai izpētītu bieži sastopamas atbalsta problēmas.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
