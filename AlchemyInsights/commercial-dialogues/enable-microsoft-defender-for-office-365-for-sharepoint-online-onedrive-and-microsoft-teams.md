---
title: Pielikumu Seifs iespējošana programmā SharePoint Online, OneDrive un Microsoft Teams
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
ms.openlocfilehash: 7357f53ef7827aea9cbb0d222c338a5edf429ffd201bfbb6d7307b3d446fdae2
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57894470"
---
# <a name="enable-safe-attachments-for-sharepoint-online-onedrive-and-microsoft-teams"></a>Pielikumu Seifs iespējošana programmā SharePoint Online, OneDrive un Microsoft Teams

1. Izmantojot globālā administratora vai drošības administratora akreditācijas datus, atveriet Microsoft 365 Defender portālu vietnē un pēc tam dodieties uz Politikas & kārtulas Apdraudējumu Seifs politikas Seifs pielikumiem <https://security.microsoft.com>  \>  \>  **sadaļā** Politikas

   Lai pārietu tieši uz **lapu Seifs Pielikumi,** izmantojiet <https://security.microsoft.com/safeattachmentv2> .

2. Lapā **Pielikumi Seifs uz** **Globālie iestatījumi**.
3. Parādītā izlidošanas logā atlasiet Opciju Ieslēgt Microsoft Defender programmatūrai **Office 365 SharePoint, OneDrive u.Microsoft Teams** un pēc tam atlasiet **Saglabāt**.

    > [!TIP]
    >
    > Veiciet tālāk norādītās darbības, lai uzlabotu Seifs, kā tiek SharePoint, OneDrive un Microsoft Teams:
    >
    > - Lai neļautu lietotājiem lejupielādēt ļaunprātīgus failus, izmantojiet parametra `$true` *DisallowInfectedFileDownload* vērtību **[cmdlet Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant)** SharePoint Online PowerShell. Papildinformāciju skatiet [rakstā SharePoint Online PowerShell izmantošana, lai neļautu lietotājiem lejupielādēt ļaunprātīgus failus.](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-2-recommended-use-sharepoint-online-powershell-to-prevent-users-from-downloading-malicious-files)
    > - [Brīdinājuma politikas izveide konstatētajiem failiem](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-mdo-for-spo-odb-and-teams#step-3-recommended-use-the-microsoft-365-defender-portal-to-create-an-alert-policy-for-detected-files)

Papildinformāciju skatiet [rakstā Seifs Office 365, SharePoint, OneDrive un Microsoft Teams.](https://go.microsoft.com/fwlink/?linkid=2092041)
