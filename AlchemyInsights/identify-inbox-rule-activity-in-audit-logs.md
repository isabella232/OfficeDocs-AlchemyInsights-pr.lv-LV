---
title: Iesūtnes kārtulas darbību identificēšana audita žurnālos
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
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 1f252836d624b4550e1f3c87cf4fd7309dec6e91
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58331130"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a>Iesūtnes kārtulas darbību identificēšana audita žurnālos

Audita žurnāla meklēšanu šajā mapē varat izmantot, Microsoft 365 atbilstības centrs skatītu iesūtnes kārtulu notikumus (izveidi, modificēšanu un dzēšanu iesūtnes kārtulas).

1. Veiciet vienu no šīm darbībām:
   - Lapā Microsoft 365 atbilstības centrs <https://compliance.microsoft.com> uz **Solutions** \> **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://compliance.microsoft.com/auditlogsearch> .
   - Vietnes Microsoft 365 Defender dodieties <https://security.microsoft.com> uz **Audit**. Vai arī, lai pārietu tieši uz **lapu Audits,** izmantojiet <https://security.microsoft.com/auditlogsearch> .

2. Audita  lapas cilnē **Meklēšana** konfigurējiet tālāk norādītos iestatījumus.
   - **Datuma un laika diapazons:** atlasiet datuma/laika diapazonu lodziņā **Sākums** **un** Beigas.
   - **Darbības:** atlasiet vienu vai vairākas no šīm vērtībām:
     - **Jauna-iesūtnes Kārtula Iesūtnes kārtulas izveide no Outlook Web App**
     - **Iestatīt iesūtni. Kārtulas modificēšana no Outlook Web App**.
     - **Iesūtnes kārtulu atjaunināšana no Outlook klienta**

3. Kad esat pabeidzis, noklikšķiniet uz **Meklēt.** Darbības tiek rādītas jaunajā **lapā Meklēšana audita** meklēšanā.

4. Atlasiet darbību rezultātos, lai atvērtu detalizētas informācijas izlidošanu. Laukā Parametri tiek parādīta informācija par iesūtnes **kārtulas** iestatījumiem.

Papildinformāciju skatiet rakstā [Noteikšana, vai lietotājs ir izveidojis iesūtnes kārtulu.](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-created-an-inbox-rule)
