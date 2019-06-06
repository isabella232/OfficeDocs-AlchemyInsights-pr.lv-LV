---
title: Pārvaldīt meklēšanas vārdnīcas SharePoint Online
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c2960093bb1cfb649c26528c9f671e6d720ff237
ms.sourcegitcommit: 241e21b6da226563bf70bdb1f5bad3d91c38cd2c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2019
ms.locfileid: "34736059"
---
# <a name="search-in-sharepoint-online"></a><span data-ttu-id="d6f00-102">Meklēt SharePoint tiešsaistē</span><span class="sxs-lookup"><span data-stu-id="d6f00-102">Search in SharePoint Online</span></span>

<span data-ttu-id="d6f00-103">Saturs pārmeklēts un pievienoti lietotāji atrast to, ko viņi meklē ar SharePoint Online meklēšanas indekss.</span><span class="sxs-lookup"><span data-stu-id="d6f00-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="d6f00-104">Tiek automātiski pārmeklēts saturs balstoties uz iepriekš definētajiem pārmeklēšanas grafiku (pārmeklēšanas grafiku nevar mainīt).</span><span class="sxs-lookup"><span data-stu-id="d6f00-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="d6f00-105">Kāpurķēžu paceļ saturu, kas mainīts, kopš pēdējās pārmeklēšanas un atjaunina indekss.</span><span class="sxs-lookup"><span data-stu-id="d6f00-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="d6f00-106">Lai nodrošinātu saturs tiek pārmeklēts un indekss tiek atjaunināts, izpildiet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="d6f00-106">To ensure content is crawled and the index is updated, follow the steps below.</span></span>

<span data-ttu-id="d6f00-107">Pārliecinieties, ka saturs var atrast, veicot meklēšanu vietnes satura.</span><span class="sxs-lookup"><span data-stu-id="d6f00-107">Make sure content can be found by making site content searchable.</span></span> <span data-ttu-id="d6f00-108">Lai iegūtu vairāk informācijas, skatiet [iespējot satura vietnē ir meklējams](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="d6f00-108">For more info, see [Enable content on a site to be searchable](https://docs.microsoft.com/en-us/sharepoint/make-site-content-searchable).</span></span>

<span data-ttu-id="d6f00-109">Mainoties pārvaldīto rekvizītu, vai ja jūs esat mainījis kartēšanu, pārmeklēts un pārvalda īpašības, vietā jābūt atkārtoti pārmeklēto pirms jūsu veiktās izmaiņas tiks atspoguļotas meklēšanas indeksā.</span><span class="sxs-lookup"><span data-stu-id="d6f00-109">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

<span data-ttu-id="d6f00-110">Jo izmaiņas veiktas meklēšanas shēmas, un nevis uz reālo vietu, kāpurķēžu tiks automātiski atkārtoti indeksēt vietni.</span><span class="sxs-lookup"><span data-stu-id="d6f00-110">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

<span data-ttu-id="d6f00-111">Lai iegūtu vairāk informācijas, skatiet [manuāli pieprasīt pārmeklēšanas un indeksēšanas atkārtoti, vietni, bibliotēku vai sarakstu](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="d6f00-111">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/en-us/sharepoint/crawl-site-conten).</span></span>

 <span data-ttu-id="d6f00-112">Pagaidiet vismaz 24 stundas pēc tam, kad manuāli pieprasīt pārmeklēšanas un pilnu Pārindeksēt redzēt, ja joprojām rodas jautājums.</span><span class="sxs-lookup"><span data-stu-id="d6f00-112">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

<span data-ttu-id="d6f00-113">Ja ilgāk par 24 stundām, ir pagājuši, kopš esat sācis rāpot un pilnu Pārindeksēt, lūdzu, piesakieties atbalsta gadījumu.</span><span class="sxs-lookup"><span data-stu-id="d6f00-113">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="d6f00-114">Daudzos gadījumos mēs jau strādājam pie risinājuma.</span><span class="sxs-lookup"><span data-stu-id="d6f00-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="d6f00-115">Lūdzu, sniedziet mums vismaz 24 stundas, lai pabeigtu risinājumu.</span><span class="sxs-lookup"><span data-stu-id="d6f00-115">Please give us at least 24 hours to complete a solution.</span></span>

<span data-ttu-id="d6f00-116">**Svarīgi**: ja vietu, dokumentu (bibliotēka) vai sarakstu tika svītrots un joprojām rāda meklēšanas rezultātus, lietotājiem vajadzētu saņemt 404 failā nav atrasta kļūda mēģinot piekļūt.</span><span class="sxs-lookup"><span data-stu-id="d6f00-116">**Important**: If a site, document (library), or a list was deleted and still shows in the search results, users should receive an Error 404 File Not Found when trying to access.</span></span> <span data-ttu-id="d6f00-117">Šis jautājums būtu pieteicies kā atbalsta gadījumā turpmākas izmeklēšanas veikšanai.</span><span class="sxs-lookup"><span data-stu-id="d6f00-117">This issue should be logged as a support case for further investigation.</span></span> 



