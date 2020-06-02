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
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="4e4d8-102">Iespējot Office 365 uzlabotā Pretdraudu aizsardzība SharePoint Online, OneDrive un Microsoft Teams</span><span class="sxs-lookup"><span data-stu-id="4e4d8-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="4e4d8-103">Dodieties uz https://protection.office.com un pierakstieties.</span><span class="sxs-lookup"><span data-stu-id="4e4d8-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="4e4d8-104">Izvēlieties **draudu pārvaldības**  >  **politiku**  >  **droši pielikumi**.</span><span class="sxs-lookup"><span data-stu-id="4e4d8-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="4e4d8-105">Atlasiet **Ieslēgt ATP darbam ar SharePoint, OneDrive un Microsoft Teams**un pēc tam noklikšķiniet uz **saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="4e4d8-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="4e4d8-106">Ieteicams Kā globālo administratoru vai SharePoint Online administrators, palaidiet [Set Sponomnieka](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet ar **Disallowinfectedfiledownload** parametrs ir iestatīts uz *True*.</span><span class="sxs-lookup"><span data-stu-id="4e4d8-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="4e4d8-107">Ieteicams [Iestatītu brīdinājumus](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) noteiktajiem failiem.</span><span class="sxs-lookup"><span data-stu-id="4e4d8-107">(Recommended) [Set up alerts](https://docs.microsoft.com/microsoft-365/security/office-365-security/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="4e4d8-108">ATP būs NTO skenēt katru failu SharePoint Online, OneDrive vai Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="4e4d8-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="4e4d8-109">Faili tiek skenēti asinhroni, izmantojot procesu, kurā tiek izmantoti koplietošanas un viesu aktivitāšu notikumi, kā arī viedā heiristika un draudu signāli, lai identificētu ļaunprātīgus failus.</span><span class="sxs-lookup"><span data-stu-id="4e4d8-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="4e4d8-110">Skatiet [ATP for SharePoint, OneDrive un Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="4e4d8-110">See [ATP for SharePoint, OneDrive, and Microsoft Teams](https://docs.microsoft.com/microsoft-365/security/office-365-security/atp-for-spo-odb-and-teams).</span></span>