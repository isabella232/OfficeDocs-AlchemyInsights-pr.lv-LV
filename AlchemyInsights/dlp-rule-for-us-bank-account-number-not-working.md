---
title: DLP rules ASV bankas konta numurs nedarbojas
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
ms.openlocfilehash: eb399e4b23de32a757562833ed32d97daa6a1247
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47679303"
---
# <a name="dlp-issues-with-us-bank-account-numbers"></a>DLP problēmas ar ASV bankas kontu numuriem

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP problēmas ar ASV bankas kontu numuriem**

Vai rodas problēmas saistībā ar **datu zuduma novēršanu (DLP)** , kas nestrādā ar saturu, kas satur **ASV bankas konta numuru** , izmantojot DLP sensitīvas informācijas tipu programmā O365? Ja tā ir, pārliecinieties, vai saturs satur nepieciešamo informāciju par DLP politikas izskatu, kad tas tiek novērtēts.
  
Piemēram, ja **ASV bankas konta numura** politika ir konfigurēta ar 85% ticamības līmeni, tiek novērtētas tālāk norādītās darbības, kas ir jāatrod, lai kārtula tiktu aktivizēta:
  
- **[Formāts:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#format-77)** 8-17 cipari

- **[Modelis:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#pattern-77)** 8-17 secīgi skaitļi.

- **[Kontrolsumma:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#checksum-76)** Nē, nav kontrolsummas

- **[Definīcija:](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)** DLP politika ir 75% pārliecināts, ka tā ir atklājusi šādu sensitīvas informācijas tipu, ja 300.

  - Parastā izteiksme Regex_usa_bank_account_number atrod saturu, kas atbilst rakstam

  - Ir atrasts atslēgvārds no Keyword_usa_Bank_Account.

    Piemēram, tālāk sniegtais piemērs izraisa **ASV bankas konta numura** politiku: konta 78344011 pārbaude

Lai iegūtu papildinformāciju par to, kas ir nepieciešams **ASV bankas konta numura** noteikšanai, skatiet šī raksta nākamajā sadaļā: [kādi ir sensitīvo informācijas tipi meklēt ASV bankas konta numuru](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions#us-bank-account-number)
  
Citas iebūvētas sensitīvas informācijas tipa izmantošana ir atrodama šajā rakstā, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [ko nozīmē sensitīvie informācijas tipi](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)
  