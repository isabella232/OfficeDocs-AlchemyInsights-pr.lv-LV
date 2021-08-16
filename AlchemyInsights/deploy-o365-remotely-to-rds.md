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
ms.openlocfilehash: 55b86557ec205dde2c459d76e8e330d2a8271dbec723f079e119ebe409b41c3f
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54031485"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Koplietojamas Microsoft 365 programmas lieluzņēmumiem izvietošanai RDS, Terminal Server vai VDI

Lai izvietotu Microsoft 365 programmas lieluzņēmumiem, izmantojot attālās darbvirsmas pakalpojumus (Remote Desktop Services — RDS), iepriekš nosaukti termināļa pakalpojumi:

- Jums jābūt Microsoft 365 For Business plānam vai Office 365 plānam, kurā ietilpst Microsoft 365 programmas lieluzņēmumiem, piemēram, Office 365 Enterprise E3 vai Enterprise E5.
   > [!NOTE]
   > Microsoft 365 programmas darbam un Microsoft 365 Business Standard plānos nav iekļauti Microsoft 365 programmas lieluzņēmumiem.
- Iespējojiet koplietojamā [datora aktivizāciju.](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation)

> [!NOTE]
> Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgs,](https://aka.ms/SaRA_OfficeSCA_M365Portal) lai instalētu Microsoft 365 programmas lieluzņēmumiem koplietojamā datora aktivizācijas režīmā.

Papildinformāciju par priekšnosacījumiem, iestatīšanas norādījumiem un norādījumiem par pielāgotām instalācijām, izmantojot Office izvietošanas rīku, skatiet rakstā [Microsoft 365 programmas lieluzņēmumiem izvietošana, izmantojot attālās darbvirsmas pakalpojumus.](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services)

Lai novērstu ar koplietojama datora aktivizēšanu saistītas kļūdas:

- Skatiet [rakstu Problēmu novēršana saistībā ar koplietojama datora aktivizēšanu Microsoft 365 programmas lieluzņēmumiem](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Skatiet rakstu [Atiestatīt Microsoft 365 programmas uzņēmumam aktivizēšanas statusam](https://go.microsoft.com/fwlink/?linkid=2109218).

Ja vēlaties instalēt ierīces Microsoft 365 programmas lieluzņēmumiem RDS no ierīces Microsoft 365 administrēšanas centrs, kas izmanto noklusējuma instalēšanas ***iestatījumus,*** veiciet tālāk norādītās darbības.

1. Pārbaudiet, kādu abonementu izmantojat. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).
2. Ja nepieciešams, pārslēdzieties uz citu abonementu. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan).
3. Ja Office jau ir instalēta RDS serverī, izmantojot jebkuru citu Microsoft abonementu, atinstalējiet to. Piemēram, dodoties uz **Vadības**  >  **panelis; atinstalējiet programmu**. Ja rodas [problēmas, atinstalējiet](https://aka.ms/SARA-OfficeUninstall-Alchemy) atbalsta un atkopšanas palīgs Microsoft atbalsta un atkopšanas palīgs.
4. RDS serverī pierakstieties e-pasta Microsoft 365 administrēšanas centrs ar savu administratora kontu un [instalējiet Microsoft 365 programmas lieluzņēmumiem](https://portal.office.com/OLS/MySoftware.aspx).
5. Pēc Office instalēšanas ***neatveriet lietojumprogrammas un nepiesakieties*** jebkurā Office programmā.
6. RDS serverī iespējojiet koplietojama datora aktivizēšanu, rediģējot reģistru, veicot tālāk norādītās darbības.
   1. Ar peles labo pogu Windows pogu ekrāna apakšējā kreisajā stūrī un atlasiet **Palaist**. Lodziņā Atvērt ierakstiet **regedit un pēc** tam atlasiet **Labi**.
   2. Kad **saņemat** aicinājumu atļaut reģistra redaktoram veikt izmaiņas ierīcē, atlasiet Jā.
   3. Reģistra redaktorā pievienojiet virknes **vērtību SharedComputerlicensing** ar iestatījumu 1 sadaļā HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS serverī pierakstieties kā ***lietotājs*** un pārliecinieties, vai koplietojama datora aktivizēšana [ir iespējota lietošanai Microsoft 365 programmas lieluzņēmumiem.](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded)
