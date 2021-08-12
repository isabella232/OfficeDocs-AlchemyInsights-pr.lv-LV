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
ms.openlocfilehash: 06395bcc1a631adeaa8abb5ad63b971639f226c19e48203078ba1097d43a50f8
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53925172"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Sapulču politiku pārvaldība programmā Microsoft Teams

**Piezīme. Var paiet līdz pat 24 stundām, līdz politikas izmaiņas stājas spēkā lietotājiem.** Iespējams, uzreiz nevarēsit veikt izmaiņas jaunizveidotajā politikā. uzgaidiet 4 stundas un vēlreiz mēģiniet modificēt jaunizveidotu politiku.

Sapulču politikas tiek izmantotas, lai kontrolētu līdzekļus, kas pieejami sapulces dalībniekiem sapulcēm, kuras ir ieplānojis lietotājs jūsu organizācijā. Daži sapulces politiku līdzekļi, iespējams, vēl netiek ieviesti Teams administrēšanas centrā (dokumentācijā tie apzīmēti ar "drīzumā"). Šajā gadījumā vai, ja saņemat kļūdas ziņojumu, piemēram, "Šobrīd nevaram atjaunināt politiku, bet vēlāk to mēģināt vēlreiz" Microsoft Teams administrēšanas centrā, ieteicams izmantot PowerShell, lai izveidotu vai modificētu Teams sapulču politikas. 

Papildinformāciju par sapulču politikām skatiet šādos resursos:

- Informāciju par to, kā izveidot politikas, veikt izmaiņas un piešķirt lietotājus politikai, skatiet rakstā [Sapulču politiku pārvaldība programmā Teams.](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams)

- Lai veiktu politikas izmaiņas, izmantojot PowerShell cmdlet, skatiet [Teams PowerShell pārskats.](https://docs.microsoft.com/microsoftteams/teams-powershell-overview) 
    - Lai lietotu sapulces Skype darbam, ir [jāizmanto Teams PowerShell](https://docs.microsoft.com/skypeforbusiness/set-up-your-computer-for-windows-powershell/download-and-install-the-skype-for-business-online-connector) modulis. 
    - [Papildinformāciju skatiet *-CsTeamsMeetingPolicy cmdlet](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) dokumentācijā.

