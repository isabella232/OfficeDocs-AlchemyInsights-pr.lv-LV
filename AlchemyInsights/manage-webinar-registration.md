---
title: Lietojumprogrammas semināra reģistrācijas pārvaldība
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11512"
- "9006672"
ms.openlocfilehash: c5b0721d286b07d7e0f84199885b6f527a2b42a2
ms.sourcegitcommit: f7a9e97d04b7b6cbb633b32094d40f1874bf0fce
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/06/2021
ms.locfileid: "52793915"
---
# <a name="manage-webinar-registration"></a>Lietojumprogrammas semināra reģistrācijas pārvaldība

Izmantojot Powershell komandas, varat Teams, lai pārvaldītu, Teams jūsu webinars. Lai instalētu Teams Powershell, skatiet [rakstu Teams PowerShell.](/microsoftteams/teams-powershell-install) 

Pēc noklusējuma *WhoCanRegister ir* iespējots un iestatīts uz **EveryoneInCompany.** Lai atļautu visiem, tostarp anonīmiem lietotājiem, reģistrēties, sapulces politika ir jāiestata kā **Ikviens,** izmantojot Powershell komandu:

`Set-CsTeamsMeetingPolicy -WhoCanRegister Everyone`

**Piezīme.** Ja sapulces iestatījumos ir izslēgta anonīma pievienošanās, anonīmi lietotāji nevar pievienoties tīmekļa semināriem. Papildinformāciju un šī iestatījuma iespējošanu skatiet [rakstā Sapulces iestatījumu pārvaldība programmā Microsoft Teams.](/microsoftteams/meeting-settings-in-teams)

Ja vēlaties izslēgt sapulces reģistrāciju, iestatiet *AllowMeetingRegistration* vērtību **False**.

Papildinformāciju par to, kā konfigurēt, kuras personas var reģistrēties tīmeklim, skatiet rakstā To personu konfigurēšana, [kas var reģistrēties tīmekļa semināriem.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Papildinformāciju par Microsoft sarakstu iestatījumiem skatiet rakstā [Microsoft sarakstu vadības iestatījumi.](/sharepoint/control-lists)
