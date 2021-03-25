---
title: Microsoft 365 lietojumprogrammu izvietošana uzņēmumam, lai to koplietotu, izmantojot RDS, Terminal Server vai VDI
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
ms.openlocfilehash: a57be7fcf9d8236a51dc4b38e33ad1c2ac717f11
ms.sourcegitcommit: 2eab0980268e08a58014459d44a08a1cc34a17d4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200680"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Microsoft 365 lietojumprogrammu izvietošana uzņēmumam, lai to koplietotu, izmantojot RDS, Terminal Server vai VDI

Lai izvietotu Microsoft 365 lietojumprogrammas darbam ar Enterprise, kas izmanto attālās darbvirsmas pakalpojumus (RDS), kas iepriekš nosaukta par termināļa pakalpojumiem:

- Jums ir nepieciešams Microsoft 365 for Business plāns vai Office 365 plāns, kurā iekļautas Microsoft 365 lietojumprogrammas darbam ar Enterprise, piemēram, Office 365 Enterprise E3 vai Enterprise E5.
   > [!NOTE]
   > Microsoft 365 programmās darbam un Microsoft 365 biznesa standarta plānos nav iekļautas Microsoft 365 lietojumprogrammas darbam ar Enterprise.
- Ir jāiespējo [koplietojamā datora aktivizēšana](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA_OfficeSCA_M365Portal) , lai instalētu Microsoft 365 lietojumprogrammas uzņēmumam koplietojamā datora aktivizēšanas režīmā.

Lai iegūtu papildinformāciju par priekšnosacījumiem, iestatīšanas instrukcijām un norādījumiem par pielāgotām instalācijām, izmantojot Office izvietošanas rīku, skatiet rakstu [Microsoft 365 lietojumprogrammu izvietošana uzņēmumam, izmantojot attālās darbvirsmas pakalpojumus](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Lai labotu ar koplietojamu datora aktivizāciju saistītās kļūdas:

- Skatiet rakstu [problēmu novēršana saistībā ar koplietojamu datora aktivizāciju attiecībā uz Microsoft 365 lietojumprogrammām darbam ar Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Skatiet rakstu [Atiestatīt Microsoft 365 programmas uzņēmumam aktivizēšanas statusam](https://go.microsoft.com/fwlink/?linkid=2109218).

Ja vēlaties instalēt Microsoft 365 lietojumprogrammas uzņēmumam RDS no Microsoft 365 administrēšanas centra, ***kas izmanto noklusējuma instalācijas iestatījumus***, veiciet tālāk norādītās darbības.

1. Pārbaudiet, kāds ir jūsu abonements. [Uzziniet, kā to](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)paveikt.
2. Ja nepieciešams, pārslēdzieties uz citu abonementu. [Uzziniet, kā to](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)paveikt.
3. Ja sistēma Office jau ir instalēta RDS serverī, izmantojot jebkurus citus Microsoft abonementus, atinstalējiet to. Piemēram, atverot **vadības paneļa**  >  **Atinstalēt programmu**. Ja rodas problēmas, atinstalējiet [, izmantojot Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SARA-OfficeUninstall-Alchemy) .
4. RDS serverī pierakstieties Microsoft 365 administrēšanas centrā ar administratora kontu un [instalējiet microsoft 365 lietojumprogrammas uzņēmumam Enterprise](https://portal.office.com/OLS/MySoftware.aspx).
5. Pēc Office instalēšanas ***neatveriet vai pierakstieties*** jebkurā Office lietojumprogrammā.
6. RDS serverī iespējojiet koplietotu datora aktivizāciju, rediģējot reģistru, veicot tālāk norādītās darbības.
   1. Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna apakšējā kreisajā stūrī un atlasiet **palaist**. Lodziņā Atvērt ierakstiet **regedit** un pēc tam atlasiet **Labi**.
   2. Atlasiet **Jā** , kad tiek parādīta uzvedne ar aicinājumu atļaut reģistra redaktoru veikt izmaiņas jūsu ierīcē.
   3. Reģistra redaktorā pievienojiet **SharedComputerLicensing** virknes vērtību ar iestatījumu 1 sadaļā HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS serverī ***pierakstieties kā lietotājs*** un [Pārbaudiet, vai koplietojamā datora aktivizācija ir iespējota Microsoft 365 lietojumprogrammām darbam ar Enterprise](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).
