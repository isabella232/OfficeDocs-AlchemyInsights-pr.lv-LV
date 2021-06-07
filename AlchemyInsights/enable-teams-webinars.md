---
title: Iespējot Teams webinars
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
- "11513"
- "9006672"
ms.openlocfilehash: 5a732e6746e9fd23e54a0b2ffeabb59623012a0e
ms.sourcegitcommit: 9de78b30602f917d58705057cdcce31fec349969
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/04/2021
ms.locfileid: "52793786"
---
# <a name="enable-teams-webinars"></a>Iespējot Teams webinars

Lietojumprogrammu lietojumprogrammas ir iespējotas pēc noklusējuma. Izmantojot PowerShell komandas, varat Teams, lai pārvaldītu, kuras personas Teams jūsu webinars.

- Visi lietotāji, kas var izveidot sapulci, var arī izveidot tīmekļa semināra sapulci. Ja vēlaties pārvaldīt to, kuras personas var Teams Webinars, izmantojiet *AllowMeetingRegistration*. 
- Pēc noklusējuma *WhoCanRegister ir* iespējots un iestatīts uz **Everyone**. Ja vēlaties izslēgt sapulces reģistrāciju, iestatiet *AllowMeetingRegistration* vērtību **False**.

Lai mainītu šos iestatījumus, ir [jāinstalē Teams PowerShell.](/microsoftteams/teams-powershell-install) Tāpat sapulču politikas ir ieviestas Teams tīmeklī. Piemēram, ja sapulces iestatījumos ir izslēgta anonīma pievienošanās, anonīmi lietotāji nevar pievienoties tīmekļa semināriem.

Papildinformāciju par to, kā konfigurēt, kuras personas var reģistrēties tīmeklim, skatiet rakstā To personu konfigurēšana, [kas var reģistrēties tīmekļa semināriem.](/microsoftteams/set-up-webinars?source=docs#configure-who-can-register-for-webinars) Papildinformāciju par Microsoft sarakstu iestatījumiem skatiet rakstā [Microsoft sarakstu vadības iestatījumi.](/sharepoint/control-lists)