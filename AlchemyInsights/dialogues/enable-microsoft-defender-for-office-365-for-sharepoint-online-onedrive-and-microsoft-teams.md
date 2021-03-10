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
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694045"
---
# <a name="enable-microsoft-defender-for-office-365-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="19a92-102">Iespējot Microsoft Defender pakalpojumam Office 365 pakalpojumam SharePoint Online, OneDrive un Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="19a92-102">Enable Microsoft Defender for Office 365 for SharePoint Online, OneDrive and Microsoft Teams</span></span>

1. <span data-ttu-id="19a92-103">Izmantojot globālā administratora vai drošības administratora akreditācijas datus, piesakieties [Office 365 drošības un atbilstības centrā](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="19a92-103">Using your global admin or security admin credentials, log in to the [Office 365 Security and Compliance Center](https://protection.office.com/).</span></span>
2. <span data-ttu-id="19a92-104">Kreisajā rūtī atlasiet **draudu pārvaldība** un pēc tam atlasiet **politikas**  >  [droši pielikumi](https://protection.office.com/safeattachment).</span><span class="sxs-lookup"><span data-stu-id="19a92-104">Select **Threat management** in the left pane, and then select **Policy** > [Safe attachments](https://protection.office.com/safeattachment).</span></span>
3. <span data-ttu-id="19a92-105">Atlasiet **ieslēgt Microsoft Defender pakalpojumam Office 365 darbam ar SharePoint, OneDrive un Microsoft Teams** un pēc tam atlasiet **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="19a92-105">Select **Turn on Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams**, and then select **Save**.</span></span>
    > [!TIP]
    >
    > - <span data-ttu-id="19a92-106">Kā globālais administrators vai SharePoint Online administrators izpildiet tālāk norādīto PowerShell cmdlet ar **DisallowInfectedFileDownload** parametru kopu kā *patiess*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span><span class="sxs-lookup"><span data-stu-id="19a92-106">As a global admin or a SharePoint Online admin, run the following PowerShell cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*: [Set-SPOTenant](https://go.microsoft.com/fwlink/?linkid=2092301)</span></span>
    > - [<span data-ttu-id="19a92-107">Noteiktu failu brīdinājumu iestatīšana</span><span class="sxs-lookup"><span data-stu-id="19a92-107">Set up alerts for detected files</span></span>](https://go.microsoft.com/fwlink/?linkid=2092110)

<span data-ttu-id="19a92-108">Lai iegūtu papildinformāciju, skatiet rakstu [Microsoft Defender for Office 365 for SharePoint, OneDrive un Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span><span class="sxs-lookup"><span data-stu-id="19a92-108">For more information, see [Microsoft Defender for Office 365 for SharePoint, OneDrive, and Microsoft Teams](https://go.microsoft.com/fwlink/?linkid=2092041).</span></span>
