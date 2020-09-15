---
title: Office instalēšana termināļa serverī — nelicencēts
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "917"
- "2000020"
ms.assetid: b1074430-489e-4d49-bfe4-3d8783d8073c
ms.openlocfilehash: 1d862f60e7a8a4c90c83f4538e57972b0c0547da
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47663124"
---
# <a name="installing-office-on-a-terminal-server"></a>Office instalēšana termināļa serverī

Microsoft 365 lietojumprogrammu izvietošanai uzņēmumam Windows serverī, izmantojot attālās darbvirsmas pakalpojumus (RDS), kas iepriekš nosaukta par termināļa pakalpojumiem:
  
- Jums ir jābūt Microsoft 365 abonementam, kurā ietilpst Microsoft 365 lietojumprogrammas uzņēmumam, piemēram, Office 365 Enterprise E3 vai Enterprise E5. Microsoft 365 programmās darbam un Microsoft 365 programmas darbam Premium plāniem nav iekļautas Microsoft 365 lietojumprogrammas darbam ar Enterprise.

- Ir jāiespējo [koplietojamā datora aktivizēšana](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

Ja vēlaties instalēt Microsoft 365 lietojumprogrammas uzņēmumam RDS no Microsoft 365 administrēšanas centra, ***kas izmanto noklusējuma instalācijas iestatījumus***, veiciet tālāk norādītās darbības.

> [!TIP]
> Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA_OfficeSCA_M365Portal) , lai instalētu Microsoft 365 lietojumprogrammas uzņēmumam koplietojamā datora aktivizēšanas režīmā.
  
1. Pārbaudiet, kāds ir Microsoft 365 abonements. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ja nepieciešams, pārslēdzieties uz citu Microsoft 365 abonementu. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ja sistēma Office jau ir instalēta RDS serverī, izmantojot jebkurus citus Microsoft 365 abonementus, atinstalējiet to. Piemēram, atverot vadības paneļa \> Atinstalēt programmu. Ja rodas problēmas, atinstalējiet [, izmantojot Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SARA-OfficeUninstall-Alchemy) .

4. RDS serverī pierakstieties Microsoft 365 administrēšanas centrā ar administratora kontu un [instalējiet microsoft 365 lietojumprogrammas uzņēmumam Enterprise](https://portal.office.com/OLS/MySoftware.aspx).

5. Pēc Office instalēšanas ***neatveriet vai pierakstieties*** jebkurā Office lietojumprogrammā.

6. RDS serverī iespējojiet koplietotu datora aktivizāciju, rediģējot reģistru, veicot tālāk norādītās darbības.

1. Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna kreisajā apakšējā stūrī un atlasiet palaist. Lodziņā Atvērt ierakstiet **regedit**un pēc tam atlasiet Labi.

2. Atlasiet Jā, kad tiek parādīta uzvedne ar aicinājumu atļaut reģistra redaktoru veikt izmaiņas jūsu ierīcē.

3. Reģistra redaktorā pievienojiet **SharedComputerLicensing** virknes vērtību ar 1 HKEY_LOCAL_MACHINE \software\microsoft \Office\ClickToRun\Configuration.

7. RDS serverī ***pierakstieties kā lietotājs*** un [Pārbaudiet, vai koplietojamā datora aktivizācija ir iespējota Microsoft 365 lietojumprogrammām darbam ar Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

Lai iegūtu detalizētāku informāciju par priekšnosacījumiem, iestatīšanas norādījumiem un norādījumiem par pielāgotām instalācijām, izmantojot Office izvietošanas rīku, skatiet rakstu [Microsoft 365 lietojumprogrammu izvietošana uzņēmumam, izmantojot attālās darbvirsmas pakalpojumus](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).
  
Lai labotu kļūdas, kas saistītas ar koplietojamu datora aktivizāciju, skatiet rakstu [problēmu novēršana saistībā ar koplietojamu datora aktivizāciju Microsoft 365 programmās darbam ar Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  