---
title: DLP, iespējams, ir jābūt pielāgotam tipam
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 72b16d437f97de27cbdc364f022c3e2059b31ef0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47712191"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP, iespējams, ir jābūt pielāgotam tipam

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP var būt nepieciešams pielāgotas informācijas tips**

Izmantojot datu zuduma novēršanas (DLP) politiku, varat identificēt un aizsargāt konfidenciālus datus savā organizācijā. Lai aizsargātu savas organizācijas datus, dažos scenārijos var būt nepieciešams izveidot savu **pielāgoto** sensitīvās informācijas tipu.

Piemēram, jūsu organizācijai, iespējams, ir jāidentificē un jāaizsargā darbinieku ID vai citi dati kādā jūsu organizācijas specifiskā formātā. Ja tā ir, skatiet tālāk norādītos rakstus, lai iegūtu papildinformāciju.
  
 **Iebūvētas sensitīvas informācijas tipa pielāgošana**
  
Ja iebūvētais sensitīvās informācijas tips atbilst jūsu vajadzībām, izmantojot tikai dažas tweaks, varat [pielāgot iebūvēto sensitīvās informācijas tipu](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Piemēram, varat pievienot vai noņemt atslēgvārdus vai pievienot vai noņemt apstiprinošus pierādījumus, piemēram, datumu vai adresi.
  
 **Pielāgota sensitīvas informācijas tipa izveide**
  
Taču, ja ir jāidentificē un jāaizsargā dažāda veida konfidenciāla informācija, varat [izveidot pielāgotu sensitīvas informācijas tipu](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) drošības & atbilstības centra lietotāja interfeisā.
  
**Pielāgota sensitīvas informācijas tipa izveide drošības & atbilstības centra PowerShell**

Visbeidzot, ja UI nenodrošina visas nepieciešamās opcijas, varat [izveidot pielāgotu sensitīvas informācijas tipu drošības & atbilstības centra PowerShell](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell). Sākot ar XML failu, varat izmantot visas pieejamās opcijas.
