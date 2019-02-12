---
title: DLP likums mums bankas konta numuru, nedarbojas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 80b40145-8376-4c3a-8d22-6efb9f9cb271
ms.openlocfilehash: 9ebfa6bc09cef9ab7c30bddb4fcb8b6be3ab55a5
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29916423"
---
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
  
Izmantojot dažādas iebūvētas sensitīvu informāciju tipu, skatiet šajā rakstā informāciju par to, kas ir nepieciešami citi veidi: [Meklēt ko jutīgas informācijas veidus](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

