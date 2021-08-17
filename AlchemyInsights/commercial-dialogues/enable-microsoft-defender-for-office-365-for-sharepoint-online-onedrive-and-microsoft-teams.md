---
title: Microsoft Defender iespējošana programmatūrai Office 365 SharePoint Online, OneDrive un Microsoft Teams
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
ms.openlocfilehash: db79c1d79ddb9bc92f0601ac156e5e41a8ab83cd603556f191d5491cdd5ae2a3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54058873"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Microsoft Defender iespējošana programmatūrai Office 365 SharePoint Online, OneDrive un Microsoft Teams

1. Izmantojot globālā administratora vai drošības administratora akreditācijas datus, piesakieties [Office 365 un atbilstības centrā](https://protection.office.com/).
2. Kreisajā **rūtī atlasiet** Apdraudējumu pārvaldība un pēc tam atlasiet **Politika**  >  [Seifs pielikumiem](https://protection.office.com/safeattachment).
3. Atlasiet **Ieslēgt Microsoft Defender programmatūrai Office 365, SharePoint, OneDrive un Microsoft Teams**, un pēc tam atlasiet **Saglabāt**.
    > [!TIP]
    >
    > - Kā globālais administrators vai SharePoint Online administrators, izpildiet šādu PowerShell cmdlet ar parametra **DisallowInfectedFileDownload** vērtību *kā true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)
    > - [Brīdinājumu iestatīšana konstatētajiem failiem](https://go.microsoft.com/fwlink/?linkid=2092110)

Papildinformāciju skatiet rakstā [Programmatūrai Office 365 Microsoft Defender SharePoint, OneDrive un Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
