---
title: Microsoft Defender for Office 365 pretpikšķerēšanas politikas piemērs
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
ms.openlocfilehash: eabff70c22b641627d3ab6c0b2f8846a0be2f49e
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694034"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Microsoft Defender for Office 365 pretpikšķerēšanas politikas piemērs

Šie iestatījumi iespējo politiku ar nosaukumu *Domain un CEO*. Šī politika nodrošina gan lietotāja, gan domēna aizsardzību no personificēšanas un pēc tam lieto politiku visiem lietotājiem, kas ir saņemti domēnā. Vispirms pievienojiet tālāk norādīto informāciju, lai izveidotu politiku.

- **Nosaukums**: Domain and CEO **Apraksts**: nodrošina, ka vadītājs un jūsu domēns netiek personificēts.
  **Lietots**: atlasiet **adresātu domēnu**. Sadaļā **jebkurš no šiem** atlasiet **izvēlēties** un pēc tam atlasiet domēnu. Atlasiet **+ Pievienot**. Atzīmējiet izvēles rūtiņu blakus domēna nosaukumam sarakstā (piemēram, *contoso.com*) un pēc tam atlasiet **Pievienot**. Atlasiet **gatavs**.
- Pēc politikas izveides varat precizēt politiku, izmantojot tālāk norādītās opcijas.
  - **Lietotāju pievienošana aizsardzībai:** Šim piemēram, pievienojiet izpilddirektora e-pasta adresi.
  - **Pievienot domēnus, lai aizsargātu**: pievienojiet organizācijas domēnu, kas ietver CEO biroju.
  - **Izvēlieties darbības**: **Ja e-pasta ziņojums tiek nosūtīts personificētam lietotājam**, atlasiet **novirzīt ziņojumu uz citu e-pasta adresi** un pēc tam ievadiet drošības administratora e-pasta adresi (piemēram, *SecurityAdmin@contoso.com*). **Ja e-pasta ziņojums tiek sūtīts ar personificētu domēnu**, atlasiet **ievietot ziņojumu karantīnā**.
  - **Pastkastes informācija**: pēc noklusējuma šī opcija ir atlasīta, kad izveidojat jaunu pretpikšķerēšanas politiku. Atstājiet **šo iestatījumu,** lai iegūtu vislabākos rezultātus.
  - **Pievienojiet uzticamos sūtītājus un domēnus:** Šajā piemērā nedefinējiet nevienu ignorēšanu.
- Kad būsit pārskatījis savus iestatījumus, atlasiet **izveidot šo politiku** vai pēc vajadzības **Saglabāt**.

Papildinformāciju skatiet rakstā [pretpikšķerēšanas politikas programmā Microsoft 365](https://go.microsoft.com/fwlink/?linkid=2092235).
