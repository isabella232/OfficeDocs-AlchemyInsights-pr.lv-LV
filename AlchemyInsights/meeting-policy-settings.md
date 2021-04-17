---
title: Sapulces politikas iestatījumi
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000734"
- "2657"
ms.openlocfilehash: 39151d3a56cc09a8ae2dd77fb7bf1e99066cc77a
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51825450"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Sapulču politiku pārvaldība darbvietā Microsoft Teams

**Piezīme. Var paiet līdz pat 24 stundām, līdz politikas izmaiņas stājas spēkā lietotājiem.** Iespējams, uzreiz nevarēsit veikt izmaiņas jaunizveidotajā politikā. uzgaidiet 4 stundas un vēlreiz mēģiniet modificēt jaunizveidotu politiku.

Sapulču politikas tiek izmantotas, lai kontrolētu līdzekļus, kas pieejami sapulces dalībniekiem sapulcēm, kuras ir ieplānojis lietotājs jūsu organizācijā. Daži sapulču politiku līdzekļi, iespējams, vēl netiks ieviesti Teams administrēšanas centrā (dokumentācijā tie apzīmēti ar "drīzumā"). Šajā gadījumā vai, ja saņemat kļūdas ziņojumu, piemēram, "Mēs pašlaik nevaram atjaunināt politiku, bet vēlāk to mēģināt vēlreiz" Microsoft Teams administrēšanas centrā, mēs iesakām izmantot PowerShell, lai izveidotu vai modificētu Teams sapulču politikas. 

Papildinformāciju par sapulču politikām skatiet šādos resursos:

- Informāciju par to, kā izveidot politikas, veikt izmaiņas un piešķirt lietotājus politikai, skatiet rakstā [Sapulču politiku pārvaldība programmā Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Lai veiktu politikas izmaiņas, izmantojot PowerShell cmdlet, skatiet [rakstu Teams PowerShell pārskats.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Jums ir jāizmanto [Skype darbam PowerShell modulis Teams](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) sapulču politikām. 
    - [Papildinformāciju skatiet *-CsTeamsMeetingPolicy cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) dokumentācijā.

