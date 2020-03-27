---
title: Nav darba SSN kārtula DLP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 4ec0df9d4954a8c65f0c34188d285dd8cf44a4f2
ms.sourcegitcommit: d108a2da2f5dab05246e30b5108cca5173e09051
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/26/2020
ms.locfileid: "42977313"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP jautājumi ar sociālās apdrošināšanas numuriem

**Svarīgi**: šo bezprecedenta laikos, mēs veikt pasākumus, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami-Lūdzu, apmeklējiet [SharePoint Online pagaidu līdzekļu korekcijas](https://aka.ms/ODSPAdjustments) , lai iegūtu vairāk informācijas.

**DLP problēmas ar SSNs**

Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nestrādā saturu, kas satur **sociālās apdrošināšanas numurs (SSN)** , izmantojot sensitīvu informācijas tipa Office 365? Ja tā ir, pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko DLP politika meklē. 
  
Piemēram, SSN politika, kas konfigurēta ar ticamības līmeni 85%, tiek novērtēti un ir jānosaka kārtulu aktivizācijai:
  
- **[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cipari, kas var būt formatēts vai Neformatēts raksts

- **[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četras funkcijas meklē SSNs četros dažādos modeļos:

  - Func_ssn atrod SSNs ar Pre-2011 spēcīgu formatējumu, kas formatēts domuzīmes vai atstarpes (DDD-dd-dddd vai DDD dd dddd)

  - Func_unformatted_ssn atrod SSNs ar Pre-2011 spēcīgu formatējumu, kas ir Neformatēts kā deviņus secīgus ciparus (ddddddddd)

  - Func_randomized_formatted_ssn atrod pēc-2011 SSNs, kas formatēti ar domuzīmes vai atstarpes (DDD-dd-dddd vai DDD dd dddd)

  - Func_randomized_unformatted_ssn atrod post-2011 SSNs, kas ir Neformatēts kā deviņus secīgus ciparus (ddddddddd)

- **[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nē, nav kontrolsummas

- **[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politika ir 85% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:

  - [Funkcija Func_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) atrod saturu, kas atbilst paraugam.

  - Tiek atrasts atslēgvārds no [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) . Atslēgvārdu piemēri ietver: *sociālo nodrošinājumu, sociālo nodrošinājumu #, SOC SEC, SSN* . Piemēram, šāda parauga izraisītu DLP SSN politika: **SSN: 489-36-8350**
  
Lai iegūtu papildinformāciju par to, kas ir nepieciešams noteikt SSNs saturu, skatiet šajā sadaļā šo rakstu: [kāda sensitīva informācijas tipi meklē SSN](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  