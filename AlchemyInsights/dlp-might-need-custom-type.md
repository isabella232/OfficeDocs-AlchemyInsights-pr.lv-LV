---
title: DLPm, iespējams, ir nepieciešams pielāgots tips
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
ms.openlocfilehash: c0996e0cc923c13b7de3752ac6534026e8627c51
ms.sourcegitcommit: dcd1c76ced1a0cec27f4cf8d383593760c198424
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/18/2021
ms.locfileid: "59446698"
---
# <a name="dlp-might-need-a-custom-type"></a>DLPm, iespējams, ir nepieciešams pielāgots tips

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP var būt nepieciešams pielāgotas informācijas tips**

Izmantojot datu zuduma novēršanas (data loss prevention – DLP) politiku, varat identificēt un aizsargāt sensitīvus datus savā organizācijā. Dažos scenārijos, iespējams, būs jāizveido pielāgoti sensitīvas informācijas tips, lai aizsargātu jūsu organizācijas datus. Papildinformāciju skatiet rakstā Informācija [par sensitīvas informācijas tipiem un](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-learn-about) [Sensitīvas informācijas tipu entītiju definīcijas.](https://docs.microsoft.com/microsoft-365/compliance/sensitive-information-type-entity-definitions)

Papildinformāciju par to, kā izveidot pielāgotus sensitīvas informācijas tipus un politikas, skatiet šeit: 

**Iebūvēta sensitīvas informācijas tipa pielāgošana**

Ja sensitīvas informācijas tips atbilst jūsu vajadzībām tikai ar dažām uzlabotām izmaiņām, skatiet rakstu Iebūvētā jutīgas [informācijas tipa pielāgošana.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type) Piemēram, varat pievienot vai noņemt atslēgvārdus vai pievienot vai noņemt atbalsta pierādījumus, piemēram, datumu vai adresi.

**Pielāgota sensitīva informācijas tipa izveide**

Tomēr, ja nepieciešams pilnībā identificēt un aizsargāt cita veida jutīgu informāciju, laukā noklikšķiniet uz pielāgotas jutīgas Microsoft 365 atbilstības centrs. Papildinformāciju skatiet rakstā Darba [sākšana ar pielāgotiem sensitīvas informācijas tipiem.](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type)

**Pielāgota sensitīva informācijas tipa izveide & atbilstības centra PowerShell**

Visbeidzot, ja lietotāja interfeiss nenodrošina visas nepieciešamās opcijas, varat izveidot pielāgotu sensitīvas informācijas tipu drošības kontroles & centra PowerShell. Sākot ar XML failu, varat izmantot visas pieejamās opcijas. Papildinformāciju skatiet rakstā [Pielāgota sensitīvas informācijas tipa izveide, izmantojot PowerShell.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell)

Lai vispirms pārbaudītu politiku pārbaudes režīmā, skatiet rakstu Politikas ieviešana [pārbaudes režīmā](https://docs.microsoft.com/microsoft-365/compliance/dlp-learn-about-dlp#implement-policy-in-test-mode) un DLP politikas [izveide, pārbaude un pielāgošana.](https://docs.microsoft.com/microsoft-365/compliance/create-test-tune-dlp-policy) 