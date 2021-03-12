---
title: Iespējot Microsoft Defender pakalpojumam Office 365 pakalpojumam SharePoint Online, OneDrive un Microsoft Teams
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: 1c29afdcc52e7032fea22d698371677918665fa9
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745302"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Iespējot Microsoft Defender pakalpojumam Office 365 pakalpojumam SharePoint Online, OneDrive un Microsoft Teams

1. Izmantojot globālā administratora vai drošības administratora akreditācijas datus, piesakieties [Office 365 drošības un atbilstības centrā](https://protection.office.com/).
2. Kreisajā rūtī atlasiet **draudu pārvaldība** un pēc tam atlasiet **politikas**  >  [droši pielikumi](https://protection.office.com/safeattachment).
3. Atlasiet **ieslēgt Microsoft Defender pakalpojumam Office 365 darbam ar SharePoint, OneDrive un Microsoft Teams** un pēc tam atlasiet **Saglabāt**.
    > [!TIP]
    >
    > - Kā globālais administrators vai SharePoint Online administrators izpildiet tālāk norādīto PowerShell cmdlet ar **DisallowInfectedFileDownload** parametru kopu kā *patiess*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Noteiktu failu brīdinājumu iestatīšana](https://go.microsoft.com/fwlink/?linkid=2092110)

Lai iegūtu papildinformāciju, skatiet rakstu [Microsoft Defender for Office 365 for SharePoint, OneDrive un Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).
