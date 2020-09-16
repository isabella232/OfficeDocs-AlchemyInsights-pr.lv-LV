---
title: Veiktspējas problēmas — SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1133"
- "2397"
- "2418"
- "5200018"
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 28867b71df5353dcee5cc3361742f10357a0efe1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771908"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="a3713-102">SharePoint vai OneDrive lēnā, nepieejama vai nav pieejama vairākiem lietotājiem</span><span class="sxs-lookup"><span data-stu-id="a3713-102">SharePoint or OneDrive slow, inaccessible, or unavailable for multiple users</span></span>

<span data-ttu-id="a3713-103">SharePoint vai OneDrive var būt lēna, nepieejama vai nepieejama, vai var tikt parādīta pakalpojuma nepieejamība vai 503 kļūdas vairāku iemeslu dēļ:</span><span class="sxs-lookup"><span data-stu-id="a3713-103">SharePoint or OneDrive may be slow, inaccessible, or unavailable, or may display service unavailable or 503 errors, for several reasons:</span></span>
  
- <span data-ttu-id="a3713-104">Ja jūsu SharePoint vai OneDrive vietne ir lēna vai aizkavēta vairākiem lietotājiem, iespējama īslaicīga pakalpojumu problēma, kur lietotājiem rodas neregulāras aizkaves vai navigācijas kļūdas, piekļūstot SharePoint vietnēm vai OneDrive saturam.</span><span class="sxs-lookup"><span data-stu-id="a3713-104">If your SharePoint or OneDrive site is slow or delayed for multiple users, there may be a temporary service issue where users experience intermittent delays or navigation errors when accessing SharePoint sites or OneDrive content.</span></span> <span data-ttu-id="a3713-105">Pārbaudiet [Pakalpojuma darbspējas informācijas paneli](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) , lai noskaidrotu, vai jūsu organizācija ir ietekmēta.</span><span class="sxs-lookup"><span data-stu-id="a3713-105">Check the [Service health dashboard](https://admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>
  
- <span data-ttu-id="a3713-106">Mēģinot veikt navigāciju uz SharePoint vai OneDrive vietnēm, lietotāji var saņemt *503 serveri ir aizņemts* .</span><span class="sxs-lookup"><span data-stu-id="a3713-106">Users may receive a *503 server is busy* error when attempting to navigate to SharePoint or OneDrive sites.</span></span> <span data-ttu-id="a3713-107">Šo kļūdu var izraisīt ierobežošana SharePoint pakalpojumā.</span><span class="sxs-lookup"><span data-stu-id="a3713-107">This error can be caused by throttling within the SharePoint service.</span></span> <span data-ttu-id="a3713-108">SharePoint Online izmanto ierobežošanu, lai uzturētu optimālu SharePoint Online pakalpojuma veiktspēju un uzticamību.</span><span class="sxs-lookup"><span data-stu-id="a3713-108">SharePoint Online uses throttling to maintain optimal performance and reliability of the SharePoint Online service.</span></span> <span data-ttu-id="a3713-109">Ierobežošana ierobežo lietotāju darbību vai vienlaicīgu zvanu skaitu (ar skriptu vai kodu), lai nepieļautu pārmērīgu resursu pielietojumu.</span><span class="sxs-lookup"><span data-stu-id="a3713-109">Throttling limits the number of user actions or concurrent calls (by script or code) to prevent overuse of resources.</span></span> <span data-ttu-id="a3713-110">Papildinformāciju par ierobežošanu skatiet rakstā Neļaujiet ierobežot [vai bloķēt pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span><span class="sxs-lookup"><span data-stu-id="a3713-110">For more information on throttling see, [Avoid getting throttled or blocked in SharePoint Online](https://docs.microsoft.com/sharepoint/dev/general-development/how-to-avoid-getting-throttled-or-blocked-in-sharepoint-online).</span></span>

- <span data-ttu-id="a3713-111">Ja rodas lēna veiktspēja ar **klasisko** vai **mūsdienīgu** SharePoint vietni vai lapu, izmantojiet [lapu diagnostikas rīku](https://aka.ms/perftool) , lai analizētu lapas.</span><span class="sxs-lookup"><span data-stu-id="a3713-111">If you experience slow performance with a **classic** or **modern** SharePoint site or page, utilize the [Page Diagnostic tool](https://aka.ms/perftool) to analyze the pages.</span></span>
  
- <span data-ttu-id="a3713-112">Ja joprojām rodas lēna veiktspēja, lūdzu, pārskatiet resursus šī raksta beigās: [Ievads par SharePoint Online veiktspējas uzlabošanu](https://go.microsoft.com/fwlink/?linkid=2024334)</span><span class="sxs-lookup"><span data-stu-id="a3713-112">If you still experience general slow performance, please review the resources at the bottom of this article: [Introduction to performance tuning for SharePoint Online](https://go.microsoft.com/fwlink/?linkid=2024334)</span></span>
  