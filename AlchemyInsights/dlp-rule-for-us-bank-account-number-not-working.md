---
title: DLP kārtula ASV bankas konta numurs nedarbojas
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
ms.openlocfilehash: 0b5c1fb175275028c56e47080708520fe115fb38
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932542"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problēmas ar ASV bankas kontu numuri

**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā. Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi. Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.

Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā. Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju. Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.

**DLP problēmas ar ASV bankas kontu numuri**

Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nedarbojas saturu, kas satur **ASV bankas konta numuru** , izmantojot DLP konfidenciālu informācijas tipu O365? Ja tā ir, pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko DLP politika meklē, kad tas ir novērtēts.
  
Piemēram, **ASV bankas konta numuru** politika konfigurēta ar ticamības līmeni 85%, tiek novērtēti un jānosaka kārtulas aktivizācijai:
  
- **[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** 8-17 cipari

- **[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** 8-17 secīgi cipari.

- **[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nē, nav kontrolsummas

- **[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)** DLP politika ir 75% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:

  - Regulārā izteiksme Regex_usa_bank_account_number atrod saturu, kas atbilst rakstam

  - Tiek atrasts atslēgvārds no Keyword_usa_Bank_Account.

    Piemēram, šādu piemēru varētu izraisīt **ASV bankas konta numuru** politika: norēķinu konts 78344011

Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai jūsu saturam tiktu noteikts **ASV bankas konta numurs** , skatiet tālāk minēto sadaļu šajā rakstā: [kāda sensitīva informācijas veida informācija mums šķiet bankas konta numurs](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us-bank-account-number)
  
Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)
  