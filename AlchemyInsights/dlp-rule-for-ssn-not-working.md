---
title: Ar SSN nedarbojošos DLP kārtulu
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
- "1242"
- "3200001"
ms.assetid: ac265ee6-c946-476e-9bf0-0ea0e8adc98a
ms.openlocfilehash: b221e66862ca01074f380fbb8433f8f9cac044cb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679376"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problēmas ar sociālās drošības numuriem

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP problēmas ar SSNs**

Vai rodas problēmas ar **datu zuduma novēršanu (DLP)** , kas nestrādā ar saturu, kurā ir iekļauts **sociālās drošības numurs (SAN)** , ja programmā Microsoft 365 izmantojat sensitīvu informācijas tipu? Ja tā ir, pārliecinieties, vai saturs satur nepieciešamo informāciju par DLP politikas izskatu. 
  
Piemēram, ja SSN politika ir konfigurēta ar 85% ticamības līmeni, tiek novērtēti tālāk norādītie un ir jānosaka, ka kārtula tiek aktivizēta:
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cipari, kas var būt formatētā vai neformatētā modelī

- **[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četras funkcijas meklē SSNs četros dažādos modeļos:

  - Func_ssn atrod SSNs, izmantojot iepriekš 2011 stipru formatējumu, kas formatēts ar defisēm vai atstarpēm (DDD-dd-dddd vai DDD dd dddd)

  - Func_unformatted_ssn atrod SSNs, izmantojot iepriekš 2011 stipru formatējumu, kas nav formatēts kā deviņi secīgi cipari (ddddddddd)

  - Func_randomized_formatted_ssn atrod ziņu par 2011 SSNs, kas formatēta ar defisēm vai atstarpēm (DDD-dd-dddd vai DDD dd dddd)

  - Func_randomized_unformatted_ssn atrod post-2011 SSNs, kas nav formatēti kā deviņi secīgi cipari (ddddddddd)

- **[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nē, nav kontrolsummas

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP politika ir 85% pārliecināts, ka tā ir atklājusi šādu sensitīvas informācijas tipu, ja 300.

  - [Funkcija Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) atrod saturu, kas atbilst rakstam.

  - Ir atrasts atslēgvārds no [Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) . Atslēgvārdu piemēri ietver:  *Social Security, Social Security #, SOC SEC, SSN*  . Piemēram, tālāk sniegtais piemērs izraisa DLP SSN politiku: **SSN: 489-36-8350**
  
Lai iegūtu papildinformāciju par to [, kas ir](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn) nepieciešams, lai SSNs jūsu saturam, skatiet tālāk šajā rakstā norādītās iespējas.
  
Citas iebūvētas sensitīvas informācijas tipa izmantošana ir atrodama šajā rakstā, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [ko nozīmē sensitīvie informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  