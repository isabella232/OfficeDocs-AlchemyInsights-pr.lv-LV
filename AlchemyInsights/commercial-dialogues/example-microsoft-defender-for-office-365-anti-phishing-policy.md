---
title: Microsoft Defender piemērs Office 365 pretpikšķerēšanas politikai
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
ms.openlocfilehash: b59abdeea6ac9be7e498e2b1ba531e7bf611c92097fbc12237e78364dae84f35
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54035013"
---
# <a name="example-microsoft-defender-for-office-365-anti-phishing-policy"></a>Microsoft Defender piemērs Office 365 pretpikšķerēšanas politikai

Šie iestatījumi iespējo politiku ar *nosaukumu Domēns un UZŅĒMUMA VADĪTĀJS.* Šī politika nodrošina lietotāja un domēna aizsardzību pret personificēšanu un pēc tam lieto politiku visiem e-pasta ziņojumiem, ko saņem lietotāji domēnā. Vispirms, lai izveidotu politiku, pievienojiet šādu informāciju:

- **Nosaukums**: Domēna un uzņēmuma administratora **apraksts:** nodrošina, ka bez personificējas ne uzņēmuma vadītājs, ne jūsu domēns.
  **Lietots:** Atlasiet **Adresāta domēns ir**. Sadaļā **Kāds no šiem** atlasiet **Izvēlēties** un pēc tam atlasiet domēnu. Atlasiet **+ Pievienot**. Atzīmējiet izvēles rūtiņu blakus domēna nosaukumam sarakstā *(piemēram,* contoso.com ) un pēc tam atlasiet **Pievienot**. Atlasiet **Gatavs**.
- Kad politika ir izveidota, jūs varat precizēt politiku, izmantojot šādas opcijas:
  - **Pievienojiet lietotājus, lai tos aizsargātu:** Šajā piemērā pievienojiet vismaz CEO e-pasta adresi.
  - **Domēnu pievienošana, lai aizsargātu:** pievienojiet organizācijas domēnu, kurā iekļauts ceO birojs.
  - **Izvēlieties darbības:** ja e-pasta ziņojumu ir nosūtījis personificēts **lietotājs,** atlasiet Novirzīt ziņojumu uz citu e-pasta adresi **un** pēc tam ievadiet drošības administratora e-pasta adresi (piemēram, *securityadmin@contoso.com*). Ja **e-pasta ziņojumu nosūta personificēts domēns,** atlasiet **Karantīnā ievietot ziņojumu**.
  - **Pastkastes informācija:** veidojot jaunu pretpikšķerēšanas politiku, šī opcija tiek atlasīta pēc noklusējuma. Lai iegūtu vislabākos **rezultātus,** atstājiet šo iestatījumu ieslēgtu.
  - **Uzticamu sūtītāju un domēnu pievienošana:** Šajā piemērā nedefinēt nekādus ignorējumus.
- Kad esat pārskatījis iestatījumus, atbilstoši **atlasiet Izveidot šo politiku** **vai** Saglabāt.

Papildinformāciju skatiet rakstā [Pretpikšķerēšanas politikas programmā Microsoft 365.](https://go.microsoft.com/fwlink/?linkid=2092235)
