---
title: E-pasta tvert visu izveide
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 2b9131a620139a93ddb844fd49d8fa2ed68e52c2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816207"
---
# <a name="create-an-email-catch-all"></a>E-pasta tvert visu izveide

Tvert visu izmantošana ir ļoti neiesarunāta. Ir labāk nodrošināt atsišanu atpakaļ uz sūtītāju, kas informēja sūtītājus par to, ka viņu ziņojumus nevarēja piegādāt, lai viņi varētu rīkoties. Varat arī ierobežot pārraudzīto pastkasti, lai tā tvertu tikai iepriekš derīgas e-pasta adreses. 

Jebkura tvērēja no visām pastkastēm saņems daudz surogātpasta, un tas var tikt aizpildīts, ja netiks rūpīgi pārraudzīts. (Pastāv saņemšanas ierobežojumi.) 

Ja izlemjat turpināt, veiciet tālāk norādītās darbības.

1. Izveidojiet dinamisko adresātu grupu, & ietvert "Visi adresātu tipi".

2. Izveidojiet atvēlētu pastkasti, lai tvertu e-pasta ziņojumus, piemēram, catchall@domain.com.

3. Konkrētam domēnam iestatiet DomainType vērtību "InternalRelay". Ja vēlāk noņemsit visu lomu, iestatiet domēnu atpakaļ uz Autoritatīvs.

4. Izveidojiet pasta plūsmas transporta kārtulu, kā norādīts tālāk.

    - Ja sūtītājs ir ārpus organizācijas
    - Novirzīt ziņojumu uz Catchall@domain.com
    - Izņemot to, ka adresāts ir grupas allusers@domain.com (Adresātu grupā ir visi dalībnieki)
    - Kā pārliecināties, vai jaunās pastkastes tiek pievienotas dinamisko adresātu grupai
