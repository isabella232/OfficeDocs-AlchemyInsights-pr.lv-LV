---
title: Nedarbojas DLP kārtula kredītkartes numurs
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: e2e93bed44749b9017dc6ff919a151d46da7a3fc
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507413"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problēmas ar kredītkaršu numuriem

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP problēmas ar kredītkaršu numuriem**

Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nedarbojas saturu, kas satur **kredītkartes numuru** , izmantojot DLP konfidenciālu informācijas tipu O365? Ja tā ir, pārliecinieties, vai saturs satur nepieciešamo informāciju, lai izraisītu DLP politiku, kad tā tiek novērtēta. Piemēram, **kredītkartes politikai** , kas konfigurēta ar ticamības līmeni 85%, tiek novērtēti tālāk minētie un ir jānosaka, lai kārtula izraisītu:
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cipari, kurus var formatēt vai Neformatēt (dddddddddddddd), un ir jānokārto Luhn tests.

- **[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Ļoti sarežģīts un spēcīgs modelis, kas atrod kārtis no visiem lielākajiem zīmoliem visā pasaulē, ieskaitot visa, MasterCard, Discover Card, JCB, American Express, dāvanu kartes un pusdienotājs kartes.

- **[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Jā, Luhn kontrolsumma

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP politika ir 85% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:

  - Funkcija Func_credit_card atrod saturu, kas atbilst paraugam.

  - Ir spēkā kāds no šiem:

  - Tiek atrasts atslēgvārds no Keyword_cc_verification.

  - Tiek atrasts atslēgvārds no Keyword_cc_name

  - Funkcija Func_expiration_date atrod datumu pareizajā datuma formātā.

  - Kontrolsumma iet

    Piemēram, šādu paraugu izraisīs DLP kredītkartes numuru politika:

  - Vīza: 4485 3647 3952 7352
  
  - Beidzas: 2/2009

Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai jūsu saturam tiktu noteikts **kredītkartes numurs** , skatiet tālāk minēto sadaļu šajā rakstā: [kādas sensitīvās informācijas veidi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number) tiek atrasti, izmantojot kredītkarti #
  
Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  