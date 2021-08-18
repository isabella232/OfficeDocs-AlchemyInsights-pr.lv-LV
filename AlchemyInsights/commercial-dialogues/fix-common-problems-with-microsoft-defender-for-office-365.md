---
title: Biežāk sastopamo problēmu novēršana saistībā ar Microsoft Defender Office 365
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
- "9000760"
- "7391"
ms.openlocfilehash: c5043bcd3d40dccc76b348f436001408e42ee7f9
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58330067"
---
# <a name="fix-common-problems-with-microsoft-defender-for-office-365"></a>Biežāk sastopamo problēmu novēršana saistībā ar Microsoft Defender Office 365

Tālāk ir piedāvājam dažus risinājumus bieži sastopamām problēmām ar Programmatūru Microsoft Defender Office 365.

- **Ziņojuma aizkave:**

  E-pasta ziņojumu piegādes aizkaves var izraisīt Seifs pielikumu skenēšana. Papildinformāciju skatiet rakstā [Seifs politikas iestatījumi](https://docs.microsoft.com/microsoft-365/security/office-365-security/safe-attachments#safe-attachments-policy-settings).

- **Ziņošana par aplami pozitīviem vai negatīviem rezultātiem:**

  Papildinformāciju skatiet rakstā [Ziņošana par ziņojumiem un failiem korporācijai Microsoft.](https://docs.microsoft.com/microsoft-365/security/office-365-security/report-junk-email-messages-to-microsoft)

- **Iespējot Seifs saites aizsardzību:**

  1. Vietnes Microsoft 365 Defender dodieties uz E-& un sadarbības politikas <https://security.microsoft.com/> **&** \> **Kārtulu** apdraudējumu \>  \> **politikas Seifs saites** **sadaļā** Politikas.

     Lai pārietu tieši uz **lapu Seifs saites,** izmantojiet <https://security.microsoft.com/safelinksv2> .

  2. Lapā **Seifs** saites atlasiet politiku, noklikšķinot uz politikas nosaukuma.
  3. Parādītā detalizētās informācijas izlidošanas logā veiciet kādu no šīm darbībām:
     - Lai pievienotu jaunu politiku, atlasiet **+ Izveidot**. Tiks palaists vednis, kas palīdzēs definēt politikas iestatījumus.
     - Lai rediģētu esošu politiku, atlasiet politiku, noklikšķinot uz politikas nosaukuma. Parādītā detalizētās informācijas izlidošanas logā **sadaļā** Aizsardzības iestatījumi **atlasiet** Rediģēt.
  4. Aizsardzības **iestatījumu lapā** konfigurējiet tālāk norādītos iestatījumus.
     - Ieslēdziet **opciju Atlasiet darbību nezināmiem iespējami ļaunprātīgiem vietrāžiem URL ziņojumos.**
     - Atlasiet **Lietot drošās saites ziņojumiem, kas nosūtīti organizācijā.**

  Papildinformāciju skatiet [rakstā Saišu Seifs iestatīšana programmatūrā Microsoft Defender Office 365.](https://docs.microsoft.com/microsoft-365/security/office-365-security/set-up-safe-links-policies)
