---
title: Koplietojamu Microsoft 365 programmas lieluzņēmumiem izvietošanai RDS, Terminal Server vai VDI
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
ms.openlocfilehash: 9d928a3bf58dedc3aaf231c8a051f87b0bbdf438
ms.sourcegitcommit: 391052026a6ce7646926d233d0fd9ba135088f79
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/01/2021
ms.locfileid: "60041013"
---
# <a name="deploying-microsoft-365-apps-for-enterprise-for-shared-use-on-rds-terminal-server-or-vdi"></a>Koplietojamu Microsoft 365 programmas lieluzņēmumiem izvietošanai RDS, Terminal Server vai VDI

Lai izvietotu Microsoft 365 programmas, izmantojot attālās darbvirsmas pakalpojumus (Remote Desktop Services — RDS), iepriekš termināļa pakalpojumi, ir:

- Izmantojiet vienkāršo labojumu, lai iespējotu TLS 1.2 kā noklusējumu, ja lietojat vecāku Windows versiju (piemēram, Windows 7 SP1, Windows Server 2008 R2). Vienkāršo labojumu un papildinformāciju skatiet rakstā Atjaunināšana, lai [iespējotu TLS 1.1 un TLS 1.2 kā noklusējuma drošos protokolus winhttp Windows.](https://support.microsoft.com/en-us/topic/update-to-enable-tls-1-1-and-tls-1-2-as-default-secure-protocols-in-winhttp-in-windows-c4bd73d2-31d7-761e-0178-11268bb10392#bkmk_easy) 
- Ir plāns, kurā ietilpst Microsoft 365 programmas lieluzņēmumiem (iepriekš Office 365 Plus). Piemēram, Office 365 E3 vai Microsoft 365 E5, vai jebkurš plāns, kurā ietilpst Project vai Visio datora versija, piemēram, Project 3. plāns vai Visio 2. plāns, vai Microsoft 365 Business Premium plāns, kurā ir iekļautas arī Microsoft 365 programmas darbam.
- Iespējot koplietojama datora aktivizēšanu. Papildinformāciju skatiet rakstā [Koplietojamā datora aktivizēšanas pārskats Microsoft 365 programmas.](https://docs.microsoft.com/deployoffice/overview-shared-computer-activation)

**Piezīme.** Lai Microsoft 365 programmas koplietojama datora aktivizācijas režīmā, lejupielādējiet un palaidiet [Microsoft atbalsta un atkopšanas palīgs](https://docs.microsoft.com/alchemyinsights/deploy-o365-remotely-to-rds). Detalizētu informāciju par priekšnosacījumiem, iestatīšanas norādījumiem un norādījumiem par instalāciju pielāgošanas, izmantojot Office izvietošanas rīku, skatiet rakstā [Microsoft 365 programmas izvietošana, izmantojot attālās darbvirsmas pakalpojumus.](https://docs.microsoft.com/deployoffice/deploy-microsoft-365-apps-remote-desktop-services)

Lai novērstu ar koplietojama datora aktivizēšanu saistītas kļūdas, skatiet rakstu:

- [Problēmu novēršana saistībā ar koplietojama datora aktivizāciju Microsoft 365 programmas](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation)
- [Aktivizācijas Microsoft 365 programmas lieluzņēmumiem atiestatīšana](https://docs.microsoft.com/office/troubleshoot/activation/reset-office-365-proplus-activation-state)

Ja vēlaties instalēt atjauninājumu Microsoft 365 programmas RDS no ierīces Microsoft 365 administrēšanas centrs, kas izmanto noklusējuma instalācijas iestatījumus, veiciet tālāk norādītās darbības.

1. Pārbaudiet Microsoft 365 savu plānu. Papildinformāciju skatiet rakstā [Kāds abonements man ir?](https://docs.microsoft.com/microsoft-365/admin/admin-overview/what-subscription-do-i-have).

1. Ja nepieciešams, pārslēdzieties uz citu Microsoft 365 plānu. Papildinformāciju skatiet [rakstā Jaunināšana uz citu plānu](https://docs.microsoft.com/microsoft-365/commerce/subscriptions/upgrade-to-different-plan).

1. Ja Microsoft 365 programmas jau ir instalēta RDS serverī, izmantojot citus nesaderīgus plānus, atinstalējiet to, dodoties uz **vadības**  >  **paneli. Atinstalējiet programmu**. Ja rodas problēmas, atinstalējiet, lejupielādējot [Microsoft atbalsta un atkopšanas palīgs.](https://aka.ms/SARA-OfficeUninstall-Alchemy)

1. RDS serverī pierakstieties e-pasta Microsoft 365 administrēšanas centrs ar savu administratora kontu un [instalējiet Office](https://portal.office.com/OLS/MySoftware.aspx).

   Kad Office ir instalēta, neatveriet lietojumprogrammas un nepiesakieties jebkurā Office programmā.

1. RDS serverī iespējojiet koplietojamā datora aktivizēšanu, rediģējot reģistru:

   1. Ar peles labo Windows pogu ekrāna apakšējā kreisajā stūrī un atlasiet **Palaist**. Lodziņā Atvērt ierakstiet **regedit un pēc** tam atlasiet **Labi**.

   1. Kad parādās aicinājums atļaut reģistra redaktoram veikt izmaiņas jūsu ierīcē, atlasiet **Jā**.

   1. Reģistra redaktora sadaļā HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration pievienojiet virknes vērtību **SharedComputerLicensing** ar iestatījumu **1.**

1. RDS serverī pierakstieties kā lietotājs un pārliecinieties, vai koplietojama datora aktivizēšana ir iespējota Microsoft 365 programmas. 

   Detalizētu informāciju skatiet rakstā [Pārbaude, vai koplietojama datora aktivizēšana ir iespējota Microsoft 365 programmas](https://docs.microsoft.com/deployoffice/troubleshoot-shared-computer-activation#verify-that-shared-computer-activation-is-enabled-for-microsoft-365-apps).