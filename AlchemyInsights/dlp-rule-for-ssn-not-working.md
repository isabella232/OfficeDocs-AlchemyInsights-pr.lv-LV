---
title: DLP kārtula nedarbojas SSN
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
ms.openlocfilehash: 757136c39700f12f40f839b29277a59b0e436f03
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529868"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problēmas, kas saistītas ar sociālās apdrošināšanas numurus

Vai jums ir problēmas ar **Datu zaudējumu novēršanas (DLP)** saturu, lietojot Office 365 konfidenciālas informācijas tips, kas satur **Sociālās apdrošināšanas numurs (SAN)** nedarbojas? Šādā gadījumā pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko meklē DLP politiku. 
  
Piemēram, SSN politikai, kas konfigurēts ar ticamības līmeni, 85 %, šādi tiek novērtētas un ir noteikusi kārtulas, lai iedarbinātu:
  
- **[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-80)** 9 cipari, kas var būt paraugs formatētu vai neformatētu

- **[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četras funkcijas meklēt SSNs četrus dažādus modeļus:

  - Func_ssn atrod SSNs ar pre-2011 spēcīgu formatējumu, kas ir formatētas defises vai atstarpes (ddd dd dddd OR ddd dd dddd)

  - Func_unformatted_ssn atrod SSNs ar pre-2011 spēcīgu formatējumu, kas ir formatēta kā deviņus secīgus ciparus (ddddddddd)

  - Func_randomized_formatted_ssn atrod amatā 2011 SSNs, kas ir formatētas defises vai atstarpes (ddd dd dddd OR ddd dd dddd)

  - Func_randomized_unformatted_ssn atrod amatā 2011 SSNs, kas ir formatēta kā deviņus secīgus ciparus (ddddddddd)

- **[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-79)** Nē, nav neviena kontrolsumma

- **[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-80)** DLP politika ir 85 % ir pārliecināti, ka tas ir konstatējusi šāda veida konfidenciālu informāciju, ja laikā tuvumu 300 rakstzīmes:

  - [Func_ssn funkcija](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80) atrod saturu, kas atbilst rakstam.

  - No [Keyword_ssn](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#keyword_ssn) atslēgvārds ir atrasts. Atslēgvārdi piemēri ietver: *sociālās apdrošināšanas, sociālās nodrošināšanas #, Soc. Sec, SSN* . Piemēram, šādas izlases izraisītu DLP SSN politikā: **SSN: 489-36-8350**
  
Papildinformāciju par to, kādām ir jābūt SSNs tiktu atrasta jūsu saturu, skatiet šī raksta sadaļā šādi: [Kāda jutīgas informācijas tipus meklēt SSNs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-social-security-number-ssn)
  
Izmantojot dažādas iebūvētas sensitīvu informāciju tipu, skatiet šajā rakstā informāciju par to, kas ir nepieciešami citi veidi: [meklēt ko jutīgas informācijas veidus](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  