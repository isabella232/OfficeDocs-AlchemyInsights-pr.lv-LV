---
title: Tāpat kā filename ir labākais
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
ms.openlocfilehash: 37398436435fb72cb5c8dca2d0798b86a0c8ccc9
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/22/2019
ms.locfileid: "30762071"
---
# <a name="required-alchemy-header-h1-h2s-dont-work"></a><span data-ttu-id="04c7a-102">Vajadzīga alķīmija Header H1, H2 ir nestrādā.</span><span class="sxs-lookup"><span data-stu-id="04c7a-102">Required Alchemy Header H1, H2's dont work.</span></span>
<span data-ttu-id="04c7a-103">Labāko praksi un pamatnostādnēm par alķīmiju autorēšanas:</span><span class="sxs-lookup"><span data-stu-id="04c7a-103">Best Practices and guidelines for Alchemy authoring:</span></span>

1. <span data-ttu-id="04c7a-104">**Neligzdo Alchemy atziņas mapēs**- tas saplīst url struktūru.</span><span class="sxs-lookup"><span data-stu-id="04c7a-104">**Do not nest Alchemy Insights in folders**- this will break the url structure.</span></span> <span data-ttu-id="04c7a-105">Mēs meklēja šo noteikšanu.</span><span class="sxs-lookup"><span data-stu-id="04c7a-105">We're looking into fixing this.</span></span>
1. <span data-ttu-id="04c7a-106">Failus mapē **AlchemyInsights** vajadzētu būt mazie filenames ar telpām ex pārnesumzīmes.</span><span class="sxs-lookup"><span data-stu-id="04c7a-106">Files in the **AlchemyInsights** folder should have lowercase filenames with hyphens for spaces ex.</span></span> <span data-ttu-id="04c7a-107">***how-to-enable-tiesvedības-turiet***.</span><span class="sxs-lookup"><span data-stu-id="04c7a-107">***how-to-enable-litigation-hold***.</span></span>
    1. <span data-ttu-id="04c7a-108">Ietver kārtulas ID vai kopuma ID no [alķīmijas partneru portāla](https://alchemyportal.azurewebsites.net) ms.custom laukā.</span><span class="sxs-lookup"><span data-stu-id="04c7a-108">Include the Rule ID or bucket ID from the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) in the ms.custom field.</span></span> <span data-ttu-id="04c7a-109">ex.</span><span class="sxs-lookup"><span data-stu-id="04c7a-109">ex.</span></span> <span data-ttu-id="04c7a-110">***MS.Custom: 100021***</span><span class="sxs-lookup"><span data-stu-id="04c7a-110">***ms.custom: 100021***</span></span>
1. <span data-ttu-id="04c7a-111">Izmantot metadatu atlikušo augšpusē šo failu kā veidnei.</span><span class="sxs-lookup"><span data-stu-id="04c7a-111">Use the rest of the metadata at the top of this file as your template.</span></span>
1. <span data-ttu-id="04c7a-112">[Alchemy partneru portāla](https://alchemyportal.azurewebsites.net)virzītos uz leju līdz sadaļai **klientu ieskatu nosaukums:** un izmantot šo kā sākuma punkts H1 titra par ieskatu.</span><span class="sxs-lookup"><span data-stu-id="04c7a-112">In the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net), navigate down to the section **Customer Insight Title:** and use that as a starting point for your H1 title for the insight.</span></span> 
    > [!NOTE]
    > <span data-ttu-id="04c7a-113">Alķīmijas atziņas ir jābūt tikai vienu H1 augšpusē vai viņi pārtrauks ražošanu.</span><span class="sxs-lookup"><span data-stu-id="04c7a-113">Alchemy Insights MUST have only a single H1 at the top or they will break in production.</span></span> <span data-ttu-id="04c7a-114">H2s nepadara tik lietot **treknraksta** vai citām konvencijām neizsaka atsevišķās sekcijās.</span><span class="sxs-lookup"><span data-stu-id="04c7a-114">H2s dont render either so use **bold** or other conventions to signify separate sections.</span></span>
1. <span data-ttu-id="04c7a-115">Pēc tam aizpildiet pamattekstu, izmantojot iesaukumam Alchemy noteikums lapas sadaļā klientu atziņas</span><span class="sxs-lookup"><span data-stu-id="04c7a-115">Next, fill in the body text using the draft material in the Customer Insights section of the Alchemy Rule page</span></span>
    1. <span data-ttu-id="04c7a-116">Aizzīmētiem sarakstiem ir smalka</span><span class="sxs-lookup"><span data-stu-id="04c7a-116">Bulleted lists are fine</span></span>
    1. <span data-ttu-id="04c7a-117">Numurētus sarakstus pārāk</span><span class="sxs-lookup"><span data-stu-id="04c7a-117">Numbered lists too</span></span>
    1. <span data-ttu-id="04c7a-118">**Treknraksts** un *kursīvs* , tiek a-ok</span><span class="sxs-lookup"><span data-stu-id="04c7a-118">**Bold** and *italic* are a-ok</span></span>
    1. <span data-ttu-id="04c7a-119">Saites, vienmēr ir jābūt vai nu **"uz web saites" / ārējo** vai **dziļas saites uz lietotāja interfeisa elementus**, nevis iekšējās saites.</span><span class="sxs-lookup"><span data-stu-id="04c7a-119">Links should always be either **"links to web"/external** OR **deep-links to UI elements**, not internal links.</span></span>
    1. <span data-ttu-id="04c7a-120">Attēli nav oficiāli atbalstīti šajā laikā, bet tas ir par plānu.</span><span class="sxs-lookup"><span data-stu-id="04c7a-120">Pictures are not officially supported at this time, but it's on the roadmap.</span></span>

<span data-ttu-id="04c7a-121">Un tas tiešām jau ir mazliet pārāk ilgi.</span><span class="sxs-lookup"><span data-stu-id="04c7a-121">And this is really already a bit too long.</span></span> <span data-ttu-id="04c7a-122">Vislabākā prakse ir apmēram 400 rakstzīmēm--</span><span class="sxs-lookup"><span data-stu-id="04c7a-122">Best practice is about 400 characters ---------------------------------</span></span>

<span data-ttu-id="04c7a-123">Kad jūsu lapa ir gatava, izvelciet to dzīvu zaru.</span><span class="sxs-lookup"><span data-stu-id="04c7a-123">Once your content is ready, pull it to the live branch.</span></span> <span data-ttu-id="04c7a-124">Pēc tam [Alchemy partneru portālā](https://alchemyportal.azurewebsites.net) un url laukā ievadiet faila nosaukumu.</span><span class="sxs-lookup"><span data-stu-id="04c7a-124">Then, go to the [Alchemy Partner portal](https://alchemyportal.azurewebsites.net) and enter the filename into the url field.</span></span> <span data-ttu-id="04c7a-125">M</span><span class="sxs-lookup"><span data-stu-id="04c7a-125">M</span></span>