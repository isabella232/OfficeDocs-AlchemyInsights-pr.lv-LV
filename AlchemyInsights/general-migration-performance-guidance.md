---
title: Vispārīgās migrācijas veikšanas vadlīnijas
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
- "3179"
ms.openlocfilehash: 10a0069c41d2e5128b2592425d815364a83b730f
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932485"
---
# <a name="general-migration-performance-guidance"></a><span data-ttu-id="9e8dd-102">Vispārīgās migrācijas veikšanas vadlīnijas</span><span class="sxs-lookup"><span data-stu-id="9e8dd-102">General migration performance guidance</span></span>

<span data-ttu-id="9e8dd-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti izmanto uzņēmumam kritiski svarīgas lietojumprogrammas pakalpojumā, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="9e8dd-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9e8dd-104">Tostarp satura migrēšanu, datu zuduma novēršanu (DLP) un dublējumkopiju izveides risinājumus.</span><span class="sxs-lookup"><span data-stu-id="9e8dd-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9e8dd-105">Šajos bezprecedenta laikos mēs veicam pasākumus, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri, strādājot attālināti, vairāk nekā jebkad agrāk ir atkarīgi no šī pakalpojuma.</span><span class="sxs-lookup"><span data-stu-id="9e8dd-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9e8dd-106">Šī mērķa atbalstam esam ieviesuši stingrākus ierobežojumus fona lietojumprogrammām (migrēšana, DLP un dublējumkopiju izveides risinājumi) darbdienu dienas stundās.</span><span class="sxs-lookup"><span data-stu-id="9e8dd-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9e8dd-107">Paredzams, ka šo lietojumprogrammu caurlaidspēja šajā laikā būs ļoti ierobežota.</span><span class="sxs-lookup"><span data-stu-id="9e8dd-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9e8dd-108">Tomēr vakara un nedēļas nogales stundās reģionā pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu daudzumu no fona lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="9e8dd-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9e8dd-109">**Migrācijas veikšanas vadlīnijas**</span><span class="sxs-lookup"><span data-stu-id="9e8dd-109">**Migration performance guidance**</span></span>

<span data-ttu-id="9e8dd-110">Migrēšanas veikšanu var ietekmēt tīkla infrastruktūra, failu izmēri, migrācijas laiks un ierobežošana.</span><span class="sxs-lookup"><span data-stu-id="9e8dd-110">Migration performance can be impacted by network infrastructure, file size, migration time, and throttling.</span></span> <span data-ttu-id="9e8dd-111">Šo faktoru izpratne palīdzēs jums plānot un maksimāli efektīvi īstenot migrāciju.</span><span class="sxs-lookup"><span data-stu-id="9e8dd-111">Understanding these will help you plan and maximize the efficiency of your migration.</span></span>

- [<span data-ttu-id="9e8dd-112">Vispārīgās migrācijas veikšanas vadlīnijas</span><span class="sxs-lookup"><span data-stu-id="9e8dd-112">General migration performance guidance</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)
