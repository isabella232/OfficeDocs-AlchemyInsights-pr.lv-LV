---
title: DLP kārtula kredītkartes numuram nedarbojas
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
ms.openlocfilehash: bd4f200233d5571fc7b01576038e7b3951a07716a7d5948005418d2896291ee5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005097"
---
# <a name="dlp-issues-with-credit-card-numbers"></a>DLP problēmas ar kredītkaršu numuriem

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP problēmas ar kredītkaršu numuriem**

Vai, izmantojot DLP sensitīvas informācijas tipu O365, rodas problēmas saistībā ar datu zuduma novēršanu (Data Loss Prevention – **DLP)** nedarbojas saturam, kurā ir kredītkartes numurs?  Šādā gadījumā pārliecinieties, vai jūsu saturā ir nepieciešamā informācija, lai aktivizētu DLP politiku, kad tā tiek novērtēta. Piemēram, kredītkartes  politikai, kas konfigurēta ar 85% ticamības līmeni, tiek novērtēti un jānosaka, kā kārtula aktivizē:
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-19)** 16 cipari, kurus var formatēt vai neformatēt (dddddddddddddd), un tiem ir jāiziet cauri Lūhnas testam.

- **[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-19)** Ļoti sarežģīts un jaudīgs modelis, kas nosaka visu galveno zīmolu kartes visā pasaulē, tostarp Visa, MasterCard, Discover Card, JCB, American Express, dāvanu kartes un vizītkartes.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-19)** Jā, Lūhnas pārbaužu laukā

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-19)** DLP politika ir 85% droša, ka tā konstatē šāda veida sensitīvo informāciju, ja tuvumā ir 300 rakstzīmes:

  - Funkcija Func_credit_card atrod modelim atbilstošu saturu.

  - Viens no šiem nosacījumiem ir patiess:

  - Tiek atrasts atslēgvārds Keyword_cc_verification no meklēšanas.

  - Tiek atrasts atslēgvārds Keyword_cc_name no meklēšanas

  - Funkcija Func_expiration_date atrod datumu pareizajā datumu formātā.

  - Pārbaudes tiek nododas

    Piemēram, šajā piemērā ir izraisīta DLP kredītkaršu numuru politika:

  - Visa: 4485 3647 3952 7352
  
  - Derīgums beidzas: 2/2009

Papildinformāciju par to,  kas ir nepieciešams, lai noteiktu kredītkartes numuru, lai noteiktu jūsu saturu, skatiet tālāk šī raksta sadaļā: Ko jutīgās informācijas tipi [meklē kredītkarti#](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#credit-card-number)
  
Izmantojot citu iebūvēto sensitīvās informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: Ko meklē sensitīvās [informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  