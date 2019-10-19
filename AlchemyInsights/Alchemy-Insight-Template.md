---
title: pats, kas faila nosaukums ir labākais
ms.author: pebaum
author: pebaum
manager: jackiesm
ms.date: 4/27/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: (guid of old soc version if any)
ms.openlocfilehash: 31a578800468e9f3a69fff4f6e2e1945943c779c
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "35800052"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="d0e8a-102">Nepieciešamā Alchemy header H1, H2's nestrādā.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="d0e8a-103">Alchemy autorēšanas paraugprakse un vadlīnijas:</span><span class="sxs-lookup"><span data-stu-id="d0e8a-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="d0e8a-104">**Neligzdot Alchemy ieskatu mapēs**-tas būs pārtraukums URL struktūru.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="d0e8a-105">Mēs meklējam nosaka to.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="d0e8a-106">Failus mapē **Alchemyinsights** jābūt mazo failu nosaukumiem ar defises atstarpēm ex.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="d0e8a-107">***kā-to-Enable-tiesvedība-turiet***.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="d0e8a-108">Iekļaujiet kārtulas ID vai kopuma ID no [Alchemy partneru portāla](https://alchemyportal.azurewebsites.net) MS. Custom laukā.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="d0e8a-109">Ex.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-109">ex.</span></span> <span data-ttu-id="d0e8a-110">***MS. Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="d0e8a-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="d0e8a-111">Izmantot pārējos metadatus šī faila augšpusē kā veidni.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="d0e8a-112">[Alķīmijas partneru portālā](https://alchemyportal.azurewebsites.net)naviģējiet uz leju līdz sadaļai **Customer Insight nosaukums:** un izmantojiet to kā sākuma punktu savam H1 nosaukumam, lai iegūtu ieskatu.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="d0e8a-113">Alchemy ieskats ir jābūt tikai vienu H1 augšpusē vai tie saplīst ražošanā.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="d0e8a-114">H2s nepadara vai nu tik izmantot **treknrakstu** vai citas konvencijas, lai norādītu atsevišķas sadaļas.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="d0e8a-115">Pēc tam ievadiet pamattekstu, izmantojot melnrakstu materiālu sadaļā alķīmiju kārtulu lappuse</span><span class="sxs-lookup"><span data-stu-id="d0e8a-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="d0e8a-116">Aizzīmētie saraksti ir labi</span><span class="sxs-lookup"><span data-stu-id="d0e8a-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="d0e8a-117">Numurēti saraksti pārāk</span><span class="sxs-lookup"><span data-stu-id="d0e8a-117">Numbered lists too</span></span>
    1. <span data-ttu-id="d0e8a-118">**Treknraksts** un *Slīpraksts* ir-labi</span><span class="sxs-lookup"><span data-stu-id="d0e8a-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="d0e8a-119">Links vienmēr jābūt vai nu **"saites uz Web"/ārējo** vai **dziļi saites uz UI elementus**, nevis iekšējās saites.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="d0e8a-120">Šajā laikā attēli nav oficiāli atbalstīti, bet tas ir ceļvedī.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="d0e8a-121">Un tas ir patiešām jau mazliet par garu.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-121">And this is really already a bit too long.</span></span> <span data-ttu-id="d0e8a-122">Labākā prakse ir aptuveni 400 rakstzīmes---------------------------------</span><span class="sxs-lookup"><span data-stu-id="d0e8a-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="d0e8a-123">Kad saturs ir gatavs, izvelciet to uz tiešraides zaru.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="d0e8a-124">Pēc tam dodieties uz [Alchemy partneru portālu](https://alchemyportal.azurewebsites.net) un ievadiet faila nosaukumu laukā URL.</span><span class="sxs-lookup"><span data-stu-id="d0e8a-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> 