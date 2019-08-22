---
title: DLP likums mums bankas konta numuru, nedarbojas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1287"
- "3200001"
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 0a32708b5ac8d95ec6777ada2d151a15f90d65bf
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36529881"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP jautājumus ar mums bankas kontu numurus

Vai jums ir problēmas ar **Datu zaudējumu novēršanas (DLP)** nav darba saturs, kurā **ASV bankas konta numuru** , lietojot DLP sensitīvu informāciju tipa O365? Šādā gadījumā pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko meklē DLP politikas, kad tās tiek novērtētas.
  
Piemēram, **ASV bankas konta numurs** politikas konfigurēta ar ticamības līmeni, 85 %, šādi tiek novērtētas un ir noteikusi kārtulas, lai iedarbinātu:
  
- **[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8 17 cipari

- **[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 secīgus ciparus.

- **[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nē, nav neviena kontrolsumma

- **[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP politika ir 75 % ir pārliecināti, ka tas ir konstatējusi šāda veida konfidenciālu informāciju, ja laikā tuvumu 300 rakstzīmes:

  - Regular expression Regex_usa_bank_account_number konstatē saturu, kas atbilst paraugam

  - No Keyword_usa_Bank_Account atslēgvārds ir atrasts.

    Piemēram, šādas izlases izraisītu politikas **ASV bankas konta numurs** : norēķinu konts 78344011

Papildinformāciju par to, kādām ir jābūt **ASV bankas konta numurs** tiktu atrasta jūsu saturu, skatiet šī raksta sadaļā šādi: [Kāda jutīgas informācijas tipus meklēt ASV bankas konta numurs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Izmantojot dažādas iebūvētas sensitīvu informāciju tipu, skatiet šajā rakstā informāciju par to, kas ir nepieciešami citi veidi: [meklēt ko jutīgas informācijas veidus](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  