---
title: DLP kārtula US / UK pases numurs nedarbojas
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 5722f7b6c9a2f905fed2ef4164787e020260edf7
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/30/2019
ms.locfileid: "29656430"
---
Vai rodas problēmas ar darba saturu, kas satur **Datu zaudējumu novēršanas (DLP)** **ASV / UK pases numurs** lietojot DLP sensitīvu informāciju tipa O365? Šādā gadījumā pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko meklē DLP politikas, kad tās tiek novērtētas. 
  
Piemēram, **US / UK pases numurs** politika, kas konfigurēts ar 75 % ticamības pakāpei, šādi tiek novērtētas un ir noteikusi kārtulas, lai iedarbinātu 
  
- **[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Deviņu ciparu 
    
- **[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Deviņus secīgus ciparus 
    
- **[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nē, nav neviena kontrolsumma 
    
- **[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika ir 75 % ir pārliecināti, ka tas ir konstatējusi šāda veida konfidenciālu informāciju, ja laikā tuvumu 300 rakstzīmes: 
    
  - Func_usa_uk_passport funkcija konstatē saturu, kas atbilst rakstam.
    
  - No Keyword_passport atslēgvārds ir atrasts.
    
    Piemēram, lai izraisītu šādu paraugu **US / UK pases numurs** politika: ASV pases numurs 123456789 
    
Lai iegūtu vairāk informācijas par to, kas ir nepieciešama ASV / UK pases numurs tiktu atrasta jūsu saturu, skatiet nākošo sadaļu šajā pantā: [ko jutīgas informācijas tipus meklēt ASV / UK pases numurs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)
  
Izmantojot dažādas iebūvētas sensitīvu informāciju tipu, skatiet šajā rakstā informāciju par to, kas ir nepieciešami citi veidi: [Meklēt ko jutīgas informācijas veidus](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

