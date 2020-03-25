---
title: Nedarbojas DLP kārtula kredītkartes numurs
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932450"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problēmas ar kredītkaršu numuriem

**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā. Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi. Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.

Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā. Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju. Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.

**DLP problēmas ar kredītkaršu numuriem**

Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nedarbojas saturu, kas satur **kredītkartes numuru** , izmantojot DLP konfidenciālu informācijas tipu O365? Ja tā ir, pārliecinieties, vai saturs satur nepieciešamo informāciju, lai izraisītu DLP politiku, kad tā tiek novērtēta. Piemēram, **kredītkartes politikai** , kas konfigurēta ar ticamības līmeni 85%, tiek novērtēti tālāk minētie un ir jānosaka, lai kārtula izraisītu:
  
- **[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cipari, kurus var formatēt vai Neformatēt (dddddddddddddd), un ir jānokārto Luhn tests.

- **[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Ļoti sarežģīts un spēcīgs modelis, kas atrod kārtis no visiem lielākajiem zīmoliem visā pasaulē, ieskaitot visa, MasterCard, Discover Card, JCB, American Express, dāvanu kartes un pusdienotājs kartes.

- **[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Jā, Luhn kontrolsumma

- **[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politika ir 85% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:

  - Funkcija Func_credit_card atrod saturu, kas atbilst paraugam.

  - Ir spēkā kāds no šiem:

  - Tiek atrasts atslēgvārds no Keyword_cc_verification.

  - Tiek atrasts atslēgvārds no Keyword_cc_name

  - Funkcija Func_expiration_date atrod datumu pareizajā datuma formātā.

  - Kontrolsumma iet

    Piemēram, šādu paraugu izraisīs DLP kredītkartes numuru politika:

  - Vīza: 4485 3647 3952 7352
  
  - Beidzas: 2/2009

Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai jūsu saturam tiktu noteikts **kredītkartes numurs** , skatiet tālāk minēto sadaļu šajā rakstā: [kādas sensitīvās informācijas veidi](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number) tiek atrasti, izmantojot kredītkarti #
  
Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  