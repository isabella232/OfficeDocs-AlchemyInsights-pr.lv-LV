---
title: Iespējot Office 365 ATP for SharePoint, OneDrive un Microsoft Teams
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: fdfdc97a198898051a3388672d01994d96dd5e97
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703433"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Iespējot Office 365 uzlabotā Pretdraudu aizsardzība SharePoint Online, OneDrive un Microsoft Teams

1. Dodieties uz https://protection.office.com un pierakstieties.
2. Izvēlieties **draudu pārvaldības** > **politiku** > **droši pielikumi**.
3. Atlasiet **Ieslēgt ATP darbam ar SharePoint, OneDrive un Microsoft Teams**un pēc tam noklikšķiniet uz **saglabāt**.
4. Ieteicams Kā globālo administratoru vai SharePoint Online administrators, palaidiet [Set Sponomnieka](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet ar **Disallowinfectedfiledownload** parametrs ir iestatīts uz *True*.
5. Ieteicams [Iestatītu brīdinājumus](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) noteiktajiem failiem.

> [!NOTE]
> ATP būs NTO skenēt katru failu SharePoint Online, OneDrive vai Microsoft Teams. Faili tiek skenēti asinhroni, izmantojot procesu, kurā tiek izmantoti koplietošanas un viesu aktivitāšu notikumi, kā arī viedā heiristika un draudu signāli, lai identificētu ļaunprātīgus failus. Redzēt [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).