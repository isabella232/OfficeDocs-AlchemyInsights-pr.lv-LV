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
ms.openlocfilehash: 51d1a66fdf9774bbe58bfdbe89317bc93834be09
ms.sourcegitcommit: 5e6a805fb0b41d714ca1cf90e23b8e2daa90f90e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/26/2019
ms.locfileid: "37205416"
---
# <a name="installing-office-on-a-terminal-server"></a>Office instalēšana termināļa serverī

Office 365 ProPlus izvietošanai Windows serverī, izmantojot attālās darbvirsmas pakalpojumus (RDS), iepriekš nosauktus termināļa pakalpojumus:
  
- Jums ir jābūt Office 365 plānu, kas ietver Office 365 ProPlus, piemēram, Office 365 Enterprise E3 vai Enterprise E5. Office 365 Business un Office 365 Business Premium plānos nav iekļauts Office 365 ProPlus.

- Ir jāiespējo [koplietojamā datora aktivizācija](https://docs.microsoft.com/DeployOffice/overview-of-shared-computer-activation-for-office-365-proplus).

Ja vēlaties instalēt Office 365 ProPlus RDS no Microsoft 365 administrēšanas centrs, ***kas izmanto noklusējuma instalācijas iestatījumus***, veiciet tālāk norādītās darbības.

> [!TIP]
> Varat arī lejupielādēt un palaist [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA_OfficeSCA_M365Portal) , lai instalētu Office 365 ProPlus koplietojamā datora aktivizācijas režīmā.
  
1. Pārbaudiet, kādi Office 365 plānu jums ir. [Uzziniet, kā](https://docs.microsoft.com/office365/admin/admin-overview/what-subscription-do-i-have)

2. Ja nepieciešams, pārslēdzieties uz citu Office 365 plānu. [Uzziniet, kā](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/switch-to-a-different-plan)

3. Ja Office jau ir instalēta RDS serverī, izmantojot citus Office 365 plānus, atinstalējiet to. Piemēram, atverot vadības paneli \> , atinstalējiet programmu. Atinstalējiet, izmantojot [Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SARA-OfficeUninstall-Alchemy) , ja rodas problēmas.

4. Serverī RDS pierakstieties Microsoft 365 administrēšanas centrā, izmantojot administratora kontu, un [instalējiet Office 365 ProPlus](https://portal.office.com/OLS/MySoftware.aspx).

5. Pēc Office instalēšanas ***neatveriet vai pierakstieties*** nevienā no Office lietojumprogrammām.

6. Serverī RDS iespējojiet koplietojamo datora aktivizāciju, rediģējot reģistru, veicot šādas darbības:

1. Ar peles labo pogu noklikšķiniet uz Windows pogas ekrāna kreisajā apakšējā stūrī un atlasiet palaist. Lodziņā Atvērt ierakstiet **regedit**un pēc tam atlasiet Labi.

2. Atlasiet Jā, kad tiek piedāvāts atļaut reģistra redaktoram veikt izmaiņas ierīcē.

3. Reģistra redaktorā pievienojiet virknes vērtību **Sharedcomputerlicensing** ar iestatījumu 1 zem HKEY_LOCAL_MACHINE\SOFTWARE\Microsoft \Office\ClickToRun\Configuration.

7. RDS serverī, ***pierakstieties kā lietotājs*** un [Pārbaudiet, vai ir iespējots Office 365 ProPlus koplietojamo datora aktivizācija](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus#verify-that-activation-for-office-365-proplus-succeeded).

Lai iegūtu papildinformāciju par priekšnosacījumi, uzstādīšanas instrukcijas un norādījumus par pielāgoto instalāciju, izmantojot Office izvietošanas rīks, lūdzu, skatiet [izvietot office 365 ProPlus, izmantojot attālās darbvirsmas pakalpojumu](https://docs.microsoft.com/DeployOffice/deploy-office-365-proplus-by-using-remote-desktop-services).
  
Lai labotu kļūdas, kas saistītas ar koplietojamu datora aktivizāciju, lūdzu, skatiet [problēmu novēršana saistībā ar Office 365 ProPlus koplietojamo datora aktivizāciju](https://docs.microsoft.com/DeployOffice/troubleshoot-issues-with-shared-computer-activation-for-office-365-proplus).
  