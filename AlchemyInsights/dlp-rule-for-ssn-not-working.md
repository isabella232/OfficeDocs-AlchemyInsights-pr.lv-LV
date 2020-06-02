---
title: Nav darba SSN kārtula DLP
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: 35859bce89ef1ae9b6a9e706fc316b0ee6cd27d1
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507377"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP jautājumi ar sociālās apdrošināšanas numuriem

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP problēmas ar SSNs**

Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nestrādā saturu, kas satur **sociālās apdrošināšanas numurs (SSN)** , izmantojot sensitīvu informācijas tipa Microsoft 365? Ja tā ir, pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko DLP politika meklē. 
  
Piemēram, SSN politika, kas konfigurēta ar ticamības līmeni 85%, tiek novērtēti un ir jānosaka kārtulu aktivizācijai:
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cipari, kas var būt formatēts vai Neformatēts raksts

- **[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četras funkcijas meklē SSNs četros dažādos modeļos:

  - Func_ssn atrod SSNs ar Pre-2011 spēcīgu formatējumu, kas formatēts domuzīmes vai atstarpes (DDD-dd-dddd vai DDD dd dddd)

  - Func_unformatted_ssn atrod SSNs ar Pre-2011 spēcīgu formatējumu, kas ir Neformatēts kā deviņus secīgus ciparus (ddddddddd)

  - Func_randomized_formatted_ssn atrod pēc-2011 SSNs, kas formatēti ar domuzīmes vai atstarpes (DDD-dd-dddd vai DDD dd dddd)

  - Func_randomized_unformatted_ssn atrod post-2011 SSNs, kas ir Neformatēts kā deviņus secīgus ciparus (ddddddddd)

- **[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nē, nav kontrolsummas

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP politika ir 85% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:

  - [Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) atrod saturu, kas atbilst paraugam.

  - Tiek atrasts atslēgvārds no [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Atslēgvārdu piemēri ietver: *sociālo nodrošinājumu, sociālo nodrošinājumu #, SOC SEC, SSN* . Piemēram, šāda parauga izraisītu DLP SSN politika: **SSN: 489-36-8350**
  
Lai iegūtu papildinformāciju par to, kas ir nepieciešams noteikt SSNs saturu, skatiet šajā sadaļā šo rakstu: [kāda sensitīva informācijas tipi meklē SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  