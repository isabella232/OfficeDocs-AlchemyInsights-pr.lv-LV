---
title: Problēmas, migrējot datus uz SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "5300030"
- "1885"
ms.openlocfilehash: b53a98480bab48497274c7358f7e606caa477f5a
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931701"
---
# <a name="issues-while-migrating-data-to-sharepoint-online"></a><span data-ttu-id="f6809-102">Problēmas, migrējot datus uz SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="f6809-102">Issues while migrating data to SharePoint Online</span></span>

<span data-ttu-id="f6809-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="f6809-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="f6809-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="f6809-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="f6809-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="f6809-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="f6809-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="f6809-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="f6809-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="f6809-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="f6809-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="f6809-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="f6809-109">**Migrē vairāk nekā 100TB datu**</span><span class="sxs-lookup"><span data-stu-id="f6809-109">**Migrating over 100TB of data**</span></span>

<span data-ttu-id="f6809-110">Šķiet, jūs esat migrē virs 100TB datu SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="f6809-110">It appears you are migrating over 100TB of data to SharePoint Online.</span></span> <span data-ttu-id="f6809-111">Lūdzu, veiciet tālāk norādītās darbības, lai mēs varētu jums palīdzēt pēc iespējas ātrāk.</span><span class="sxs-lookup"><span data-stu-id="f6809-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="f6809-112">Atlasiet **Jauns pakalpojuma pieprasījums**un pēc tam **jauna pakalpojuma pieprasījums**.</span><span class="sxs-lookup"><span data-stu-id="f6809-112">Select **New Service Request**, and then **New Service Request**.</span></span> 
2. <span data-ttu-id="f6809-113">Atstājiet nosaukumu un aprakstu kā **SharePoint migrācija virs 100TB**.</span><span class="sxs-lookup"><span data-stu-id="f6809-113">Leave the title and description as **SharePoint migration over 100TB**.</span></span>
3. <span data-ttu-id="f6809-114">Kad biļete ir iesniegta, lūdzu, atjauniniet to ar šādu informāciju:</span><span class="sxs-lookup"><span data-stu-id="f6809-114">Once the ticket has been submitted, please update it with the following information:</span></span> 

    - <span data-ttu-id="f6809-115">Aptuveno migrācijas lielumu.</span><span class="sxs-lookup"><span data-stu-id="f6809-115">Estimated size of your migration.</span></span>
    - <span data-ttu-id="f6809-116">Aprēķins par to, kad jūs vēlētos sākt un pabeigt savu migrāciju.</span><span class="sxs-lookup"><span data-stu-id="f6809-116">An estimate of when you would like to start and complete your migration.</span></span>
    - <span data-ttu-id="f6809-117">Aprakstiet, kur jūs migrējat saturu no, piemēram, SharePoint Server, Box, GDrive, failu koplietojumos utt.</span><span class="sxs-lookup"><span data-stu-id="f6809-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>


  

