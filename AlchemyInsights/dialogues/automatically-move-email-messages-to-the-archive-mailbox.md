---
title: Automātiska e-pasta ziņojumu pārvietošana uz arhīva pastkasti
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100008"
- "7217"
ms.openlocfilehash: 14ded561ee2b3c244fadbdab42fd0e833a1c66d5
ms.sourcegitcommit: 7fa9bf6f9fc7438791aa9241a440e5be817d4401
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50527107"
---
# <a name="automatically-move-email-messages-to-the-archive-mailbox"></a>Automātiska e-pasta ziņojumu pārvietošana uz arhīva pastkasti

Tālāk ir aprakstīts, kā iestatīt politiku, lai automātiski pārvietotu lietotāja veco e-pasta ziņojumu uz arhīva pastkasti.

1. Dodieties uz [**drošības & atbilstības**](https://go.microsoft.com/fwlink/p/?linkid=2077143)  >  **datu pārvaldības**  >  **arhīvu** , lai pārbaudītu, vai ir iespējota arhīva pastkaste lietotājam. Ja tā nav, brīdinājuma lodziņā noklikšķiniet uz **Iespējot** un pēc tam uz **Jā** .
2. Dodieties uz [**Exchange administrēšanas centrs > atbilstības pārvaldības > saglabāšanas atzīmes**](https://go.microsoft.com/fwlink/?linkid=2059104).
3. Izvēlieties ikonu +, pēc tam izvēlieties **automātiski lietot visai pastkastei**.
4. Piešķiriet nosaukumu saglabāšanas frāzei un izvēlieties **Pārvietot uz arhīvu**. Saglabāšanas periodam ievadiet vēlamo laiku, piemēram, 90 dienas. Noklikšķiniet uz **Saglabāt**.
5. Tagad izveidojiet saglabāšanas politiku: izvēlieties **saglabāšanas** politikas, izvēlieties ikonu, lai pievienotu jaunu politiku.
6. Piešķiriet nosaukumu saglabāšanas politikai, pēc tam noklikšķiniet un ritiniet, lai atrastu un pievienotu saglabāšanas atzīmi, ko tikko izveidojāt. Noklikšķiniet uz **Saglabāt**.
7. Visbeidzot, lietotāja pastkastei lietojiet saglabāšanas politiku: joprojām Exchange administrēšanas centrā dodieties uz **adresāti**  >  **pastkastes**. Izvēlieties visi lietotāji, kuriem vēlaties lietot politiku, un pēc tam izvēlieties **Rediģēt** (zīmuļa ikona).
8. Dialoglodziņā noklikšķiniet uz **pastkastes līdzekļi**. Sadaļā **saglabāšanas politika** lietojiet tikko izveidoto politiku > **Saglabāt**.
9. Norādījumus par politikas lietošanu visiem lietotājiem skatiet rakstā [saglabāšanas politikas lietošana pastkastēm](https://docs.microsoft.com/exchange/security-and-compliance/messaging-records-management/apply-retention-policy).
