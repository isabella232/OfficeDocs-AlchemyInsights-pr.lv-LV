---
title: tas pats, kas faila nosaukums ir vispiemērotākais
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 113d01e0fc92cc9845e585919ab05f386d6892bb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664141"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="7f2b7-102">"Required Alchemy header H1, H2's nedarbojas".</span><span class="sxs-lookup"><span data-stu-id="7f2b7-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="7f2b7-103">Paraugprakse un norādījumi par alķīmijas autorēšanu:</span><span class="sxs-lookup"><span data-stu-id="7f2b7-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="7f2b7-104">**Neligzdojiet alķīmijas ieskatus mapēs**— tas pārtrauks vietrāža URL struktūru.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="7f2b7-105">Mēs meklējam šo problēmu.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="7f2b7-106">Failiem mapē **AlchemyInsights** ir jābūt ar mazajiem burtiem ar defisēm, kas paredzētas atstarpēm.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="7f2b7-107">***padomi par to, kā to iespējot***.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="7f2b7-108">Iekļaujiet kārtulas ID vai kopas ID no [alķīmijas partnera portāla](https://alchemyportal.azurewebsites.net) MS. Custom laukā.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="7f2b7-109">//templates.Office.com/.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-109">ex.</span></span> <span data-ttu-id="7f2b7-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="7f2b7-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="7f2b7-111">Izmantojiet pārējos šī faila augšdaļā esošo metadatu veidnes.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="7f2b7-112">[Alķīmijas partnera portālā](https://alchemyportal.azurewebsites.net)pārejiet uz leju līdz sadaļas **klientu izpratnes virsrakstam:** un izmantojiet to kā sākumpunktu, lai iegūtu ieskatu.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="7f2b7-113">Alķīmijas ieskatiem augšdaļā ir jābūt tikai vienam H1, vai tie salūsts ražošanā.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="7f2b7-114">H2s neatveido, tāpēc izmantojiet **treknraksta** vai citas konvencijas, lai norādītu atsevišķas sadaļas.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="7f2b7-115">Pēc tam aizpildiet pamattekstu, izmantojot melnraksta materiālu, kas atrodas alķīmijas kārtulas lapas sadaļā klientu ieskati</span><span class="sxs-lookup"><span data-stu-id="7f2b7-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="7f2b7-116">Saraksti ar aizzīmēm ir precīzi</span><span class="sxs-lookup"><span data-stu-id="7f2b7-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="7f2b7-117">Arī numurētie saraksti</span><span class="sxs-lookup"><span data-stu-id="7f2b7-117">Numbered lists too</span></span>
    1. <span data-ttu-id="7f2b7-118">**Treknraksts** un *Slīpraksts* ir a-OK</span><span class="sxs-lookup"><span data-stu-id="7f2b7-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="7f2b7-119">Saitēm vienmēr jābūt vai nu **"saitēm uz tīmekli"/External** vai **dziļām saitēm uz UI elementiem**, nevis iekšējām saitēm.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="7f2b7-120">Pašlaik attēli nav oficiāli atbalstīti, taču tie ir iekļauti ceļvedī.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="7f2b7-121">Un tas jau ir pārāk garš.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-121">And this is really already a bit too long.</span></span> <span data-ttu-id="7f2b7-122">Paraugprakse ir par 400 rakstzīmēm---------------------------------</span><span class="sxs-lookup"><span data-stu-id="7f2b7-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="7f2b7-123">Kad saturs ir gatavs, velciet to uz tiešo zaru.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="7f2b7-124">Pēc tam dodieties uz [alķīmijas partnera portālu](https://alchemyportal.azurewebsites.net) un ievadiet faila nosaukumu laukā URL.</span><span class="sxs-lookup"><span data-stu-id="7f2b7-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 