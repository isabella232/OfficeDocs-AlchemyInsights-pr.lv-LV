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
ms.openlocfilehash: 35ef317ea87fedd01c08fee5b370e3c81e515c27
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58322006"
---
# <a name="installing-office-on-a-terminal-server"></a>Instalē Office termināļa serverī

Servera izvietošanai Microsoft 365 programmas lieluzņēmumiem serverī, Windows attālās darbvirsmas pakalpojumi (Remote Desktop Services — RDS), iepriekš nosaukti par Termināļa pakalpojumiem:
  
- Jūsu rīcībā jābūt Microsoft 365 abonementam, kurā ietilpst Microsoft 365 programmas lieluzņēmumiem, piemēram, Office 365 Enterprise E3 vai Enterprise E5. Microsoft 365 programmas darbam un Microsoft 365 programmas darbam Premium plānos nav iekļauti Microsoft 365 programmas lieluzņēmumiem.

- Jums ir jāiespējo koplietojamā [datora aktivizācija.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

Ja vēlaties instalēt ierīces Microsoft 365 programmas lieluzņēmumiem RDS no ierīces Microsoft 365 administrēšanas centrs, kas izmanto noklusējuma instalācijas ***iestatījumus,*** veiciet tālāk norādītās darbības.

    **Tip**: You can also download and run the [Microsoft Support and Recovery Assistant](https://aka.ms/SaRA_OfficeSCA_M365Portal) to install Microsoft 365 Apps for enterprise in shared computer activation mode.
  
1. Pārbaudiet, Microsoft 365 savu abonementu. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)

2. Ja nepieciešams, pārslēdzieties uz citu Microsoft 365 abonementu. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)

3. Ja Office jau ir instalēta RDS serverī, izmantojot jebkuru citu Microsoft 365 abonementu, atinstalējiet to. Piemēram, dodoties uz Vadības \> panelis. Atinstalējiet programmu. Ja rodas [problēmas, atinstalējiet](https://aka.ms/SARA-OfficeUninstall-Alchemy) atbalsta un atkopšanas palīgs Microsoft atbalsta un atkopšanas palīgs.

4. RDS serverī pierakstieties e-pasta Microsoft 365 administrēšanas centrs ar savu administratora kontu un [instalējiet Microsoft 365 programmas lieluzņēmumiem](https://portal.office.com/OLS/MySoftware.aspx).

5. Pēc Office instalēšanas ***neatveriet lietojumprogrammas un nepiesakieties*** jebkurā Office programmā.

6. RDS serverī iespējojiet koplietojama datora aktivizēšanu, rediģējot reģistru, veicot tālāk norādītās darbības.

1. Ar peles labo Windows pogu ekrāna apakšējā kreisajā stūrī un atlasiet Palaist. Lodziņā Atvērt ierakstiet **regedit un** pēc tam atlasiet Labi.

2. Kad saņemat aicinājumu atļaut reģistra redaktoram veikt izmaiņas ierīcē, atlasiet Jā.

3. Reģistra redaktorā pievienojiet virknes **vērtību SharedComputerlicensing** ar iestatījumu 1 sadaļā HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. RDS serverī pierakstieties kā ***lietotājs*** un pārliecinieties, vai koplietojama datora aktivizēšana [ir iespējota Microsoft 365 programmas lieluzņēmumiem.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)

Papildinformāciju par priekšnosacījumiem, iestatīšanas norādījumus un norādījumus par pielāgotām instalācijām, izmantojot Office izvietošanas rīku, skatiet rakstā Microsoft 365 programmas lieluzņēmumiem izvietošana, [izmantojot attālās darbvirsmas pakalpojumus.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)
  
Lai novērstu ar koplietojama datora aktivizēšanu saistītas kļūdas, lūdzu, skatiet rakstu Problēmu novēršana saistībā ar [koplietojama datora aktivizēšanu Microsoft 365 programmas lieluzņēmumiem](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
  