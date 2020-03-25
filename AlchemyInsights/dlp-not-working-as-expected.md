---
title: DLP nedarbojas, kā paredzēts
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 1/9/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1241"
- "3200001"
ms.assetid: f6fcf5ad-55a1-4f25-af27-1f7c1ce06409
ms.openlocfilehash: a56e18ddadef3a2f9056978b8542c1dba8f29665
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932629"
---
# <a name="dlp-not-working-as-expected"></a>DLP nedarbojas, kā paredzēts

**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā. Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi. Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.

Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā. Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju. Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.

 **DLP iestatīšana**

Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** Office 365 nedarbojas, kā paredzēts? Ja tā ir, pārliecinieties, vai **DLP politika** ir iestatīta pareizi un jūsu dati satur **DLP politika** meklē, kad tas tiek novērtēts.
  
DLP politika ļauj identificēt un aizsargāt sensitīvu informāciju jūsu organizācijā. Lai iestatītu DLP politikas, izmantojiet [šeit](https://docs.microsoft.com/office365/securitycompliance/prevent-data-loss#set-up-dlp)informāciju.
  
 **Kāda DLP politika meklē**
  
Izmantojot **iebūvēto sensitīvo informācijas tipu** Office 365 drošības un atbilstības centru, DLP politikas meklēt konkrētu modeļu un elementi, nosakot šo sensitīvo tipu.
  
- **Iebūvēti sensitīvi informācijas veidi**

    Lai iegūtu informāciju par iebūvētiem sensitīviem tipiem un to, kāda ir DLP politika, kad tiek noteikta sensitīva tipa noteikšana, skatiet: [kāda veida sensitīvo informācijas tipu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).

- **Pielāgoti sensitīvi informācijas tipi**

    Ja mēģināt izveidot pielāgotu konfidenciālus informācijas tipus, izmantojiet šo rakstu, lai iegūtu informāciju par to, kā izveidot pielāgotu sensitīvu tipu: [izveidojiet pielāgotu sensitīvo informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type).

**DLP politikas pārbaude**

Lai pārbaudītu datus ar iebūvētu vai pielāgotu sensitīvu informācijas tipu, izmantojiet opciju **testa tips** sadaļā **klasifikācija** > **sensitīvo informācijas tipi**. Papildinformāciju skatiet sadaļā [pielāgotu sensitīvo informācijas tipu testēšana](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type#test-custom-sensitive-information-types-in-the-security--compliance-center).

 **Ziņojumi**
  
- Iegūstiet sensitīvu datu ieskati ar [DLP pārskatiem.](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#dlp-reports)

- Skatiet detalizētu informāciju par notikumu, izmantojot [ziņojumu par incidentu](https://docs.microsoft.com/office365/securitycompliance/data-loss-prevention-policies#incident-reports).
