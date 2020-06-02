---
title: DLP noteikums ASV/Lielbritānijas pases numurs nedarbojas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: 3d3b7dc2d9510376bc9eef6ec69b87ad7c681b05
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507305"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problēmas ar DLP-US/UK pases numuru

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP jautājumi ar ASV/Lielbritānijas pases numuriem**

Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nestrādā par saturu, kas satur **ASV/UK pases numuru** , izmantojot DLP konfidenciālu informāciju tipa O365? Ja tā ir, pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko DLP politika meklē, kad tas ir novērtēts.
  
Piemēram, **ASV/Apvienotās Karalistes pases numuru** politikai, kas konfigurēta ar ticamības līmeni 75%, tiek novērtēti tālāk minētie, un tie ir jānosaka, lai kārtula izraisītu
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Deviņi cipari

- **[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Deviņus secīgus ciparus

- **[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nē, nav kontrolsummas

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP politika ir 75% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:

  - Funkcija Func_usa_uk_passport atrod saturu, kas atbilst paraugam.

  - Tiek atrasts atslēgvārds no Keyword_passport.

    Piemēram, šādu paraugu izraisītu **ASV/Lielbritānijas pases numuru** politika: ASV pases numurs 123456789

Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai jūsu saturam tiktu noteikts ASV/Apvienotās Karalistes pases numurs, skatiet šajā rakstā minēto sadaļu: [kādas sensitīvās informācijas veidi meklē US/UK pases numuru](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  