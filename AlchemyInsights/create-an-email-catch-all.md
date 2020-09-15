---
title: E-pasta nozvejas izveide visiem
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 262d2c6a7181d94094f3d840c4ba3ebd07000cf4
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712993"
---
# <a name="create-an-email-catch-all"></a>E-pasta nozvejas izveide visiem

Ir stingri kavēta nozvejas lietošana. Labāk ir nodrošināt atlēcienu sūtītājam, kas nosūta sūtītājus par to, ka viņu ziņojumu nevarēja nosūtīt kā adresētu, lai viņi varētu rīkoties. Varat arī ierobežot monitorētās pastkastes tikai iepriekš derīgās e-pasta adreses. 

Visas nozvejas visas pastkastes saņems lielu surogātpasta daudzumu, un tā, iespējams, tiks aizpildīta, ja netiek stingri pārraudzīta. (Ir saņemti ierobežojumi.) 

Ja izlemjat turpināt, veiciet tālāk norādītās darbības.

1. Izveidojiet dinamisku adresātu grupu & iekļaujiet visus adresātu tipus.

2. Izveidojiet atvēlētu pastkasti e-pasta ziņojumu nozvejai, piemēram, catchall@domain.com.

3. Konkrētajā domēnā iestatiet DomainType uz "InternalRelay". Ja vēlāk noņemat catch all, noteikti iestatiet domēnu atpakaļ uz autoritatīvo.

4. Izveidojiet pasta risinātājahttps://Configure.Office.com/Scenario.aspx?SID=12 transporta kārtulu šādi:

    - Ja sūtītājs ir ārpus organizācijas
    - Ziņojuma novirzīšana uz Catchall@domain.com
    - Izņemot gadījumus, kad adresāts ir allusers@domain.com dalībnieks (adresātu grupā ir visi dalībnieki)
    - Nodrošiniet, lai validētu, ka jaunās pastkastes tiek pievienotas dinamiskās adresātu grupai
