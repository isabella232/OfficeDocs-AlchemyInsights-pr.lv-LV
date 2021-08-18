---
title: Koplietojamas Microsoft 365 programmas lieluzņēmumiem izvietošanai RDS, Terminal Server vai VDI
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: ''
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: b8df97c19937a757c1de9865b6c7b8d1cddfd62d
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58325610"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Koplietojamas Microsoft 365 programmas lieluzņēmumiem izvietošanai RDS, Terminal Server vai VDI

Lai izvietotu Microsoft 365 programmas lieluzņēmumiem, izmantojot attālās darbvirsmas pakalpojumus (Remote Desktop Services — RDS), iepriekš nosaukti par Termināļa pakalpojumiem:

- Jums jābūt Microsoft 365 for Business plānam vai Office 365 plānam, kurā ietilpst Microsoft 365 programmas lieluzņēmumiem, piemēram, Office 365 Enterprise E3 vai Enterprise E5.
   **Piezīme.** Microsoft 365 programmas darbam un Microsoft 365 Business Standard plānos Microsoft 365 programmas lieluzņēmumiem.
- Iespējojiet koplietojamā [datora aktivizāciju.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

**Piezīme.** Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgs,](https://aka.ms/SaRA_OfficeSCA_M365Portal) lai instalētu Microsoft 365 programmas lieluzņēmumiem koplietojamā datora aktivizācijas režīmā.

Papildinformāciju par priekšnosacījumiem, iestatīšanas norādījumiem un norādījumiem par pielāgotām instalācijām, izmantojot Office izvietošanas rīku, skatiet rakstā [Microsoft 365 programmas lieluzņēmumiem izvietošana, izmantojot attālās darbvirsmas pakalpojumus.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Lai novērstu ar koplietojama datora aktivizēšanu saistītas kļūdas:

- Skatiet [rakstu Problēmu novēršana saistībā ar koplietojama datora aktivizēšanu Microsoft 365 programmas lieluzņēmumiem](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Skatiet rakstu [Atiestatīt Microsoft 365 programmas uzņēmumam aktivizēšanas statusam](https://go.microsoft.com/fwlink/?linkid=2109218).

Ja vēlaties instalēt ierīces Microsoft 365 programmas lieluzņēmumiem RDS no ierīces Microsoft 365 administrēšanas centrs, kas izmanto instalācijas noklusējuma ***iestatījumus,*** veiciet tālāk norādītās darbības.

1. Pārbaudiet, kādu abonementu izmantojat. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Ja nepieciešams, pārslēdzieties uz citu abonementu. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Ja Office jau ir instalēta RDS serverī, izmantojot jebkuru citu Microsoft abonementu, atinstalējiet to. Piemēram, dodoties uz **Vadības**  >  **panelis; atinstalējiet programmu**. Ja rodas [problēmas, atinstalējiet](https://aka.ms/SARA-OfficeUninstall-Alchemy) atbalsta un atkopšanas palīgs Microsoft atbalsta un atkopšanas palīgs.
4. RDS serverī pierakstieties e-pasta Microsoft 365 administrēšanas centrs ar savu administratora kontu un [instalējiet Microsoft 365 programmas lieluzņēmumiem](https://portal.office.com/OLS/MySoftware.aspx).
5. Pēc Office instalēšanas ***neatveriet lietojumprogrammas un nepiesakieties*** jebkurā Office programmā.
6. RDS serverī iespējojiet koplietojama datora aktivizēšanu, rediģējot reģistru, veicot tālāk norādītās darbības.
   1. Ar peles labo Windows pogu ekrāna apakšējā kreisajā stūrī un atlasiet **Palaist**. Lodziņā Atvērt ierakstiet **regedit un pēc** tam atlasiet **Labi**.
   2. Kad **saņemat** aicinājumu atļaut reģistra redaktoram veikt izmaiņas ierīcē, atlasiet Jā.
   3. Reģistra redaktorā pievienojiet virknes **vērtību SharedComputerlicensing** ar iestatījumu 1 sadaļā HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS serverī pierakstieties kā ***lietotājs*** un pārliecinieties, vai koplietojama datora aktivizēšana [ir iespējota Microsoft 365 programmas lieluzņēmumiem.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
