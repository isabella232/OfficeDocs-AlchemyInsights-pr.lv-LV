---
title: Meklēt SharePoint tiešsaistē
ms.author: efrene
author: efrene
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: fc49978fbd2c07381dae83061b1a1868cd1df0d0
ms.sourcegitcommit: 327a2c77afc2ff3d67d3aaaea1a92068a3c4bb1f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/06/2019
ms.locfileid: "36059259"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="b7332-102">Meklēt SharePoint tiešsaistē</span><span class="sxs-lookup"><span data-stu-id="b7332-102">Search in SharePoint Online</span></span>

<span data-ttu-id="b7332-103">Saturs pārmeklēts un pievienoti lietotāji atrast to, ko viņi meklē ar SharePoint Online meklēšanas indekss.</span><span class="sxs-lookup"><span data-stu-id="b7332-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="b7332-104">Tiek automātiski pārmeklēts saturs balstoties uz iepriekš definētajiem pārmeklēšanas grafiku (pārmeklēšanas grafiku nevar mainīt).</span><span class="sxs-lookup"><span data-stu-id="b7332-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="b7332-105">Kāpurķēžu paceļ saturu, kas mainīts, kopš pēdējās pārmeklēšanas un atjaunina indekss.</span><span class="sxs-lookup"><span data-stu-id="b7332-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="b7332-106">Lai nodrošinātu saturs tiek pārmeklēts un indekss tiek atjaunināts, ievērojiet sekojošo:</span><span class="sxs-lookup"><span data-stu-id="b7332-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="b7332-107">Pārliecinieties, ka saturs var atrast, [veicot meklēšanu vietnes saturu](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="b7332-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="b7332-108">Mainoties pārvaldīto rekvizītu, vai ja jūs esat mainījis kartēšanu, pārmeklēts un pārvalda īpašības, vietā jābūt atkārtoti pārmeklēto pirms jūsu veiktās izmaiņas tiks atspoguļotas meklēšanas indeksā.</span><span class="sxs-lookup"><span data-stu-id="b7332-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="b7332-109">Jo izmaiņas veiktas meklēšanas shēmas, un nevis uz reālo vietu, kāpurķēžu tiks automātiski atkārtoti indeksēt vietni.</span><span class="sxs-lookup"><span data-stu-id="b7332-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="b7332-110">Lai iegūtu vairāk informācijas, skatiet [manuāli pieprasīt pārmeklēšanas un indeksēšanas atkārtoti, vietni, bibliotēku vai sarakstu](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="b7332-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="b7332-111">Pagaidiet vismaz 24 stundas pēc tam, kad manuāli pieprasīt pārmeklēšanas un pilnu Pārindeksēt redzēt, ja joprojām rodas jautājums.</span><span class="sxs-lookup"><span data-stu-id="b7332-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="b7332-112">Ja ilgāk par 24 stundām, ir pagājuši, kopš esat sācis rāpot un pilnu Pārindeksēt, lūdzu, piesakieties atbalsta gadījumu.</span><span class="sxs-lookup"><span data-stu-id="b7332-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="b7332-113">Daudzos gadījumos mēs jau strādājam pie risinājuma.</span><span class="sxs-lookup"><span data-stu-id="b7332-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="b7332-114">Lūdzu, sniedziet mums vismaz 24 stundas, lai pabeigtu risinājumu.</span><span class="sxs-lookup"><span data-stu-id="b7332-114">Please give us at least 24 hours to complete a solution.</span></span>

>[! Svarīgi!]<span data-ttu-id="b7332-115">: ja vietu, dokumentu (bibliotēka) vai sarakstu tika svītrots un joprojām rāda meklēšanas rezultātus, lietotājiem vajadzētu saņemt **Kļūda 404 fails nav atrasts** , mēģinot piekļūt.</span><span class="sxs-lookup"><span data-stu-id="b7332-115">: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="b7332-116">Šis jautājums būtu pieteicies kā atbalsta gadījumā turpmākas izmeklēšanas veikšanai.</span><span class="sxs-lookup"><span data-stu-id="b7332-116">This issue should be logged as a support case for further investigation.</span></span> 



