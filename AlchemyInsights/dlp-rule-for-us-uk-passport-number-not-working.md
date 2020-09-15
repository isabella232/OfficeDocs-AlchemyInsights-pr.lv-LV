---
title: DLP rules ASV/Apvienotās Karalistes pases numurs nedarbojas
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
ms.openlocfilehash: c6c7191f380f264113e2042f2869d9767922b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679231"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a>Problēmas ar DLP-US/UK Passport numuriem

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP problēmas ar ASV/Apvienotās Karalistes pases numuriem**

Vai rodas problēmas saistībā ar **datu zuduma novēršanu (DLP)** , kas nestrādā ar saturu, kas ietver **ASV/Apvienotās Karalistes pases numuru** , ja izmantojat datu tipu DLP ar O365? Ja tā ir, pārliecinieties, vai saturs satur nepieciešamo informāciju par DLP politikas izskatu, kad tas tiek novērtēts.
  
Piemēram, **ASV/Apvienotās Karalistes pases numuru** politikai, kas konfigurēta ar 75% ticamības līmeni, tiek novērtētas un ir jānosaka, ka kārtula tiek aktivizēta
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** Deviņi cipari

- **[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** Deviņi secīgi cipari

- **[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nē, nav kontrolsummas

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#definition-77)** DLP politika ir 75% pārliecināts, ka tā ir atklājusi šādu sensitīvas informācijas tipu, ja 300.

  - Funkcija Func_usa_uk_passport atrod saturu, kas atbilst rakstam.

  - Ir atrasts atslēgvārds no Keyword_passport.

    Piemēram, tālāk sniegtais piemērs izraisa **ASV/Apvienotās Karalistes pases numuru** politiku: ASV pases numurs 123456789

Lai iegūtu papildinformāciju par to, kas ir nepieciešams ASV/Apvienotās Karalistes pases numura satura noteikšanai, skatiet šī raksta nākamajā sadaļā: [kādi ir sensitīvo informācijas tipi meklēt ASV/Apvienotās Karalistes pases numuru](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us--uk-passport-number)
  
Citas iebūvētas sensitīvas informācijas tipa izmantošana ir atrodama šajā rakstā, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [ko nozīmē sensitīvie informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  