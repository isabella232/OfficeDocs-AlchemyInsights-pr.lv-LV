---
title: Izvietojot Microsoft 365 Apps Enterprise koplietojamai izmantošanai RDS, termināļa serverī vai VDI
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001419"
- "3411"
ms.openlocfilehash: fe051cd1dac899dc9bb19d275c352ec6585b6a93
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44507593"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Izvietojot Microsoft 365 Apps Enterprise koplietojamai izmantošanai RDS, termināļa serverī vai VDI

Izvietot Microsoft 365 lietojumprogrammas uzņēmumiem, izmantojot attālās darbvirsmas pakalpojumu (RDS), iepriekš nosaukto termināļa pakalpojumi:
- Jums ir jābūt Microsoft 365 biznesa plānu vai Office 365 plānu, kas ietver Microsoft 365 lietojumprogrammas uzņēmumiem, piemēram, Office 365 Enterprise E3 vai Enterprise E5.
   > [!NOTE] 
   > Microsoft 365 lietojumprogrammas uzņēmumiem un Microsoft 365 Business Premium Standard plāniem neietver Microsoft 365 lietojumprogrammas uzņēmumiem.
- Ir jāiespējo [koplietojamā datora aktivizācija](https://docs.microsoft.com/DeployOffice/overview-shared-computer-activation).

> [!NOTE]
> Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA_OfficeSCA_M365Portal) , lai instalētu Microsoft 365 lietojumprogrammas Enterprise koplietojamo datoru aktivizācijas režīmā.

Lai iegūtu papildinformāciju par priekšnosacījumi, uzstādīšanas instrukcijas un norādījumus par pielāgoto instalāciju, izmantojot Office izvietošanas rīks, skatiet [izvietot Microsoft 365 lietojumprogrammas Enterprise, izmantojot attālās darbvirsmas pakalpojumu](https://docs.microsoft.com/DeployOffice/deploy-microsoft-365-apps-remote-desktop-services).

Lai labotu kļūdas, kas saistītas ar koplietojamu datora aktivizāciju:
- Skatiet [problēmu novēršana saistībā ar koplietojamo datoru aktivizācija Microsoft 365 lietojumprogrammas uzņēmumiem](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation).
- Skatiet rakstu [Atiestatīt Microsoft 365 programmas uzņēmumam aktivizēšanas statusam](https://go.microsoft.com/fwlink/?linkid=2109218).

Ja vēlaties instalēt Microsoft 365 Apps Enterprise RDS no Microsoft 365 administrēšanas centrs, ***kas izmanto noklusējuma instalācijas iestatījumus***, rīkojieties šādi:

1.    Pārbaudiet, kāds abonements jums ir. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have)to darīt.
2.    Ja nepieciešams, pārslēdzieties uz citu abonementu. [Uzziniet, kā](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/switch-to-a-different-plan)to darīt.
3.    Ja Office jau ir instalēta RDS serverī, izmantojot citus Microsoft abonementus, atinstalējiet to. Piemēram, atverot **vadības paneli**,  >  **atinstalējiet programmu**. Atinstalējiet, izmantojot [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ja rodas problēmas.
4.    RDS serverī, pierakstieties Microsoft 365 administrēšanas centrs ar administratora kontu un [instalēt Microsoft 365 lietojumprogrammas uzņēmumiem](https://portal.office.com/OLS/MySoftware.aspx).
5.    Pēc Office instalēšanas ***neatveriet vai pierakstieties*** nevienā no Office lietojumprogrammām.
6.    Serverī RDS iespējojiet koplietojamo datora aktivizāciju, rediģējot reģistru, veicot šādas darbības:
   1. Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna apakšējā kreisajā stūrī un atlasiet **palaist**. Lodziņā Atvērt ierakstiet **regedit**un pēc tam atlasiet **Labi**.
   2. Atlasiet **Jā** , kad tiek piedāvāts atļaut reģistra redaktoram veikt izmaiņas ierīcē.
   3. Reģistra redaktorā pievienojiet virknes vērtību **Sharedcomputerlicensing** ar iestatījumu 1 zem HKEY_LOCAL_MACHINE \SOFTWARE\Microsoft \Office\ClickToRun\Configuration.
   4. RDS serverī, ***pierakstieties kā lietotājs*** un [Pārbaudiet, vai ir iespējota Microsoft 365 lietojumprogrammas uzņēmumiem koplietojamā datora aktivizācija](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation#verify-that-activation-for-microsoft-365-apps-succeeded).

