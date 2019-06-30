---
title: Saturs netiek parādīti SharePoint meklēšanas rezultātus
ms.author: tlarsen
author: tklarsen
ms.date: 1/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "750"
- "5300017"
ms.assetid: 693db84f-2737-4c21-b027-4ab3d121b4a8
ms.openlocfilehash: 8215b0a5cde5adffa3bec37d6699418557f914dd
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35363820"
---
# <a name="content-doesnt-appear-in-sharepoint-search-results"></a><span data-ttu-id="51b07-102">Saturs netiek parādīti SharePoint meklēšanas rezultātus</span><span class="sxs-lookup"><span data-stu-id="51b07-102">Content doesn't appear in SharePoint search results</span></span>

<span data-ttu-id="51b07-103">Veiciet šādus traucējumu meklēšanas posmus, kad paredzamais saturs neparādās meklēšanas rezultātos:</span><span class="sxs-lookup"><span data-stu-id="51b07-103">Follow these troubleshooting steps when expected content doesn't appear in search results:</span></span>
  
1. <span data-ttu-id="51b07-104">Pārbaudiet, vai **vietnē** , kurā atrodas paredzamais saturs ir iestatīts atļaut saturs tiek parādīti meklēšanu rezultātos.</span><span class="sxs-lookup"><span data-stu-id="51b07-104">Check that the **site** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="51b07-105">Izpildiet norādījumus sadaļā [Rādīt saturu vietnes meklēšanas rezultātos](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="51b07-105">Follow the steps in [Show content on a site in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-on-a-site-in-search-results).</span></span>

2. <span data-ttu-id="51b07-106">Pārbaudiet, vai **saraksts** vai **bibliotēka** , kurā atrodas paredzamais saturs ir iestatīts atļaut saturs tiek parādīti meklēšanu rezultātos.</span><span class="sxs-lookup"><span data-stu-id="51b07-106">Check that the **list** or **library** that contains the expected content is set to allow content to appear in search results.</span></span> <span data-ttu-id="51b07-107">Izpildiet norādījumus sadaļā [Rādīt saturu no sarakstiem vai bibliotēkām, meklēšanas rezultātos](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span><span class="sxs-lookup"><span data-stu-id="51b07-107">Follow the steps in [Show content from lists or libraries in search results](https://docs.microsoft.com/sharepoint/make-site-content-searchable#show-content-from-lists-or-libraries-in-search-results).</span></span>

3. <span data-ttu-id="51b07-108">Pārbaudīt, kā tiek publicēts lappusi, dokumentu vai pielāgotā lappuses izkārtojumā **pamatversijas.**</span><span class="sxs-lookup"><span data-stu-id="51b07-108">Verify that the page, document, or custom page layout is published as a **Major version.**</span></span> <span data-ttu-id="51b07-109">Sekot soli 3 [meklēšana neatgriež visus rezultātus SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span><span class="sxs-lookup"><span data-stu-id="51b07-109">Follow step 3 in [Search doesn't return all results in SharePoint Online](https://go.microsoft.com/fwlink/?linkid=874525).</span></span>

4. <span data-ttu-id="51b07-110">Pārbaudiet, vai lietotājam ir **atļaujas** skatīt ārējo saturu.</span><span class="sxs-lookup"><span data-stu-id="51b07-110">Verify that the user has **permissions** to view the content.</span></span> <span data-ttu-id="51b07-111">Izpildiet norādītās darbības [izpratne atļauju līmeņus koplietošanas vidē SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="51b07-111">Follow the steps in [Understanding permission levels in SharePoint](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels).</span></span>
    
5. <span data-ttu-id="51b07-112">Ja ir mainīta meklēšanas shēmas, pievienojot jaunu pārvaldīto rekvizītu, pārvaldīto rekvizītu rediģēšana vai noņemšana pārvaldīto rekvizītu, tad pieprasītāja rāpot un Pārindeksēt būs nepieciešami.</span><span class="sxs-lookup"><span data-stu-id="51b07-112">If the search schema has been changed by adding a new managed property, by editing a managed property, or by removing a managed property then requesting a crawl and re-index will be required.</span></span> <span data-ttu-id="51b07-113">**Pārindeksēt** saturu, izpildot darbības, [manuāli pieprasīt pārmeklēšanas un indeksēšanas atkārtoti, vietni, bibliotēku vai sarakstu](https://docs.microsoft.com/sharepoint/crawl-site-content).</span><span class="sxs-lookup"><span data-stu-id="51b07-113">**Re-index** the content by following the steps in [Manually request crawling and re-indexing of a site, a library or a list](https://docs.microsoft.com/sharepoint/crawl-site-content).</span></span> <span data-ttu-id="51b07-114">Tas var aizņemt kādu laiku, pagaidiet 24 stundas pirms atkārtotas pārbaudes rezultātus.</span><span class="sxs-lookup"><span data-stu-id="51b07-114">This might take a while, wait 24 hours before checking the results again.</span></span>

<span data-ttu-id="51b07-115">Papildinformāciju skatiet sadaļā [iespējot satura vietnē ir meklējams](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span><span class="sxs-lookup"><span data-stu-id="51b07-115">For more information, see [Enable content on a site to be searchable](https://docs.microsoft.com/sharepoint/make-site-content-searchable).</span></span> 
  
