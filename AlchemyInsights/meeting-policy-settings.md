---
title: Sapulču politikas iestatījumi
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2657"
- "9000734"
ms.openlocfilehash: b5599c9974eb1c112835a9f42e4ebdc926071ea2
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/27/2019
ms.locfileid: "39627581"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Sapulču politiku pārvaldīšana programmā Microsoft Teams

Sapulču politikas tiek izmantotas, lai kontrolētu līdzekļus, kas ir pieejami sapulces dalībniekiem sapulcēs, kuras ieplānoja lietotāji jūsu organizācijā. Daži sapulču politikas līdzekļi, iespējams, nav ieviesti komandu administrēšanas centrā, tomēr (dokumentācijā tie ir apzīmēti ar "drīzumā"). Šajā gadījumā, vai, ja saņemat kļūdas, piemēram, "mēs nevaram atjaunināt politiku tūlīt, bet mēģināt vēlreiz vēlāk" Microsoft Teams administrēšanas centrs, ieteicams izmantot PowerShell, lai izveidotu vai modificētu grupas sapulču politiku. 

Lai iegūtu papildinformāciju par sapulču politiku, skatiet šādus resursus:

- Lai uzzinātu, kā izveidot politikas, veikt izmaiņas un piešķirt lietotājiem politiku, skatiet sadaļu [Sapulču politiku pārvaldīšana komandā](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Lai veiktu politikas izmaiņas, izmantojot PowerShell cmdlet, skatiet [Teams PowerShell pārskats](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Jums ir jāizmanto [Skype biznesa PowerShell modulis](https://www.microsoft.com/download/details.aspx?id=39366) grupas sapulču politiku. 
    - Pārskatiet [*-csteamsmeetingpolicy cmdlet dokumentāciju](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) , lai iegūtu papildinformāciju.

**Piezīme:** Politikas izmaiņām var būt nepieciešams līdz 24 stundām, lai tās stātos spēkā lietotājiem. Iespējams, nevarēsit nekavējoties veikt izmaiņas jaunizveidotajā politikā; uzgaidiet 4 stundas un vēlreiz mēģiniet modificēt tikko izveidoto politiku. Ja jums joprojām ir problēmas, mēģiniet PowerShell.  