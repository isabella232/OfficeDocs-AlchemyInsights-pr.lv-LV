---
title: DLP kārtula SSN nedarbojas
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
ms.openlocfilehash: 3f30998fb3bc4c5442e4e1541b87d88ecd7df6eef3a50e719fa5014eb86af39c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004989"
---
# <a name="dlp-issues-with-social-security-numbers"></a>DLP problēmas ar sociālās apdrošināšanas numuriem

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP problēmas ar SSN**

Vai jums ir problēmas ar datu zuduma novēršanu **(DLP),** kas nedarbojas satur sociālās apdrošināšanas numura **(SSN)** saturu, izmantojot sensitīvas informācijas tipu programmā Microsoft 365? Šādā gadījumā pārliecinieties, vai jūsu saturā ir nepieciešamā informācija par to, kāda ir DLP politika. 
  
Piemēram, SSN politikai, kas konfigurēta ar 85% ticamības līmeni, tiek novērtēti un jānosaka, kā kārtula aktivizē:
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-80)** 9 cipari, kas var būt formatētā vai neformatēta rakstā

- **[Modelis:](https://msconnect.microsoft.com/https:/docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-80)** Četras funkcijas meklē SSN četros dažādos modeļos:

  - Func_ssn atrod SSN ar pirms 2011. gada stipru formatējumu, kas formatēti ar svītrām vai atstarpēm (ddd-dd-dddd OR ddd dd dddd)

  - Func_unformatted_ssn atrod SSN ar pirms 2011. gada stipru formatējumu, kas nav formatēti kā deviņi secīgi cipari (ddddddddd)

  - Func_randomized_formatted_ssn atrod pēc 2011. gada SSN, kas formatēti ar domuzīmēm vai atstarpēm (ddd-dd-dddd OR ddd dd dddd)

  - Func_randomized_unformatted_ssn atrod pēc 2011. gada SSN, kuri nav formatēti kā deviņi secīgi cipari (ddddddddd)

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-79)** Nē, nav nevienas checksum

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-80)** DLP politika ir 85% droša, ka tā konstatē šāda veida sensitīvo informāciju, ja tuvumā ir 300 rakstzīmes:

  - Funkcija [Func_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-80) atrod modelim atbilstošu saturu.

  - Tiek atrasts [atslēgvārds Keyword_ssn](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#keyword_ssn) no meklēšanas. Atslēgvārdi ir šādi:  *sociālā drošība, sociālā drošība#, Soc Sec ,SSN*  . Piemēram, šis piemērs izraisītu DLP SSN politiku: **SSN: 489-36-8350**
  
Papildinformāciju par to, kas ir nepieciešams, lai noteiktu, kādi SSN tiek noteikti jūsu saturam, skatiet tālāk šī raksta sadaļā: Ko jutīgās informācijas tipi meklē [SSN](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-social-security-number-ssn)
  
Izmantojot citu iebūvēto sensitīvās informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: Ko meklē sensitīvās [informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  