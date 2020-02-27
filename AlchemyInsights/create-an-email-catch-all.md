---
title: Izveidot e-pasta catch visu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001524"
- "3732"
ms.openlocfilehash: 35f31c1662547d57c2fc9978ffb495ac29abcc01
ms.sourcegitcommit: 67015549afcbe05f3b77ea314e2ef7e0e439f9f2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/26/2020
ms.locfileid: "42286199"
---
# <a name="create-an-email-catch-all"></a>Izveidot e-pasta catch visu

Visas nozvejas izmantošana tiek stingri kavēti. Tas ir labāk, lai nodrošinātu piepeši atpakaļ sūtītājam izīrēšanas sūtītājiem zināt viņu ziņu nevar piegādāt kā adresēts, lai viņi varētu rīkoties. Varat arī ierobežot pārraudzītas pastkastes tikai catch iepriekš derīgu e-pasta adreses. 

Jebkurš nozvejas visas pastkastes saņems daudz surogātpasta un galu galā var aizpildīt, ja nav cieši jāuzrauga. (Ir saņemšanas ierobežojumi.) 

Ja nolemjat turpināt, veiciet tālāk norādītās darbības.

1. Dinamiskās adresātu grupas izveide & iekļaut "visi adresātu tipi".

2. Izveidojiet speciālu pastkasti, lai noķertu e-pastus, piemēram, catchall@domain.com.

3. Konkrētu domēna, iestatiet DomainType "InternalRelay". Ja jūs vēlāk izņemt nozvejas visiem, pārliecinieties, lai uzstādītu domēna atpakaļ autoritatīvu.

4. Izveidojiet šādu Mailflow transporta kārtulu:

    - Ja sūtītājs ir "ārpus organizācijas"
    - Novirzīt ziņojumu uz Catchall@domain.com
    - Izņemot, ja saņēmējs ir biedrs allusers@domain.com (adresātu grupa ir visi dalībnieki)
    - Pārliecinieties, lai apstiprinātu, ka jaunās pastkastes tiek pievienotas dinamiskā adresātu grupa
