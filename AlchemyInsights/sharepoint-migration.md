---
title: Opciju migrēšana uz SharePoint Online
ms.author: pebaum
author: v-miegge
manager: v-cojank
ms.date: 11/04/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: c8c339c9-2e50-4daa-aa91-3eb5053e2bc6
ms.openlocfilehash: 830b39c51658cbc02f4be81acdfdf3b164a8df70
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932737"
---
# <a name="migrate-options-to-sharepoint-online"></a><span data-ttu-id="66476-102">Opciju migrēšana uz SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="66476-102">Migrate options to SharePoint Online</span></span>

<span data-ttu-id="66476-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="66476-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="66476-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="66476-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="66476-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="66476-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="66476-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="66476-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="66476-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="66476-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="66476-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="66476-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="66476-109">**Migrācijas opcijas**</span><span class="sxs-lookup"><span data-stu-id="66476-109">**Migration options**</span></span>

<span data-ttu-id="66476-110">Ir dažādas iespējas migrēt saturu uz SharePoint Online, atkarībā no lieluma un daudzuma failus, kas jums ir nepieciešams, lai pārvietotos, lūdzu, skatiet sarakstu ar iespējām, kas [atrodas šeit](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="66476-110">There are different options available to migrate content to SharePoint Online, depending on the size and quantity of files you need to move, please see a list of options [located here](https://docs.microsoft.com/sharepointmigration/migrate-to-sharepoint-online).</span></span>

<span data-ttu-id="66476-111">Lai iegūtu plašāku informāciju par satura migrāciju, lūdzu, apmeklējiet tālāk norādītās saites.</span><span class="sxs-lookup"><span data-stu-id="66476-111">For more information on content migration, please visit the links below.</span></span>

- [<span data-ttu-id="66476-112">SharePoint migrācijas rīks</span><span class="sxs-lookup"><span data-stu-id="66476-112">Sharepoint Migration Tool</span></span>](https://docs.microsoft.com/sharepointmigration/introducing-the-sharepoint-migration-tool)

- [<span data-ttu-id="66476-113">Sākt darbu ar migrācijas pārvaldnieku</span><span class="sxs-lookup"><span data-stu-id="66476-113">Get started with the Migration Manager</span></span>](https://docs.microsoft.com/sharepointmigration/mm-get-started)

- [<span data-ttu-id="66476-114">SharePoint Online un ODB migrācijas ātrums</span><span class="sxs-lookup"><span data-stu-id="66476-114">Sharepoint Online and ODB Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

- [<span data-ttu-id="66476-115">Izvairīties no ierobežotas vai bloķēts SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="66476-115">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="66476-116">SharePoint migrācijas novērtēšanas rīks (SMAT)</span><span class="sxs-lookup"><span data-stu-id="66476-116">SharePoint Migration Assessment Tool (SMAT)</span></span>](https://www.microsoft.com/download/details.aspx?id=53598&amp;751be11f-ede8-5a0c-058c-2ee190a24fa6=True)

<span data-ttu-id="66476-117">**Piezīme**: pašlaik SharePoint migrācijas rīks atbalsta tikai migrāciju SharePoint 2010 un 2013.</span><span class="sxs-lookup"><span data-stu-id="66476-117">**Note**: Currently the SharePoint Migration tool only support migrations from SharePoint 2010  and 2013.</span></span> <span data-ttu-id="66476-118">2016 versija vai 2019 pašlaik netiek atbalstīti.</span><span class="sxs-lookup"><span data-stu-id="66476-118">Version 2016 or 2019 are not supported at this time.</span></span>
