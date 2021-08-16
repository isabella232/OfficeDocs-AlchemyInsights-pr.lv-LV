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
ms.openlocfilehash: 1b0beb89eaf8a4105659a1faa7cc723174a73940ef46bd2355bdddfee7b94adb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54030801"
---
# <a name="dlp-might-need-a-custom-type"></a>DLPm, iespējams, ir nepieciešams pielāgots tips

**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).

**DLP var būt nepieciešams pielāgotas informācijas tips**

Izmantojot datu zuduma novēršanas (data loss prevention – DLP) politiku, varat identificēt un aizsargāt sensitīvus datus savā organizācijā. Dažos scenārijos, iespējams, būs jāizveido **pielāgoti** sensitīvas informācijas tips, lai aizsargātu jūsu organizācijas datus.

Piemēram, jūsu organizācijai var būt nepieciešams identificēt un aizsargāt darbinieku ID vai citus datus noteiktā formātā, kas ir specifiski jūsu organizācijai. Šādā gadījumā papildinformāciju skatiet šādos rakstos:
  
 **Iebūvēta sensitīvas informācijas tipa pielāgošana**
  
Ja iebūvētais sensitīvās informācijas tips atbilst jūsu vajadzībām, tikai dažas izmaiņas, varat pielāgot iebūvēto [sensitīvās informācijas tipu](https://docs.microsoft.com/microsoft-365/compliance/customize-a-built-in-sensitive-information-type). Piemēram, varat pievienot vai noņemt atslēgvārdus vai pievienot vai noņemt atbalsta pierādījumus, piemēram, datumu vai adresi.
  
 **Pielāgota sensitīva informācijas tipa izveide**
  
Tomēr, ja nepieciešams pilnībā identificēt un aizsargāt cita veida [](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type) jutīgu informāciju, drošības un atbilstības centra & lietotāja interfeisā varat izveidot pielāgotu sensitīvas informācijas tipu.
  
**Pielāgota sensitīva informācijas tipa izveide & atbilstības centra PowerShell**

Visbeidzot, ja lietotāja interfeiss nenodrošina visas nepieciešamās opcijas, rakstā Drošības un atbilstības centra [PowerShell varat izveidot pielāgotu sensitīvas informācijas & tipu.](https://docs.microsoft.com/microsoft-365/compliance/create-a-custom-sensitive-information-type-in-scc-powershell) Sākot ar XML failu, varat izmantot visas pieejamās opcijas.
