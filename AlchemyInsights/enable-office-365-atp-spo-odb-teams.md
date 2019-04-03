---
title: Iespējotu Office 365 ATP SharePoint, OneDrive un grupu Microsoft
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 04/01/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Admin_O365
ms.custom: 3100021
ms.openlocfilehash: ae2f574663ae3233a056589c2d5a578171f3b2f4
ms.sourcegitcommit: 601aec31e6556286fe5e0fd62827a037cbb6fe17
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/02/2019
ms.locfileid: "31031022"
---
# <a name="enable-office-365-advanced-threat-protection-for-sharepoint-online-onedrive-and-microsoft-teams"></a><span data-ttu-id="2b600-102">Iespējotu Office SharePoint tiešsaistē, OneDrive un komandas Microsoft 365 papildu draudus aizsardzībai</span><span class="sxs-lookup"><span data-stu-id="2b600-102">Enable Office 365 Advanced Threat Protection for SharePoint Online, OneDrive, and Microsoft Teams</span></span>

1. <span data-ttu-id="2b600-103">Dodieties uz https://protection.office.com un pierakstieties.</span><span class="sxs-lookup"><span data-stu-id="2b600-103">Go to https://protection.office.com and sign in.</span></span>
2. <span data-ttu-id="2b600-104">Izvēlieties **draudu pārvaldības** > **politikas** > **Drošu pielikumu**.</span><span class="sxs-lookup"><span data-stu-id="2b600-104">Choose **Threat management** > **Policy** > **Safe Attachments**.</span></span>
3. <span data-ttu-id="2b600-105">Atlasiet **Ieslēgt ATP SharePoint, OneDrive, un Microsoft komandas**un pēc tam noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="2b600-105">Select **Turn on ATP for SharePoint, OneDrive, and Microsoft Teams**, and then click **Save**.</span></span>
4. <span data-ttu-id="2b600-106">(Ieteicams) Kā pasaules administrators vai SharePoint Online administrators, palaist [Set SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet ar parametru **DisallowInfectedFileDownload** , kas iestatīts uz *true*.</span><span class="sxs-lookup"><span data-stu-id="2b600-106">(Recommended) As a global administrator or a SharePoint Online administrator, run the [Set-SPOTenant](https://docs.microsoft.com/powershell/module/sharepoint-online/Set-SPOTenant?view=sharepoint-ps) cmdlet with the **DisallowInfectedFileDownload** parameter set to *true*.</span></span>
5. <span data-ttu-id="2b600-107">(Ieteicams) [Iestatīt brīdinājumus](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) noteiktajiem failiem.</span><span class="sxs-lookup"><span data-stu-id="2b600-107">(Recommended) [Set up alerts](https://docs.microsoft.com/office365/securitycompliance/turn-on-atp-for-spo-odb-and-teams#set-up-alerts-for-detected-files) for detected files.</span></span>

> [!NOTE]
> <span data-ttu-id="2b600-108">ATP būs nto skenēšanas ik viena faila SharePoint Online, OneDrive vai Microsoft Teams.</span><span class="sxs-lookup"><span data-stu-id="2b600-108">ATP will nto scan every single file in SharePoint Online, OneDrive, or Microsoft Teams.</span></span> <span data-ttu-id="2b600-109">Faili tiek skenēti asinhroni, caur procesu, kas izmanto koplietošanas un viesu aktivitāti notikumi kopā ar gudru heiristiku un draudu signālus identificēt ļaunprātīgu failus.</span><span class="sxs-lookup"><span data-stu-id="2b600-109">Files are scanned asynchronously, through a process that uses sharing and guest activity events, along with smart heuristics and threat signals to identify malicious files.</span></span> <span data-ttu-id="2b600-110">Sk. [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span><span class="sxs-lookup"><span data-stu-id="2b600-110">See [https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams](https://docs.microsoft.com/office365/securitycompliance/atp-for-spo-odb-and-teams).</span></span>