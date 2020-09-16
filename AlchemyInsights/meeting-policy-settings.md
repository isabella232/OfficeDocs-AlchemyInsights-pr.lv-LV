---
title: Sapulču politikas iestatījumi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 683ca12c8f6e2511311c10ab5c4599ee66c08eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794341"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Sapulču politikas pārvaldība pakalpojumā Microsoft Teams

**Piezīme. lai politikas izmaiņas stātos spēkā lietotājiem, var paiet līdz pat 24 stundām.** Jūs, iespējams, nevarēsit tūlīt veikt izmaiņas jaunizveidotās politikās; uzgaidiet 4 stundas un vēlreiz mēģiniet modificēt jaunizveidoto politiku.

Sapulču politikas tiek lietotas, lai kontrolētu dalībniekiem pieejamos līdzekļus sapulcēm, ko ieplānojuši lietotāji jūsu organizācijā. Daži sapulču politiku līdzekļi, iespējams, vēl nav implementēti grupu administrēšanas centrā (šeit ir atzīmēti "drīzumā"). Šajā gadījumā, vai, ja saņemat kļūdas ziņojumu, kas līdzīgs "pašlaik nevar atjaunināt politiku, bet vēlāk mēģiniet vēlreiz" Microsoft Teams administrēšanas centrā, iesakām izmantot PowerShell, lai izveidotu vai modificētu grupu sapulču politikas. 

Papildinformāciju par sapulču politikām skatiet šajos resursos:

- Lai uzzinātu, kā izveidot politikas, veikt izmaiņas un piešķirt lietotājus politikai, skatiet rakstu [Sapulču politiku pārvaldība pakalpojumā Teams](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Lai veiktu politikas izmaiņas, izmantojot PowerShell cmdlet, skatiet rakstu [Teams PowerShell pārskats](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Jums ir jāizmanto [Skype darbam PowerShell modulis](https://www.microsoft.com/download/details.aspx?id=39366) grupu sapulču politikām. 
    - Lai iegūtu papildinformāciju, pārskatiet [*-CsTeamsMeetingPolicy cmdlet dokumentāciju](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) .

