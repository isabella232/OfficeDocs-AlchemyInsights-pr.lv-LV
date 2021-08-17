---
title: Iesūtnes kārtulās veikto notikumu atrašana
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
ms.openlocfilehash: d6a4eadd897dfae3b65ccda6363edfe9cef1c810
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58313506"
---
# <a name="find-events-performed-on-inbox-rules"></a>Iesūtnes kārtulās veikto notikumu atrašana

Kad iesūtnes kārtulas tiek izveidotas, mainītas vai izdzēstas, notikumi tiek ierakstīti audita žurnālā. Lūk, kā tās pārskatīt:

1. Veiciet kādu no šīm darbībām:
   - Lapā Microsoft 365 atbilstības centrs <https://compliance.microsoft.com> uz **Solutions** \> **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://compliance.microsoft.com/auditlogsearch> .
   - Vietnes Microsoft 365 Defender dodieties <https://security.microsoft.com> uz **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://security.microsoft.com/auditlogsearch> .

    **Piezīme.** Ja redzat paziņojumu, ka ir jāieslēdz auditēšana, turpiniet un ieslēdziet to. Ja šis līdzeklis nav ieslēgts, meklēšanas rezultāti nevarēs izvilkt datus no iepriekšējiem datumiem.
1. Atlasiet lauku Darbības, atrodiet vienumu Exchange darbības un pēc tam atlasiet New-InboxRule Izveidot iesūtnes kārtulu no Outlook Web App. Kad esat beidzis darbu, noklikšķiniet ārpus rūts, lai minimizētu rūti Darbības.
1. Norādiet datumu diapazonu un pēc tam laukā Lietotāji atlasiet tā lietotāja lietotājvārdu, kuru vēlaties izpētīt. Vienlaikus varat atlasīt vairākus lietotājus.
1. Atlasiet Meklēt. Darbības tiek rādītas sadaļā Rezultāti.
1. Lai skatītu detalizētu informāciju, atlasiet darbību un pēc tam atlasiet Papildinformācija. Sadaļā Parametri varat skatīt kārtulas nosaukumu, iestatītos nosacījumus un darbības, kuras veiks kārtula.

2. Audita  lapas cilnē **Meklēšana** konfigurējiet tālāk norādītos iestatījumus.
   - **Datuma un laika diapazons:** atlasiet datuma/laika diapazonu lodziņā **Sākums** **un** Beigas.
   - **Darbības:** jaunas **iesūtnes atlaseSakurses kārtulas izveide no Outlook Web App**

3. Kad esat pabeidzis, noklikšķiniet uz **Meklēt.** Darbības tiek rādītas jaunajā **lapā Meklēšana audita** meklēšanā.

4. Atlasiet darbību rezultātos, lai atvērtu detalizētas informācijas izlidošanu. Sadaļā **Parametri** varat skatīt kārtulas nosaukumu, iestatītos nosacījumus un darbības, kuras veiks kārtula.

Papildinformāciju skatiet rakstā [Meklēšana audita žurnālā, lai izpētītu bieži sastopamas atbalsta problēmas.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios)
