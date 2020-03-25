---
title: DLP var būt nepieciešams pielāgots tips
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932665"
---
# <a name="dlp-might-need-a-custom-type"></a>DLP var būt nepieciešams pielāgots tips

**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā. Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi. Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.

Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā. Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju. Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.

**DLP var būt nepieciešams pielāgots informācijas tips**

Ar datu zuduma novēršanas (DLP) politiku jūs varat identificēt un aizsargāt sensitīvus datus savā organizācijā. Dažos gadījumos, lai aizsargātu savas organizācijas datus, iespējams, vajadzēs izveidot **pielāgotu** sensitīvo informācijas tipu.

Piemēram, jūsu organizācijai var būt nepieciešams identificēt un aizsargāt darbinieku ID vai citus datus noteiktā formātā, kas specifisks jūsu organizācijai. Ja tā ir, skatiet šos rakstus, lai iegūtu papildinformāciju.
  
 **Iebūvēta sensitīva informācijas tipa pielāgošana**
  
Ja iebūvētais sensitīvo informācijas tips atbilst jūsu vajadzībām, izmantojot tikai dažas tweaks, varat [pielāgot iebūvēto sensitīvo informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type). Piemēram, varat pievienot vai noņemt atslēgvārdus vai pievienot vai noņemt apstiprinošus pierādījumus, piemēram, datumu vai adresi.
  
 **Pielāgota sensitīva informācijas tipa izveide**
  
Tomēr, ja jums ir jāidentificē un jāaizsargā cita veida sensitīva informācija, varat [izveidot pielāgotu sensitīvo informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) drošības & atbilstības centra lietotāja interfeisā.
  
**Pielāgota sensitīva informācijas tipa izveide drošības & atbilstības centra PowerShell**

Visbeidzot, ja UI nesniedz visas jums nepieciešamo opciju, [drošības & atbilstības centra PowerShell var izveidot pielāgotu sensitīvu informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell). Sākot ar XML failu, var izmantot visas pieejamās opcijas.
