---
title: Izdzēsto notikumu audita žurnālu lasīšana
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
ms.openlocfilehash: ec8f845f599e397814bc9077c3fe59edb5324192
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58324740"
---
# <a name="read-the-audit-logs-for-deleted-events"></a>Izdzēsto notikumu audita žurnālu lasīšana

Lūk, kā to paveikt:

1. Veiciet kādu no šīm darbībām:
   - Lapā Microsoft 365 atbilstības centrs <https://compliance.microsoft.com> dodieties uz **Risinājumu** \> **audits**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://compliance.microsoft.com/auditlogsearch> .
   - Vietnes Microsoft 365 Defender dodieties <https://security.microsoft.com> uz **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://security.microsoft.com/auditlogsearch> .

    **Piezīme.** Ja redzat paziņojumu, ka līdzeklis ir jāieslēdz, turpiniet un ieslēdziet to. Ja līdzeklis nav ieslēgts, meklēšanas rezultāti nevarēs izvilkt datus no iepriekšējiem datumiem.

2. Audita  lapas cilnē **Meklēšana** konfigurējiet tālāk norādītos iestatījumus.
   - **Datuma un laika diapazons:** atlasiet datuma/laika diapazonu lodziņā **Sākums** **un** Beigas.
   - **Darbības**. **Ievadiet Exchange pastkastes darbības** un pēc tam atlasiet tālāk norādītās vērtības.
     - **Izdzēsti ziņojumi no mapes Izdzēstie vienumi**
     - **Pārvietoti ziņojumi uz mapi Izdzēstie vienumi**

       Kad esat beidzis darbu, noklikšķiniet ārpus rūts, lai minimizētu **rūti** Darbības.

   - **Lietotāji:** akceptējiet tukšo noklusējuma vērtību, lai atgrieztu rezultātus visiem lietotājiem, vai ievadiet vienu vai vairākus lietotājus.

3. Kad esat pabeidzis, noklikšķiniet uz **Meklēt.** Darbības tiek rādītas jaunajā **lapā Meklēšana audita** meklēšanā.

4. Atlasiet darbību rezultātos, lai atvērtu detalizētas informācijas izlidošanu. Laukā **AffectedItems** tiek rādīta papildinformācija par izdzēsto vienumu, piemēram, tēmas rindiņa un vienuma dzēšanas vieta.

   **Piezīme.** Izdzēstos vienumus nevar atjaunot, izmantojot audita žurnāla līdzekli. Informāciju par izdzēsto vienumu atjaunošanu skatiet [rakstā Izdzēsto e-pasta ziņojumu atkopšana Outlook tīmeklī.](https://support.microsoft.com/office/recover-deleted-email-messages-in-outlook-on-the-web-a8ca78ac-4721-4066-95dd-571842e9fb11)

Papildinformāciju skatiet rakstā [Meklēšana audita žurnālā, lai izpētītu bieži sastopamas atbalsta problēmas.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
