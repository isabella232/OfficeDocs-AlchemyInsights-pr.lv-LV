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
ms.openlocfilehash: 564a7f1f6a37e64dbd7d679878ebadbbe35f3fa0
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44506925"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Iespējot Office 365 uzlabotā Pretdraudu aizsardzība SharePoint Online, OneDrive un Microsoft Teams

1. Dodieties uz https://protection.office.com un pierakstieties.
2. Izvēlieties **draudu pārvaldības**  >  **politiku**  >  **droši pielikumi**.
3. Atlasiet **Ieslēgt ATP darbam ar SharePoint, OneDrive un Microsoft Teams**un pēc tam noklikšķiniet uz **saglabāt**.
4. Ieteicams Kā globālo administratoru vai SharePoint Online administrators, palaidiet [Set Sponomnieka](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet ar **Disallowinfectedfiledownload** parametrs ir iestatīts uz *True*.
5. Ieteicams [Iestatītu brīdinājumus](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) noteiktajiem failiem.

> [!NOTE]
> ATP būs NTO skenēt katru failu SharePoint Online, OneDrive vai Microsoft Teams. Faili tiek skenēti asinhroni, izmantojot procesu, kurā tiek izmantoti koplietošanas un viesu aktivitāšu notikumi, kā arī viedā heiristika un draudu signāli, lai identificētu ļaunprātīgus failus. Skatiet [ATP for SharePoint, OneDrive un Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).