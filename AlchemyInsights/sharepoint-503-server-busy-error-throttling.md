---
title: SharePoint Online ierobežošana
ms.author: pebaum
author: pebaum
ms.date: 9/17/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: b376d8ea-50c4-47f0-9720-50d80aa3f7f1
ms.custom:
- "9000149"
- "1662"
- "3491"
ms.openlocfilehash: 59104ef96c95de4e4bc7744825245bdafba97d7c
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931233"
---
# <a name="sharepoint-online-throttling"></a><span data-ttu-id="71f5c-102">SharePoint Online ierobežošana</span><span class="sxs-lookup"><span data-stu-id="71f5c-102">SharePoint Online Throttling</span></span>

<span data-ttu-id="71f5c-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="71f5c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="71f5c-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="71f5c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="71f5c-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="71f5c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="71f5c-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="71f5c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="71f5c-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="71f5c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="71f5c-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="71f5c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="71f5c-109">**503 serveris ir aizņemts kļūdas**</span><span class="sxs-lookup"><span data-stu-id="71f5c-109">**503 server is busy error**</span></span>

<span data-ttu-id="71f5c-110">Lietotāji var saņemt 503 serveris ir aizņemts kļūda, mēģinot naviģēt uz SharePoint vai OneDrive vietnes.</span><span class="sxs-lookup"><span data-stu-id="71f5c-110">Users may receive a 503 server is busy error when attempting to navigate to SharePoint or OneDrive sites.</span></span> 

<span data-ttu-id="71f5c-111">Šo kļūdu var izraisīt ierobežošana SharePoint pakalpojumu ietvaros.</span><span class="sxs-lookup"><span data-stu-id="71f5c-111">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="71f5c-112">SharePoint Online izmanto ierobežošana, lai uzturētu optimālu veiktspēju un uzticamību SharePoint Online pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="71f5c-112">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="71f5c-113">Ierobežošana ierobežo lietotāja darbību skaitu vai vienlaicīgus zvanus (pēc skripta vai koda), lai novērstu resursu pārmērīgu izmantošanu.</span><span class="sxs-lookup"><span data-stu-id="71f5c-113">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> 

<span data-ttu-id="71f5c-114">Lai iegūtu papildinformāciju par ierobežošana redzēt, [Izvairieties kļūst ierobežotas vai bloķēts SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="71f5c-114">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

<span data-ttu-id="71f5c-115">Ja uzskatāt, ka šī kļūda nav saistīta ar ierobežošana, varat pārbaudīt, vai ir aktīva uzturēšana notiek jūsu nomnieka, pārvietojoties uz [ziņojumu centru](https://portal.office.com/adminportal/home#/MessageCenter).</span><span class="sxs-lookup"><span data-stu-id="71f5c-115">If you believe this error is unrelated to throttling, you can check if there is active maintenance occurring on your tenant by navigating to the [Message center](https://portal.office.com/adminportal/home#/MessageCenter).</span></span>

 <span data-ttu-id="71f5c-116">Visbeidzot, pārliecinieties, ka jūs apmeklējat [pakalpojumu veselības](https://portal.office.com/adminportal/home#/servicehealth) lapu, lai pārbaudītu jebkuru konsultācijas/starpgadījumiem, kas var būt noticis.</span><span class="sxs-lookup"><span data-stu-id="71f5c-116">Finally, ensure you visit the [Service Health](https://portal.office.com/adminportal/home#/servicehealth) page to check for any advisories/incidents that may be occurring.</span></span>

