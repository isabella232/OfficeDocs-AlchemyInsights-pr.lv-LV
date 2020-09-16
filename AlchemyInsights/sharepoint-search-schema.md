---
title: Meklēšanas shēmas pārvaldība pakalpojumā SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: f2d8d3e07fe32d21af484e4c59e0f5ac6fe8081c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770558"
---
# <a name="manage-search-schema-in-sharepoint-online"></a><span data-ttu-id="2e4df-102">Meklēšanas shēmas pārvaldība pakalpojumā SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="2e4df-102">Manage search schema in SharePoint Online</span></span>

<span data-ttu-id="2e4df-103">Meklēšanas shēma kontrolē to, ko lietotāji var meklēt, kā lietotāji var tos meklēt un kā var prezentēt rezultātus meklēšanas tīmekļa vietnēs.</span><span class="sxs-lookup"><span data-stu-id="2e4df-103">The search schema controls what users can search for, how users can search it, and how you can present the results on your search websites.</span></span> 

<span data-ttu-id="2e4df-104">Papildinformāciju [par to,](https://docs.microsoft.com/sharepoint/manage-search-schema) kā:</span><span class="sxs-lookup"><span data-stu-id="2e4df-104">See [Manage the Search Schema in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-search-schema) to learn how to:</span></span> 
- <span data-ttu-id="2e4df-105">Mainiet meklēšanas shēmu.</span><span class="sxs-lookup"><span data-stu-id="2e4df-105">Change the search schema.</span></span>
- <span data-ttu-id="2e4df-106">Izveidot pārvaldītos rekvizītus.</span><span class="sxs-lookup"><span data-stu-id="2e4df-106">Create managed properties.</span></span>
- <span data-ttu-id="2e4df-107">Kartēt pārmeklētos kartes pārmeklētos rekvizītus uz pārvaldītajiem rekvizītiem.</span><span class="sxs-lookup"><span data-stu-id="2e4df-107">Map crawled map crawled properties to managed properties.</span></span>

<span data-ttu-id="2e4df-108">Ņemiet vērā tālāk norādītās darbības, lai pārvaldītu meklēšanas shēmu:</span><span class="sxs-lookup"><span data-stu-id="2e4df-108">Note the following in regards to managing your Search Schema:</span></span>

- <span data-ttu-id="2e4df-109">Ja saņemat brīdinājumu par to, **ka lietojumprogrammas darbība ir apturēta** , veicot izmaiņas shēmā, šī darbība ir tikai pagaidu, jo notiek pakalpojuma uzturēšana.</span><span class="sxs-lookup"><span data-stu-id="2e4df-109">If you receive a warning stating **the application is paused** when making a schema change, this is only temporary as there is service maintenance occurring.</span></span> 

    <span data-ttu-id="2e4df-110">Ja ir pagājušas vairāk nekā 24 stundas un joprojām tiek rādīts brīdinājums, lūdzu, piesakieties atbalsta lietu.</span><span class="sxs-lookup"><span data-stu-id="2e4df-110">If more than 24 hours have passed and you still experience the warning, please log a support case.</span></span>
- <span data-ttu-id="2e4df-111">Mainot pārvaldītos rekvizītus vai pievienojot jaunus, izmaiņas stājas spēkā tikai pēc tam, kad saturs ir atkārtoti pārmeklēts.</span><span class="sxs-lookup"><span data-stu-id="2e4df-111">When you change managed properties or add new ones, the changes take effect only after the content has been re-crawled.</span></span> <span data-ttu-id="2e4df-112">Pakalpojumā SharePoint Online pārmeklēšana notiek automātiski, pamatojoties uz definēto pārmeklēšanas plānu.</span><span class="sxs-lookup"><span data-stu-id="2e4df-112">In SharePoint Online, crawling happens automatically based on the defined crawl schedule.</span></span>
- <span data-ttu-id="2e4df-113">Lai pārliecinātos, vai veiktās izmaiņas ir pārmeklētas, varat īpaši [pieprasīt saraksta vai bibliotēkas atkārtotu indeksēšanu](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span><span class="sxs-lookup"><span data-stu-id="2e4df-113">To make sure that your changes are crawled, you can specifically [request a re-indexing of the list or library](https://docs.microsoft.com/sharepoint/manage-search-schema#request-re-indexing-of-a-document-library-or-list)</span></span> 

<span data-ttu-id="2e4df-114">Pilnīgu pārskatu par meklēšanas shēmu skatiet rakstā [Ievads par meklēšanas shēmu](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span><span class="sxs-lookup"><span data-stu-id="2e4df-114">For a complete overview of the Search Schema, see [Introducing Search Schema](https://blogs.technet.microsoft.com/tothesharepoint/2012/11/25/introducing-search-schema-for-sharepoint-2013/)</span></span> 


