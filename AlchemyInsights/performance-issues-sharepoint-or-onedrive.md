---
title: Veiktspējas problēmas-SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: aecbf4043c6456ece73f7deed6b068040f0691a2
ms.sourcegitcommit: 0fb89d8106fe409ab1b78e50f5357ffc2252f7c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/17/2019
ms.locfileid: "40068416"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="6bf5d-102">SharePoint vai OneDrive lēns, nepieejams vai nav pieejams vairākiem lietotājiem</span><span class="sxs-lookup"><span data-stu-id="6bf5d-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="6bf5d-103">SharePoint vai OneDrive var būt lēns, nepieejams vai nav pieejams, vai var parādīt pakalpojumu nav pieejams vai 503 kļūdas, vairāku iemeslu dēļ:</span><span class="sxs-lookup"><span data-stu-id="6bf5d-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="6bf5d-104">Ja SharePoint vai OneDrive vietne ir lēna vai aizkavēta vairākiem lietotājiem, var būt pagaidu pakalpojumu problēma, kad lietotājiem rodas intermitējošas aizkaves vai navigācijas kļūdas, piekļūstot SharePoint vietnes vai OneDrive saturu.</span><span class="sxs-lookup"><span data-stu-id="6bf5d-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="6bf5d-105">Pārbaudiet [pakalpojuma darbspējas informācijas paneli](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , lai noskaidrotu, vai jūsu organizācija ir ietekmēta.</span><span class="sxs-lookup"><span data-stu-id="6bf5d-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="6bf5d-106">Lietotāji var saņemt *503 serveris ir aizņemts* kļūda, mēģinot naviģēt uz SharePoint vai OneDrive vietnes.</span><span class="sxs-lookup"><span data-stu-id="6bf5d-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="6bf5d-107">Šo kļūdu var izraisīt ierobežošana SharePoint pakalpojumu ietvaros.</span><span class="sxs-lookup"><span data-stu-id="6bf5d-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="6bf5d-108">SharePoint Online izmanto ierobežošana, lai uzturētu optimālu veiktspēju un uzticamību SharePoint Online pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="6bf5d-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="6bf5d-109">Ierobežošana ierobežo lietotāja darbību skaitu vai vienlaicīgus zvanus (pēc skripta vai koda), lai novērstu resursu pārmērīgu izmantošanu.</span><span class="sxs-lookup"><span data-stu-id="6bf5d-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="6bf5d-110">Lai iegūtu papildinformāciju par ierobežošana redzēt, [Izvairieties kļūst ierobežotas vai bloķēts SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="6bf5d-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="6bf5d-111">Ja sistēma darbojas ļoti lēni ar **klasisko** vai **moderno** SharePoint vietni vai lapu, izmantojiet [lapu diagnostikas rīku](https://aka.ms/perftool) , lai analizētu lapas.</span><span class="sxs-lookup"><span data-stu-id="6bf5d-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="6bf5d-112">Ja joprojām rodas vispārīga lēna veiktspēja, lūdzu, pārskatiet resursus šī raksta apakšā: [Ievads SharePoint Online veiktspējas precizēšana](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="6bf5d-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  