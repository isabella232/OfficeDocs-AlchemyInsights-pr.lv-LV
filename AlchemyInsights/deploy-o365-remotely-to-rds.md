---
title: Izvietojot Office 365 ProPlus koplietojuma lietošanai RDS, termināļa serverī vai VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 12/9/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: 2312cca9ebf5dad1322bc98335cef6a6bc81f03e
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959466"
---
# <a name="deploying-office-365-proplus-for-shared-use-on-rds-terminal-server-or-vdi"></a>Izvietojot Office 365 ProPlus koplietojuma lietošanai RDS, termināļa serverī vai VDI

Lai izvietotu Office 365 ProPlus, izmantojot attālās darbvirsmas pakalpojumu (RDS), iepriekš nosaukto termināļa pakalpojumi:
- Jums ir jābūt Microsoft 365 biznesa plānu vai Office 365 plānu, kas ietver Office 365 ProPlus, piemēram, Office 365 Enterprise E3 vai Enterprise E5.
   > [!NOTE] 
   > Office 365 Business un Office 365 Business Premium plānos nav iekļauts Office 365 ProPlus.
- Ir jāiespējo [koplietojamā datora aktivizācija](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

> [!NOTE]
> Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA_OfficeSCA_M365Portal) , lai instalētu Office 365 ProPlus koplietojamā datora aktivizācijas režīmā.

Lai iegūtu papildinformāciju par priekšnosacījumiem, uzstādīšanas instrukcijas un norādījumus par pielāgotām instalācijām, izmantojot Office izvietošanas rīku, skatiet sadaļu [office 365 ProPlus izvietošana, izmantojot attālās darbvirsmas pakalpojumus](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).

Lai labotu kļūdas, kas saistītas ar koplietojamu datora aktivizāciju:
- Skatiet [problēmu novēršana saistībā ar Office 365 ProPlus koplietojamo datora aktivizāciju](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
- Skatiet sadaļu [Office 365 ProPlus aktivizācijas stāvokļa atiestatīšana](https://go.microsoft.com/fwlink/?linkid=2109218).

Ja vēlaties instalēt Office 365 ProPlus RDS no Microsoft 365 administrēšanas centrs, ***kas izmanto noklusējuma instalācijas iestatījumus***, rīkojieties šādi:

1.  Pārbaudiet, kādi Office 365 plānu jums ir. [Uzziniet, kā](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)to darīt.
2.  Ja nepieciešams, pārslēdzieties uz citu Office 365 plānu. [Uzziniet, kā](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)to darīt.
3.  Ja Office jau ir instalēta RDS serverī, izmantojot citus Office 365 plānus, atinstalējiet to. Piemēram, atverot **vadības paneli** > ,**atinstalējiet programmu**. Atinstalējiet, izmantojot [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ja rodas problēmas.
4.  Serverī RDS pierakstieties Microsoft 365 administrēšanas centrā, izmantojot administratora kontu, un [instalējiet Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).
5.  Pēc Office instalēšanas ***neatveriet vai pierakstieties*** nevienā no Office lietojumprogrammām.
6.  Serverī RDS iespējojiet koplietojamo datora aktivizāciju, rediģējot reģistru, veicot šādas darbības:
   1. Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna apakšējā kreisajā stūrī un atlasiet **palaist**. Lodziņā Atvērt ierakstiet **regedit**un pēc tam atlasiet **Labi**.
   2. Atlasiet **Jā** , kad tiek piedāvāts atļaut reģistra redaktoram veikt izmaiņas ierīcē.
   3. Reģistra redaktorā pievienojiet virknes vērtību **Sharedcomputerlicensing** ar iestatījumu 1 zem HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS serverī, ***pierakstieties kā lietotājs*** un [Pārbaudiet, vai ir iespējots Office 365 ProPlus koplietojamo datora aktivizācija](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

