---
title: SharePoint Online ierobežošana
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.openlocfilehash: 9af4f09d50992c04a1f3d5a164093049a3ec3517
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931449"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="0828c-102">SharePoint Online ierobežošana</span><span class="sxs-lookup"><span data-stu-id="0828c-102">SharePoint Online throttling</span></span>

<span data-ttu-id="0828c-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="0828c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="0828c-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="0828c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="0828c-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="0828c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="0828c-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="0828c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="0828c-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="0828c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="0828c-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="0828c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="0828c-109">**SharePoint Online ierobežošana**</span><span class="sxs-lookup"><span data-stu-id="0828c-109">**SharePoint Online throttling**</span></span>

<span data-ttu-id="0828c-110">SharePoint Online izmanto ierobežošana, lai uzturētu optimālu veiktspēju un uzticamību SharePoint Online pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="0828c-110">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="0828c-111">Ierobežošana ierobežo lietotāja darbību skaitu vai vienlaicīgus zvanus (pēc skripta vai koda), lai novērstu resursu pārmērīgu izmantošanu.</span><span class="sxs-lookup"><span data-stu-id="0828c-111">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="0828c-112">Lai iegūtu vairāk informācijas, lūdzu, apmeklējiet saites zemāk.</span><span class="sxs-lookup"><span data-stu-id="0828c-112">For more information, please visit the links below.</span></span>

- [<span data-ttu-id="0828c-113">Izvairīties no ierobežotas vai bloķēts SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="0828c-113">Avoid getting throttled or blocked in SharePoint Online</span></span>](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online)

- [<span data-ttu-id="0828c-114">Datu migrēšana un SPO ierobežošana</span><span class="sxs-lookup"><span data-stu-id="0828c-114">Data Migration and SPO Throttling </span></span>](https://blogs.technet.microsoft.com/sposupport/2017/08/12/data-migration-and-spo-service-throttling/)

- [<span data-ttu-id="0828c-115">SharePoint Online un OneDrive migrācijas ātrums</span><span class="sxs-lookup"><span data-stu-id="0828c-115">SharePoint Online and OneDrive Migration Speed</span></span>](https://docs.microsoft.com/sharepointmigration/sharepoint-online-and-onedrive-migration-speed)

 - [<span data-ttu-id="0828c-116">Rīkoties ar SharePoint Online ierobežošana, izmantojot eksponenciālo atpakaļ off</span><span class="sxs-lookup"><span data-stu-id="0828c-116">Handle SharePoint Online throttling by using exponential back off</span></span>](https://docs.microsoft.com/sharepoint/dev/solution-guidance/handle-sharepoint-online-throttling-by-using-exponential-back-off)

- [<span data-ttu-id="0828c-117">Noslodzes plānošana un slodzes testēšana SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="0828c-117">Capacity planning and load testing SharePoint Online</span></span>](https://docs.microsoft.com/office365/enterprise/capacity-planning-and-load-testing-sharepoint-online)

