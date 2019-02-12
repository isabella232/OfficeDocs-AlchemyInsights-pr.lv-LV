---
title: Office instalēšanas termināla serverī - nelicencētu
ms.author: pebaum
author: pebaum
ms.date: 12/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 971edd9c064b448446ba16361e99df4a2291c14f
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29918984"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalējot Office termināļu serverī

Par to, kā izvietot Office 365 ProPlus Windows serverī, izmantojot attālās darbvirsmas pakalpojumu (RDS), iepriekš dēvēts par termināļa pakalpojumi:
  
- Datorā jābūt instalētai Office 365 plānu, kas ietver Office 365 ProPlus, piemēram, Office 365 Enterprise E3 vai uzņēmuma E5. Office 365 Business un Office 365 Business Premium plāni nav iekļauti Office 365 ProPlus.
    
- Ir jāiespējo [koplietojamās datora aktivizāciju](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).
    
Ja vēlaties instalēt Office 365 ProPlus RDS no portāla Office 365 * * *kas izmanto instalācijas noklusējuma iestatījumus* * *, rīkojieties šādi: 
  
1. Pārbaudiet, kāda Office 365 plānu, kas jums ir. [Uzzināt cik](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)
    
2. Ja nepieciešams, pārslēdzieties uz citu Office 365 plānu. [Uzzināt cik](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)
    
3. Ja RDS servera, izmantojot citas Office 365 plāni jau ir instalēta Office, noņemt tās instalāciju. Piemēram, dodoties uz Control Panel \> atinstalēt programmu. Atinstalējiet to, izmantojot [Microsoft atbalsts un palīgs atgūšanas](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ja jūs strādājat par jautājumiem. 
    
4. RDS serverī, pierakstieties pakalpojumā Office 365 portāls ar administratora kontu un [instalēt Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
    
5. Pēc tam, kad ir instalēta Office * * *nav atvērts vai pierakstieties* * * lai visas Office lietojumprogrammas. 
    
6. Serverī RDS iespējotu koplietojamās datora aktivizāciju, rediģējot reģistru, veicot šādas darbības:
    
1. Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna kreisajā apakšējā stūrī un izvēlieties Run. Lodziņā Atvērt ierakstiet **regedit**un pēc tam izvēlieties Labi. 
    
2. Izvēlieties Jā, ja tiek prasīts atļaut Registry Editor veikt izmaiņas jūsu ierīcē.
    
3. Reģistra redaktoru, pievienot virknes vērtība ir **SharedComputerLicensing** , kurā 1 zem HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration. 
    
7. Serverī RDS * * *, pierakstieties kā lietotājs* * * un [pārbaudīt, ka koplietojama datora aktivizēšana ir iespējota Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).
    
Sīkāku informāciju par priekšnoteikumiem, uzstādīšanas instrukcijas un norādījumi par pielāgoto instalāciju, izmantojot rīku Office izvietošanu, lūdzu skatīt [Izvietot Office 365 ProPlus, izmantojot attālās darbvirsmas pakalpojumu](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Lai novērstu kļūdas, kas attiecas uz koplietojamās datora aktivizāciju, lūdzu, skatiet [novērst problēmas, kas saistītas ar koplietojama datora aktivizāciju Office 365 ProPlus](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  

