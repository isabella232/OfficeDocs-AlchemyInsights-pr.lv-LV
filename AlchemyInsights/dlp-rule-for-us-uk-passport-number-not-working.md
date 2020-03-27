---
title: DLP noteikums ASV/Lielbritānijas pases numurs nedarbojas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 534e258c31a9a71c618765511487487c53f455b5
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977113"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problēmas ar DLP-US/UK pases numuru

**Svarīgi**: šo bezprecedenta laikos, mēs veikt pasākumus, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami-Lūdzu, apmeklējiet [SharePoint Online pagaidu līdzekļu korekcijas](https://aka.ms/ODSPAdjustments) , lai iegūtu vairāk informācijas.

**DLP jautājumi ar ASV/Lielbritānijas pases numuriem**

Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nestrādā par saturu, kas satur **ASV/UK pases numuru** , izmantojot DLP konfidenciālu informāciju tipa O365? Ja tā ir, pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko DLP politika meklē, kad tas ir novērtēts.
  
Piemēram, **ASV/Apvienotās Karalistes pases numuru** politikai, kas konfigurēta ar ticamības līmeni 75%, tiek novērtēti tālāk minētie, un tie ir jānosaka, lai kārtula izraisītu
  
- **[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Deviņi cipari

- **[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Deviņus secīgus ciparus

- **[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nē, nav kontrolsummas

- **[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika ir 75% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:

  - Funkcija Func_usa_uk_passport atrod saturu, kas atbilst paraugam.

  - Tiek atrasts atslēgvārds no Keyword_passport.

    Piemēram, šādu paraugu izraisītu **ASV/Lielbritānijas pases numuru** politika: ASV pases numurs 123456789

Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai jūsu saturam tiktu noteikts ASV/Apvienotās Karalistes pases numurs, skatiet šajā rakstā minēto sadaļu: [kādas sensitīvās informācijas veidi meklē US/UK pases numuru](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  