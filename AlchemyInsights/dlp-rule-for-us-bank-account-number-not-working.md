---
title: DLP kārtula ASV bankas konta numuram nedarbojas
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
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: d19b2dcc29e23fab522159945496165338a117a47bfcfcadf0b93e4e5f14464f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54005025"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problēmas ar ASV bankas konta numuriem

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP problēmas ar ASV bankas konta numuriem**

Vai, izmantojot DLP sensitīvas informācijas tipu O365, rodas problēmas saistībā ar datu zuduma novēršanu **(DLP)** nedarbojas saturam, kurā ir **ASV** bankas konta numurs? Šādā gadījumā pārliecinieties, vai jūsu saturā ir nepieciešamā informācija par to, ko meklē DLP politika, kad tā tiek novērtēta.
  
Piemēram, ASV bankas konta **numura** politikai, kas konfigurēta ar 85% ticamības līmeni, tiek novērtēti un jānosaka, kā kārtula aktivizē:
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8–17 cipari

- **[Raksts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8–17 secīgi cipari.

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nē, nav nevienas checksum

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP politika ir 75% droša, ka tā konstatē šāda veida sensitīvo informāciju, ja tuvumā ir 300 rakstzīmes:

  - Parastā izteiksme Regex_usa_bank_account_number atrast saturu, kas atbilst modelim

  - Tiek atrasts Keyword_usa_Bank_Account atslēgvārds.

    Piemēram, tālāk sniegtajā paraugā ir norādīts ASV bankas konta **numura** politikas trigeris: konta numura 78344011

Lai iegūtu papildinformāciju par to, kas ir nepieciešams **ASV** bankas konta numura noteikšanai, lai noteiktu jūsu saturu, skatiet šī raksta sadaļu: Sensitīvās informācijas tipi meklē [ASV bankas konta numuru](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Izmantojot citu iebūvēto sensitīvās informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: Ko meklē sensitīvās [informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  