---
title: Office instalēšana termināļa serverī-nelicencēta
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: c781e9fd492ff97bc80667956e6609b3d40b28b4
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508635"
---
# <a name="installing-office-on-a-terminal-server"></a>Office instalēšana termināļa serverī

Lai izvietotu Microsoft 365 Apps Enterprise Windows Server, izmantojot attālās darbvirsmas pakalpojumu (RDS), iepriekš nosaukto termināļa pakalpojumi:
  
- Jums ir jābūt Microsoft 365 abonements, kas ietver Microsoft 365 lietojumprogrammas uzņēmumiem, piemēram, Office 365 Enterprise E3 vai Enterprise E5. Microsoft 365 lietojumprogrammas uzņēmumiem un Microsoft 365 lietojumprogrammām Business Premium plāniem neietver Microsoft 365 lietojumprogrammas uzņēmumiem.

- Ir jāiespējo [koplietojamā datora aktivizācija](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ja vēlaties instalēt Microsoft 365 Apps Enterprise RDS no Microsoft 365 administrēšanas centrs, ***kas izmanto noklusējuma instalācijas iestatījumus***, rīkojieties šādi.

> [!TIP]
> Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA_OfficeSCA_M365Portal) , lai instalētu Microsoft 365 lietojumprogrammas Enterprise koplietojamo datoru aktivizācijas režīmā.
  
1. Pārbaudiet, kāds ir Microsoft 365 abonements. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ja nepieciešams, pārslēdzieties uz citu Microsoft 365 abonementu. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ja Office jau ir instalēta RDS serverī, izmantojot citu Microsoft 365 abonementu, atinstalējiet to. Piemēram, atverot vadības paneli, \> atinstalējiet programmu. Atinstalējiet, izmantojot [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ja rodas problēmas.

4. RDS serverī, pierakstieties Microsoft 365 administrēšanas centrs ar administratora kontu un [instalēt Microsoft 365 lietojumprogrammas uzņēmumiem](https://portal.office.com/OLS/MySoftware.aspx).

5. Pēc Office instalēšanas ***neatveriet vai pierakstieties*** nevienā no Office lietojumprogrammām.

6. Serverī RDS iespējojiet koplietojamo datora aktivizāciju, rediģējot reģistru, veicot šādas darbības:

1. Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna kreisajā apakšējā stūrī un atlasiet palaist. Lodziņā Atvērt ierakstiet **regedit**un pēc tam atlasiet Labi.

2. Atlasiet Jā, kad tiek piedāvāts atļaut reģistra redaktoram veikt izmaiņas ierīcē.

3. Reģistra redaktorā pievienojiet virknes vērtību **Sharedcomputerlicensing** ar iestatījumu 1 zem HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. RDS serverī, ***pierakstieties kā lietotājs*** un [Pārbaudiet, vai ir iespējota Microsoft 365 lietojumprogrammas uzņēmumiem koplietojamā datora aktivizācija](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Lai iegūtu papildinformāciju par priekšnosacījumi, uzstādīšanas instrukcijas un norādījumus par pielāgoto instalāciju, izmantojot Office izvietošanas rīks, lūdzu, skatiet [izvietot Microsoft 365 lietojumprogrammas uzņēmumiem, izmantojot attālās darbvirsmas pakalpojumu](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Lai labotu kļūdas, kas saistītas ar koplietojamu datora aktivizāciju, lūdzu, skatiet [problēmu novēršana saistībā ar koplietojamo datora aktivizēšanu Microsoft 365 lietojumprogrammām uzņēmumam](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  