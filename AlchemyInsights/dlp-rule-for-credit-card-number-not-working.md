---
title: DLP kārtula nedarbojas kredītkartes numuru
ms.author: cmcatee
author: cmcatee-MSFT
manager: mnirkhe
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 4b8897c5cc8286bc4bd49860658a5a94ad17380d
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/30/2019
ms.locfileid: "29657474"
---
Vai jums ir problēmas ar **Datu zaudējumu novēršanas (DLP)** nav darba saturs, kurā **Kredītkartes numuru** , lietojot DLP sensitīvu informāciju tipa O365? Šādā gadījumā pārliecinieties, ka jūsu saturs ietver visu vajadzīgo informāciju, lai iedarbinātu DLP politiku, ja tas tiek novērtēts. Piemēram, **kredītkaršu politikas** konfigurēta ar ticamības līmeni, 85 % šādu tiek novērtētas un ir noteikusi kārtulas, lai iedarbinātu: 
  
- **[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cipari, kuru var formatēt vai neformatētu (dddddddddddddddd) un jāiziet Luhn tests. 
    
- **[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Ļoti sarežģīta un spēcīgu modelis, kas atklāj kārtis no visiem galvenajiem zīmoliem visā pasaulē, tai skaitā Visa, Mastercard, Discover Card, JCB, American Express, dāvanu kartes un pusdienotājs kārtis. 
    
- **[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Jā, Luhn kontrolsumma 
    
- **[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politika ir 85 % ir pārliecināti, ka tas ir konstatējusi šāda veida konfidenciālu informāciju, ja laikā tuvumu 300 rakstzīmes: 
    
  - Func_credit_card funkcija konstatē saturu, kas atbilst rakstam.
    
  - Ir spēkā kāds no šiem: 
    
  - No Keyword_cc_verification atslēgvārds ir atrasts.
    
  - No Keyword_cc_name atslēgvārds ir atrasts
    
  - Func_expiration_date funkcija atrod datuma pareizā datuma formātā.
    
  - Kontrolsumma caurlaides
    
    Piemēram, šādas izlases izraisītu DLP kredītkartes numuru politiku:
    
  - Vīzas: 4485 3647 3952 7352 
    
  - Expires: 2/2009
    
Papildinformāciju par to, kas tiek prasīts **Kredītkartes numurs** tiktu atrasta jūsu saturu, skatiet šī raksta sadaļā šādi: [Ko jutīgas informācijas tipus meklēt kredītkartes #](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)
  
Izmantojot dažādas iebūvētas sensitīvu informāciju tipu, skatiet šajā rakstā informāciju par to, kas ir nepieciešami citi veidi: [Meklēt ko jutīgas informācijas veidus](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  

