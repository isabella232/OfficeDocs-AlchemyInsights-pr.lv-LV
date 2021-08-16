---
title: DLP kārtula ASV/UK pases numuram nedarbojas
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
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 85e3ed7fdc221981de13ab6e2ada8adf2a3a80b40ff163981e047cc4a02a1514
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54004953"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problēmas ar DLP — ASV/UK pases numuri

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP problēmas ar ASV/UK pases numuriem**

Vai jums ir problēmas ar datu zuduma novēršanu **(DLP),** kas nedarbojas satur **US/UK** pases numuru, izmantojot DLP sensitīvas informācijas tipu O365? Šādā gadījumā pārliecinieties, vai jūsu saturā ir nepieciešamā informācija par to, ko meklē DLP politika, kad tā tiek novērtēta.
  
Piemēram, **ASV/UK** pases numura politikai, kas konfigurēta ar 75% ticamības līmeni, tiek novērtētas tālāk minētās vērtības, un tās ir jānosaka, lai kārtula aktivizētu
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Deviņi cipari

- **[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Deviņi secīgi cipari

- **[Checksum:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nē, nav nevienas checksum

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP politika ir 75% droša, ka tā konstatē šāda veida sensitīvo informāciju, ja tuvumā ir 300 rakstzīmes:

  - Funkcija Func_usa_uk_passport atrod modelim atbilstošu saturu.

  - Tiek atrasts atslēgvārds Keyword_passport no meklēšanas.

    Piemēram, šajā piemērā **ASV/UK** pases numura politika ir trigeris: ASV pases numura 123456789

Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai ASV/APVIENOTĀS KARALISTES pases numuru noteiktu jūsu saturam, skatiet šī raksta sadaļu: Ko sensitīvas informācijas tipi meklē [ASV/Apvienotās Karalistes pases numuram](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Izmantojot citu iebūvēto sensitīvās informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: Ko meklē sensitīvās [informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  