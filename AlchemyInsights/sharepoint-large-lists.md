---
title: SharePoint lieli saraksti
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: e85686788c60d365a00970e9ffe58e97512894a3
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43767292"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="089d3-102">Strādājiet ar lieliem sarakstiem un bibliotēkām programmā SharePoint</span><span class="sxs-lookup"><span data-stu-id="089d3-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="089d3-103">SharePoint sarakstiem un bibliotēkām var būt līdz pat 30 000 000 vienumiem, bet, ja tiem ir vairāk par 5 000 vienumiem, iespējams, redzēsit saraksta skata sliekšņa kļūdu, kad mēģināsit ar tiem strādāt.</span><span class="sxs-lookup"><span data-stu-id="089d3-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="089d3-104">Šī sliekšņa mērķis ir uzturēt pakalpojuma veiktspēju.</span><span class="sxs-lookup"><span data-stu-id="089d3-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="089d3-105">To nevar mainīt.</span><span class="sxs-lookup"><span data-stu-id="089d3-105">It can't be changed.</span></span> <span data-ttu-id="089d3-106">Lai izvairītos no hitting šo slieksni:</span><span class="sxs-lookup"><span data-stu-id="089d3-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="089d3-107">**Izmantot modernas**</span><span class="sxs-lookup"><span data-stu-id="089d3-107">**Use modern**</span></span>

<span data-ttu-id="089d3-108">Skati, kuros redzami daudzi vienumi, vislabāk darbojas mūsdienu pieredzē.</span><span class="sxs-lookup"><span data-stu-id="089d3-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="089d3-109">[Izmantojiet moderno pieredzi](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , lai izvairītos no kļūdām, kuras varētu būt redzamas klasiskajā pieredzē.</span><span class="sxs-lookup"><span data-stu-id="089d3-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="089d3-110">**Indeksu pievienošana**</span><span class="sxs-lookup"><span data-stu-id="089d3-110">**Add indexes**</span></span>

<span data-ttu-id="089d3-111">Ja filtrējat vai kārtojat pēc kolonnas, kurai nav indeksa, iespējams, redzēsit kļūdas ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="089d3-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="089d3-112">[Pievienojiet alfabētisko rādītāju](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manuāli no **saraksta iestatījumi** izvēlnē Iestatījumi, pēc tam **indeksētas kolonnas**.</span><span class="sxs-lookup"><span data-stu-id="089d3-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="089d3-113">**Saraksta skata rediģēšana**</span><span class="sxs-lookup"><span data-stu-id="089d3-113">**Edit the list view**</span></span>

<span data-ttu-id="089d3-114">Ja rodas kļūda, strādājot ar lielu sarakstu, [rediģējiet saraksta skatu](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="089d3-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="089d3-115">Šīs četras izmaiņas noņems saraksta skata slieksnis kļūdas.</span><span class="sxs-lookup"><span data-stu-id="089d3-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="089d3-116">Veiciet visas četras izmaiņas, lai noņemtu visas kļūdas.</span><span class="sxs-lookup"><span data-stu-id="089d3-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="089d3-117">Ja joprojām saņemat kļūdas, pārbaudiet [pārvaldīt lielus sarakstus un bibliotēkas](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="089d3-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="089d3-118">Atlasiet **nav** no **kolonnas pirmā kārtošana** un **pēc tam kārtojiet pēc kolonnas**.</span><span class="sxs-lookup"><span data-stu-id="089d3-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="089d3-119">Kolonnā atlasiet **neviens** no **pirmās grupas** un **pēc tam grupējiet pēc kolonnas**.</span><span class="sxs-lookup"><span data-stu-id="089d3-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="089d3-120">Atlasiet **nav** visām kolonnām sadaļā **kopsummas** .</span><span class="sxs-lookup"><span data-stu-id="089d3-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="089d3-121">Noņemiet atzīmi no visas, izņemot vienu kolonnu, lai parādītu no **slejas** sadaļa.</span><span class="sxs-lookup"><span data-stu-id="089d3-121">Deselect all but one column for display from the **Columns** section.</span></span>

