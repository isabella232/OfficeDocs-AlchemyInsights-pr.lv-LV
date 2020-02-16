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
- "9000734"
- "2657"
ms.openlocfilehash: 509bd0c686830c04ed27f97372411677c0a7f4a4
ms.sourcegitcommit: 9aaa61d717e0fd475d2e9f0507c42aa40d073b5f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/15/2020
ms.locfileid: "42042851"
---
# <a name="manage-meeting-policies-in-microsoft-teams"></a>Sapulču politiku pārvaldīšana programmā Microsoft Teams

**Piezīme: politikas izmaiņām var būt nepieciešams līdz 24 stundām, lai tās stātos spēkā lietotājiem.** Iespējams, nevarēsit nekavējoties veikt izmaiņas jaunizveidotajā politikā; uzgaidiet 4 stundas un vēlreiz mēģiniet modificēt tikko izveidoto politiku.

Sapulču politikas tiek izmantotas, lai kontrolētu līdzekļus, kas ir pieejami sapulces dalībniekiem sapulcēs, kuras ieplānoja lietotāji jūsu organizācijā. Daži sapulču politikas līdzekļi, iespējams, nav ieviesti komandu administrēšanas centrā, tomēr (dokumentācijā tie ir apzīmēti ar "drīzumā"). Šajā gadījumā, vai, ja saņemat kļūdas, piemēram, "mēs nevaram atjaunināt politiku tūlīt, bet mēģināt vēlreiz vēlāk" Microsoft Teams administrēšanas centrs, ieteicams izmantot PowerShell, lai izveidotu vai modificētu grupas sapulču politiku. 

Lai iegūtu papildinformāciju par sapulču politiku, skatiet šādus resursus:

- Lai uzzinātu, kā izveidot politikas, veikt izmaiņas un piešķirt lietotājiem politiku, skatiet sadaļu [Sapulču politiku pārvaldīšana komandā](https://docs.microsoft.com/microsoftteams/meeting-policies-in-teams).

- Lai veiktu politikas izmaiņas, izmantojot PowerShell cmdlet, skatiet [Teams PowerShell pārskats](https://docs.microsoft.com/microsoftteams/teams-powershell-overview). 
    - Jums ir jāizmanto [Skype biznesa PowerShell modulis](https://www.microsoft.com/download/details.aspx?id=39366) grupas sapulču politiku. 
    - Pārskatiet [*-csteamsmeetingpolicy cmdlet dokumentāciju](https://docs.microsoft.com/search/?search=CsTeamsMeetingPolicy&view=skype-ps) , lai iegūtu papildinformāciju.

