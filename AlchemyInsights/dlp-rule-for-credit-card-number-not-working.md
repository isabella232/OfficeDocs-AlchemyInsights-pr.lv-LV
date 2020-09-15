---
title: Jūsu kredītkartes numura DLP noteikums nedarbojas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: d5dd6354e7a1bcbb7f2fb917952ddbee5077e88d
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679448"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problēmas ar kredītkaršu numuriem

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP problēmas ar kredītkaršu numuriem**

Vai rodas problēmas saistībā ar **datu zuduma novēršanu (DLP)** , kas nestrādā ar saturu, kas satur **kredītkartes numuru** , izmantojot DLP sensitīvas informācijas tipu programmā O365? Ja jā, pārliecinieties, vai saturs satur nepieciešamo informāciju, lai aktivizētu DLP politiku, kad tas tiek novērtēts. Piemēram, **kredītkaršu politikai** , kas konfigurēta ar 85% ticamības līmeni, tiek novērtētas tālāk norādītās darbības un ir jānosaka, ka kārtula tiek aktivizēta:
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cipari, kas var būt formatēti vai neformatēti (dddddddddddddddd), un ir jāiztur Luhn pārbaude.

- **[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Ļoti sarežģīts un robusts modelis, kas atklāj kartes no galvenajiem zīmoliem visā pasaulē, tostarp visa, MasterCard, Discovery Card, JCB, American Express, dāvanu kartes un Diner Cards.

- **[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Jā, Luhn kontrolsumma

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP politika ir 85% pārliecināts, ka tā ir atklājusi šādu sensitīvas informācijas tipu, ja 300.

  - Funkcija Func_credit_card atrod saturu, kas atbilst rakstam.

  - Ir patiess viens no šiem apgalvojumiem:

  - Ir atrasts atslēgvārds no Keyword_cc_verification.

  - Ir atrasts atslēgvārds no Keyword_cc_name

  - Funkcija Func_expiration_date atrod datumu pareizajā datuma formātā.

  - Kontrolsummas caurlaides

    Piemēram, tālāk norādītie paraugi izraisītu DLP kredītkaršu numuru politiku:

  - Vīza: 4485 3647 3952 7352
  
  - Derīgums beidzas: 2/2009

Lai iegūtu papildinformāciju par to, kas ir nepieciešams **kredītkartes numura** noteikšanai jūsu saturam, skatiet šī raksta nākamajā sadaļā: [kādi ir sensitīvo informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number) .
  
Citas iebūvētas sensitīvas informācijas tipa izmantošana ir atrodama šajā rakstā, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [ko nozīmē sensitīvie informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  