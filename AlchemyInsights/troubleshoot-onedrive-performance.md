---
title: OneDrive veiktspējas problēmu novēršana
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1977"
- "9000343"
ms.openlocfilehash: 4699f6113acd70b4778f9feeaeec012ff8fdd63f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47757892"
---
# <a name="troubleshoot-onedrive-performance"></a><span data-ttu-id="e5ffd-102">OneDrive veiktspējas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="e5ffd-102">Troubleshoot OneDrive performance</span></span>

<span data-ttu-id="e5ffd-103">Ja rodas lēnāka nekā gaidītā sinhronizācija vai līdzīgas veiktspējas problēmas ar OneDrive:</span><span class="sxs-lookup"><span data-stu-id="e5ffd-103">If you’re experiencing a slower than expected sync, or similar performance issues with OneDrive:</span></span>

- <span data-ttu-id="e5ffd-104">Apstipriniet, ka nav nevienas zināmas problēmas, izmantojot [Pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home?ref=/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="e5ffd-104">Confirm there are no known issues using the [Service Health Dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth).</span></span>

- <span data-ttu-id="e5ffd-105">[Iespējojiet failus pēc pieprasījuma](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) , lai jūs varētu piekļūt visiem saviem failiem pakalpojumā OneDrive, nelejupielādējot visus failus un izmantojot krātuves vietu savā ierīcē.</span><span class="sxs-lookup"><span data-stu-id="e5ffd-105">[Enable Files On Demand](https://support.office.com/article/save-disk-space-with-onedrive-files-on-demand-for-windows-10-0e6860d3-d9f3-4971-b321-7092438fb38e) so that you can access all your files in OneDrive without having to download all of them and use storage space on your device.</span></span>

- <span data-ttu-id="e5ffd-106">[Pārskatiet paraugpraksi](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) , lai veiktu tīkla plānošanu un veiktspēju.</span><span class="sxs-lookup"><span data-stu-id="e5ffd-106">[Review best practices](https://docs.microsoft.com/office365/enterprise/network-planning-and-performance) for network planning and performance.</span></span>

- <span data-ttu-id="e5ffd-107">[Maksimizējiet augšupielādes un lejupielādes ātrumu](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), it īpaši, ja ierīce tiek sinhronizēta pirmoreiz.</span><span class="sxs-lookup"><span data-stu-id="e5ffd-107">[Maximize upload and download speed](https://support.office.com/article/maximize-upload-and-download-speed-8eeadfb8-501f-406d-997b-98ab6ff67f43), especially if you’re syncing a device for the first time.</span></span>

- <span data-ttu-id="e5ffd-108">Ja sinhronizējat bibliotēku, kurā ir vairāk nekā 100 000 vienumu, OneDrive sinhronizācija var šķiet neilga ilgu laiku, vai arī statuss rāda, ka tiek apstrādāti 0KB no xMB.</span><span class="sxs-lookup"><span data-stu-id="e5ffd-108">If you’re syncing a library with more than 100,000 items, OneDrive sync may seem stuck for a long time, or the status shows Processing 0KB of xMB."</span></span> <span data-ttu-id="e5ffd-109">[Uzziniet vairāk par to, kā sinhronizēt vairāk nekā 100 000 failu](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) , kā arī [OneDrive atbalstīto 300 000 failu ierobežojumu](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span><span class="sxs-lookup"><span data-stu-id="e5ffd-109">[Learn more about syncing more than 100,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa) as well as [OneDrive’s supported limit of 300,000 files](https://support.office.com/article/invalid-file-names-and-file-types-in-onedrive-onedrive-for-business-and-sharepoint-64883a5d-228e-48f5-b3d2-eb39e07630fa).</span></span>

- <span data-ttu-id="e5ffd-110">Pēc tam, kad lietotājs ir pārsniedzis lietojuma ierobežojumus, SharePoint Online droselē papildu pieprasījumus no šī lietotāja konta uz neilgu laiku.</span><span class="sxs-lookup"><span data-stu-id="e5ffd-110">When a user exceeds usage limits, SharePoint Online throttles any further requests from that user account for a short period.</span></span> <span data-ttu-id="e5ffd-111">Kamēr droseļvārsta ir spēkā, visas lietotāju darbības tiek ierobežotas.</span><span class="sxs-lookup"><span data-stu-id="e5ffd-111">All user actions are throttled while the throttle is in effect.</span></span>
