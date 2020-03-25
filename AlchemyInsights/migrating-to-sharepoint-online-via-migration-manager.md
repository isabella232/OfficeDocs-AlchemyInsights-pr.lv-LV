---
title: Migrēšana uz SharePoint Online, izmantojot migrācijas pārvaldnieku
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
- "3192"
ms.openlocfilehash: 5aebf7903670e74f616c8f151749d760caf1d642
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932185"
---
# <a name="migrating-to-sharepoint-online-via-migration-manager"></a><span data-ttu-id="aa311-102">Migrēšana uz SharePoint Online, izmantojot migrācijas pārvaldnieku</span><span class="sxs-lookup"><span data-stu-id="aa311-102">Migrating to SharePoint Online via Migration Manager</span></span>

<span data-ttu-id="aa311-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti izmanto uzņēmumam kritiski svarīgas lietojumprogrammas pakalpojumā, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="aa311-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="aa311-104">Tostarp satura migrēšanu, datu zuduma novēršanu (DLP) un dublējumkopiju izveides risinājumus.</span><span class="sxs-lookup"><span data-stu-id="aa311-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="aa311-105">Šajos bezprecedenta laikos mēs veicam pasākumus, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri, strādājot attālināti, vairāk nekā jebkad agrāk ir atkarīgi no šī pakalpojuma.</span><span class="sxs-lookup"><span data-stu-id="aa311-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="aa311-106">Šī mērķa atbalstam esam ieviesuši stingrākus ierobežojumus fona lietojumprogrammām (migrēšana, DLP un dublējumkopiju izveides risinājumi) darbdienu dienas stundās.</span><span class="sxs-lookup"><span data-stu-id="aa311-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="aa311-107">Paredzams, ka šo lietojumprogrammu caurlaidspēja šajā laikā būs ļoti ierobežota.</span><span class="sxs-lookup"><span data-stu-id="aa311-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="aa311-108">Tomēr vakara un nedēļas nogales stundās reģionā pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu daudzumu no fona lietojumprogrammām.</span><span class="sxs-lookup"><span data-stu-id="aa311-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="aa311-109">**Migrācijas pārvaldnieks**</span><span class="sxs-lookup"><span data-stu-id="aa311-109">**Migration Manager**</span></span>

<span data-ttu-id="aa311-110">Migrācijas pārvaldnieks, kas atrodas modernajā SharePoint administrēšanas centrā, sniedz norādījumus par klientu iestatīšanu un uzdevumu izveidi.</span><span class="sxs-lookup"><span data-stu-id="aa311-110">Located in the modern SharePoint Admin Center, the Migration Manager guides you through the setup of your clients and the creation of your tasks.</span></span> <span data-ttu-id="aa311-111">Varat norādīt globālos vai uzdevuma līmeņa iestatījumus, apskatīt visu darbību gaitu un lejupielādēt apkopotu kopsavilkumu un uzdevuma līmeņa pārskatus.</span><span class="sxs-lookup"><span data-stu-id="aa311-111">You can specify global or task-level settings, view all-up task progress, and download aggregated summary and task-level reports.</span></span>

- [<span data-ttu-id="aa311-112">Darba sākšana ar migrācijas pārvaldnieku</span><span class="sxs-lookup"><span data-stu-id="aa311-112">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="aa311-113">Migrēšanas pārvaldnieka klientu iestatīšana</span><span class="sxs-lookup"><span data-stu-id="aa311-113">Setup Migration Manager clients</span></span>](https://docs.microsoft.com/sharepointmigration/mm-setup-clients)

- [<span data-ttu-id="aa311-114">Migrācijas pārvaldnieka iestatījumi</span><span class="sxs-lookup"><span data-stu-id="aa311-114">Migration Manager Settings</span></span>](https://docs.microsoft.com/sharepointmigration/mm-settings)
