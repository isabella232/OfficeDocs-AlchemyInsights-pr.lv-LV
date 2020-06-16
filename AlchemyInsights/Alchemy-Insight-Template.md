---
title: pats , kas faila nosaukums , ir vislabākais
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: bd2901580acdb1dc17f3e14a7a9356b07e70f910
ms.sourcegitcommit: bf6a0e80d09aebae19b9e993c2552b88e49177c9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/16/2020
ms.locfileid: "44750977"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="24c32-102">"Required Alchemy Header H1, H2's nedarbojas."</span><span class="sxs-lookup"><span data-stu-id="24c32-102">"Required Alchemy Header H1, H2's dont work."</span></span>
<span data-ttu-id="24c32-103">Paraugprakse un vadlīnijas alķīmijas autorēšanas:</span><span class="sxs-lookup"><span data-stu-id="24c32-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="24c32-104">**Neligzdo alchemy Ieskats mapēs**- tas būs pārtraukums URL struktūru.</span><span class="sxs-lookup"><span data-stu-id="24c32-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="24c32-105">Mēs meklējam to noteikt.</span><span class="sxs-lookup"><span data-stu-id="24c32-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="24c32-106">Failiem mapē **AlchemyInsights** ir jābūt mazo burtu failu nosaukumiem ar defisēm atstarpēm ex.</span><span class="sxs-lookup"><span data-stu-id="24c32-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="24c32-107">***how-to-enable-litigation-hold***.</span><span class="sxs-lookup"><span data-stu-id="24c32-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="24c32-108">Iekļaujiet kārtulas ID vai kopuma ID [alhemijas partnera portālā](https://alchemyportal.azurewebsites.net) ms.custom laukā.</span><span class="sxs-lookup"><span data-stu-id="24c32-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="24c32-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="24c32-109">ex.</span></span> <span data-ttu-id="24c32-110">***ms.custom: 100021 ms.custom: 100.021***</span><span class="sxs-lookup"><span data-stu-id="24c32-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="24c32-111">Izmantojiet pārējos metadatus, kas atrodas šī faila augšdaļā kā veidni.</span><span class="sxs-lookup"><span data-stu-id="24c32-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="24c32-112">Portālā [Alchemy partner (Alchemy partner"](https://alchemyportal.azurewebsites.net)) naviģējiet uz leju līdz sadaļai **Customer Insight Title (Customer Insight Title):** un izmantojiet to kā sākumpunktu savam H1 nosaukumam, lai gūtu ieskatu.</span><span class="sxs-lookup"><span data-stu-id="24c32-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="24c32-113">Alchemy Insights jābūt tikai vienu H1 augšpusē vai tie būs pārtraukums ražošanā.</span><span class="sxs-lookup"><span data-stu-id="24c32-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="24c32-114">H2s nav padarīt vai nu tik izmantot **treknrakstā vai** citās konvencijās, lai apzīmējums atsevišķas sadaļas.</span><span class="sxs-lookup"><span data-stu-id="24c32-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="24c32-115">Pēc tam aizpildiet pamattekstu, izmantojot melnraksta materiālu lapas "Klients ieskati" sadaļā Customer Insights</span><span class="sxs-lookup"><span data-stu-id="24c32-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="24c32-116">Saraksti ar aizzīmēm ir labi</span><span class="sxs-lookup"><span data-stu-id="24c32-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="24c32-117">Numurēti saraksti pārāk</span><span class="sxs-lookup"><span data-stu-id="24c32-117">Numbered lists too</span></span>
    1. <span data-ttu-id="24c32-118">**Treknraksts** *un slīpraksts* ir -ok</span><span class="sxs-lookup"><span data-stu-id="24c32-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="24c32-119">Saites vienmēr ir vai nu **"saites uz web" / ārējo** vai **dziļi saites uz UI elementiem,** nevis iekšējās saites.</span><span class="sxs-lookup"><span data-stu-id="24c32-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="24c32-120">Attēli pašlaik netiek oficiāli atbalstīti, bet tie ir ceļvedī.</span><span class="sxs-lookup"><span data-stu-id="24c32-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="24c32-121">Un tas tiešām jau mazliet par garu.</span><span class="sxs-lookup"><span data-stu-id="24c32-121">And this is really already a bit too long.</span></span> <span data-ttu-id="24c32-122">Labākā prakse ir aptuveni 400 rakstzīmes ---------------------------------</span><span class="sxs-lookup"><span data-stu-id="24c32-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="24c32-123">Kad saturs ir gatavs, pavelciet to uz tiešo zaru.</span><span class="sxs-lookup"><span data-stu-id="24c32-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="24c32-124">Pēc tam dodieties [uz alchemy partneru portāls](https://alchemyportal.azurewebsites.net) un ievadiet faila nosaukumu url laukā.</span><span class="sxs-lookup"><span data-stu-id="24c32-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 