---
title: Meklēt SharePoint Online
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: fe00f4c0-44d5-49d4-9db0-a62698bcd1d1
ms.openlocfilehash: c4ff98f0cf928834c803542340b32da15a40d583
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40044050"
---
# <a name="content-crawling-and-indexing-in-sharepoint-online"></a><span data-ttu-id="8feb7-102">Satura indeksēšanu un indeksēšanu SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="8feb7-102">Content crawling and indexing in SharePoint Online</span></span>

<span data-ttu-id="8feb7-103">Saturs ir jāpārmeklē un jāpievieno meklēšanas indeksam, lai lietotāji varētu atrast to, ko viņi meklē SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="8feb7-103">Content must be crawled and added to the search index for users to find what they're searching for in SharePoint Online.</span></span> <span data-ttu-id="8feb7-104">Saturs tiek automātiski pārmeklēts, pamatojoties uz iepriekš definētu pārmeklēšanas grafiku (pārmeklēšanas grafiku nevar mainīt).</span><span class="sxs-lookup"><span data-stu-id="8feb7-104">Content is automatically crawled based on a pre-defined crawl schedule (the crawl schedule cannot be changed).</span></span> <span data-ttu-id="8feb7-105">Kāpurķēžu paceļ saturu, kas ir mainījies kopš pēdējās pārmeklēšanas un atjaunina indeksu.</span><span class="sxs-lookup"><span data-stu-id="8feb7-105">The crawler picks up content that has changed since the last crawl and updates the index.</span></span> <span data-ttu-id="8feb7-106">Lai nodrošinātu, ka saturs tiek pārmeklēts un indekss tiek atjaunināts, ņemiet vērā tālāk minēto.</span><span class="sxs-lookup"><span data-stu-id="8feb7-106">To ensure content is crawled and the index is updated, note the following:</span></span>

- <span data-ttu-id="8feb7-107">Pārliecinieties, vai saturu var atrast, [padarot vietnes saturu meklējamu](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="8feb7-107">Make sure content can be found by [making site content searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span>

- <span data-ttu-id="8feb7-108">Kad esat mainījis pārvaldīto rekvizītu vai esat mainījis pārmeklēto un pārvaldīto rekvizītu kartēšanu, vietne ir atkārtoti jāindeksē, pirms izmaiņas tiks atspoguļotas meklēšanas indeksā.</span><span class="sxs-lookup"><span data-stu-id="8feb7-108">When you have changed a managed property, or when you have changed the mapping of crawled and managed properties, the site must be re-crawled before your changes will be reflected in the search index.</span></span> 

    <span data-ttu-id="8feb7-109">Tāpēc, ka veiktās izmaiņas tiek veiktas meklēšanas shēmā, nevis faktiskajā vietā, rāpuļprogramma automātiski neindeksēs vietni.</span><span class="sxs-lookup"><span data-stu-id="8feb7-109">Because your changes are made in the search schema, and not to the actual site, the crawler will not automatically re-index the site.</span></span> 

    <span data-ttu-id="8feb7-110">Papildinformāciju skatiet sadaļā [manuāla pieprasījuma pārmeklēšanas un atkārtotas indeksēšanas vietnei, bibliotēkai vai sarakstam](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span><span class="sxs-lookup"><span data-stu-id="8feb7-110">For more info, see [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-conten).</span></span>

- <span data-ttu-id="8feb7-111">Uzgaidiet vismaz 24 stundas pēc manuālas pārmeklēšanas un pilna atkārtotas indeksa pieprasīšanas, lai redzētu, vai problēma joprojām pastāv.</span><span class="sxs-lookup"><span data-stu-id="8feb7-111">Wait at least 24 hours after manually requesting a crawl and full re-index to see if you're still experiencing an issue.</span></span> 

    <span data-ttu-id="8feb7-112">Ja vairāk nekā 24 stundas ir pagājis kopš sākāt pārmeklēšanas un pilnu re-Index, lūdzu, piesakieties atbalsta pieteikumu.</span><span class="sxs-lookup"><span data-stu-id="8feb7-112">If more than 24 hours have passed since you initiated the crawl and full re-index, please log a support case.</span></span> <span data-ttu-id="8feb7-113">Daudzos gadījumos mēs jau strādājam pie risinājuma.</span><span class="sxs-lookup"><span data-stu-id="8feb7-113">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="8feb7-114">Lūdzu, sniedziet mums vismaz 24 stundas, lai pabeigtu risinājumu.</span><span class="sxs-lookup"><span data-stu-id="8feb7-114">Please give us at least 24 hours to complete a solution.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="8feb7-115">Ja vietne, dokumentu (bibliotēka) vai saraksts ir izdzēsts un joprojām rāda meklēšanas rezultātos, lietotājiem ir jāsaņem **kļūda 404 fails nav atrasts** , mēģinot piekļūt.</span><span class="sxs-lookup"><span data-stu-id="8feb7-115">If a site, document (library), or a list was deleted and still shows in the search results, users should receive an **Error 404 File Not Found** when trying to access it.</span></span> <span data-ttu-id="8feb7-116">Šī problēma ir jāpiesakās kā atbalsta gadījumu tālākai izmeklēšanai.</span><span class="sxs-lookup"><span data-stu-id="8feb7-116">This issue should be logged as a support case for further investigation.</span></span> 



