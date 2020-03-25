---
title: SharePoint migrācijas veiktspēja
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "2700"
ms.openlocfilehash: 812444589d5a5bf766bbc6f466077d4ca829d79f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932241"
---
# <a name="sharepoint-migration-performance"></a><span data-ttu-id="4f8e7-102">SharePoint migrācijas veiktspēja</span><span class="sxs-lookup"><span data-stu-id="4f8e7-102">SharePoint migration performance</span></span>

<span data-ttu-id="4f8e7-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti izmanto uzņēmumam kritiski svarīgas lietojumprogrammas pakalpojumā, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="4f8e7-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="4f8e7-104">Tostarp satura migrēšanu, datu zuduma novēršanu (DLP) un dublējumkopiju izveides risinājumus.</span><span class="sxs-lookup"><span data-stu-id="4f8e7-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="4f8e7-105">Šajos bezprecedenta laikos mēs veicam pasākumus, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri, strādājot attālināti, vairāk nekā jebkad agrāk ir atkarīgi no šī pakalpojuma.</span><span class="sxs-lookup"><span data-stu-id="4f8e7-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="4f8e7-106">Šī mērķa atbalstam esam ieviesuši stingrākus ierobežojumus fona lietojumprogrammām (migrēšana, DLP un dublējumkopiju izveides risinājumi) darbdienu dienas stundās.</span><span class="sxs-lookup"><span data-stu-id="4f8e7-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="4f8e7-107">Paredzams, ka šo lietojumprogrammu caurlaidspēja šajā laikā būs ļoti ierobežota.</span><span class="sxs-lookup"><span data-stu-id="4f8e7-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="4f8e7-108">Tomēr vakara un nedēļas nogales stundās reģionā pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu daudzumu no fona lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="4f8e7-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="4f8e7-109">**Migrācijas veiktspēja**</span><span class="sxs-lookup"><span data-stu-id="4f8e7-109">**Migration performance**</span></span>

<span data-ttu-id="4f8e7-110">Migrēšanas veikšanu var ietekmēt tīkla infrastruktūra, failu izmēri, migrācijas laiks un ierobežošana.</span><span class="sxs-lookup"><span data-stu-id="4f8e7-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="4f8e7-111">Šo faktoru izpratne palīdzēs jums plānot un maksimāli efektīvi īstenot migrāciju.</span><span class="sxs-lookup"><span data-stu-id="4f8e7-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

<span data-ttu-id="4f8e7-112">Lai iegūtu papildinformāciju, lūdzu, apmeklējiet šo tālāk norādītās saites.</span><span class="sxs-lookup"><span data-stu-id="4f8e7-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="4f8e7-113">SharePoint Online un ODB migrācijas ātrums</span><span class="sxs-lookup"><span data-stu-id="4f8e7-113">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="4f8e7-114">Izvairīšanās no ierobežošanas vai bloķēšanas pakalpojumā SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="4f8e7-114">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="4f8e7-115">SharePoint migrācijas rīka lejupielāde un instalēšana</span><span class="sxs-lookup"><span data-stu-id="4f8e7-115">Download and install the SharePoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)
