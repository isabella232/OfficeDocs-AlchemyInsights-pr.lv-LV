---
title: SharePoint lielie saraksti
ms.author: toresing
author: tomresing
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "407"
- "530001"
ms.assetid: ee07bf74-7aeb-4c47-8f5d-f496d6c09d79
ms.openlocfilehash: 1bc891a912c6753ea6c85d7d4b2a5d802080bd5c
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720140"
---
# <a name="work-with-large-lists-and-libraries-in-sharepoint"></a><span data-ttu-id="aa36d-102">Darbs ar lieliem sarakstiem un bibliotēkām pakalpojumā SharePoint</span><span class="sxs-lookup"><span data-stu-id="aa36d-102">Work with large lists and libraries in SharePoint</span></span>

<span data-ttu-id="aa36d-103">SharePoint sarakstos un bibliotēkās var būt ne vairāk kā 30 000 000 vienumi, bet, ja tiem ir vairāk nekā 5 000 vienumu, iespējams, būs redzama saraksta skata sliekšņa kļūda, kad mēģināt ar tiem strādāt.</span><span class="sxs-lookup"><span data-stu-id="aa36d-103">SharePoint lists and libraries can contain up to 30 million items, but when they have more than 5,000 items, you might see a List View Threshold error when you try to work with them.</span></span> <span data-ttu-id="aa36d-104">Šī sliekšņa mērķis ir uzturēt pakalpojuma veiktspēju.</span><span class="sxs-lookup"><span data-stu-id="aa36d-104">This threshold is in place to maintain performance of the service.</span></span> <span data-ttu-id="aa36d-105">To nevar mainīt.</span><span class="sxs-lookup"><span data-stu-id="aa36d-105">It can't be changed.</span></span> <span data-ttu-id="aa36d-106">Lai izvairītos no šī sliekšņa sišanas:</span><span class="sxs-lookup"><span data-stu-id="aa36d-106">To avoid hitting this threshold:</span></span>

<span data-ttu-id="aa36d-107">**Moderna izmantošana**</span><span class="sxs-lookup"><span data-stu-id="aa36d-107">**Use modern**</span></span>

<span data-ttu-id="aa36d-108">Skati, kas rāda daudzus vienumus, vislabāk darbojas mūsdienīgajā pieredzē.</span><span class="sxs-lookup"><span data-stu-id="aa36d-108">Views showing many items work best in the modern experience.</span></span> <span data-ttu-id="aa36d-109">[Izmantojiet mūsdienīgu pieredzi](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) , lai izvairītos no kļūdām, kuras var būt redzamas klasiskajā pieredzē.</span><span class="sxs-lookup"><span data-stu-id="aa36d-109">[Use the modern experience](https://support.office.com/article/66dac24b-4177-4775-bf50-3d267318caa9) to avoid errors you might see in the classic experience.</span></span>

<span data-ttu-id="aa36d-110">**Indeksu pievienošana**</span><span class="sxs-lookup"><span data-stu-id="aa36d-110">**Add indexes**</span></span>

<span data-ttu-id="aa36d-111">Ja filtrējat vai kārtojat pēc kolonnas, kurā nav indeksa, iespējams, tiks parādīts kļūdas ziņojums.</span><span class="sxs-lookup"><span data-stu-id="aa36d-111">When you filter or sort by a column that doesn't have an index, you might see an error message.</span></span> <span data-ttu-id="aa36d-112">Manuāli [pievienojiet indeksu](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) no **saraksta iestatījumiem** izvēlnē Iestatījumi un pēc tam **Indeksētās kolonnas**.</span><span class="sxs-lookup"><span data-stu-id="aa36d-112">[Add an index](https://support.office.com/article/f3f00554-b7dc-44d1-a2ed-d477eac463b0) manually from **List Settings** in the settings menu, then **Indexed Columns**.</span></span>

<span data-ttu-id="aa36d-113">**Saraksta skata rediģēšana**</span><span class="sxs-lookup"><span data-stu-id="aa36d-113">**Edit the list view**</span></span>

<span data-ttu-id="aa36d-114">Ja, strādājot ar lielu sarakstu, rodas kļūda, [rediģējiet saraksta skatu](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span><span class="sxs-lookup"><span data-stu-id="aa36d-114">If an error occurs when working with a large list, [edit your list view](https://support.office.com/article/15916903-e79a-423f-b4e2-02d37e1ff372).</span></span>

<span data-ttu-id="aa36d-115">Veicot šīs četras izmaiņas, tiek noņemtas saraksta skata sliekšņa kļūdas.</span><span class="sxs-lookup"><span data-stu-id="aa36d-115">The following four changes will remove list view threshold errors.</span></span> <span data-ttu-id="aa36d-116">Veiciet visas četras izmaiņas, lai noņemtu visas kļūdas.</span><span class="sxs-lookup"><span data-stu-id="aa36d-116">Make all four changes to remove all errors.</span></span> <span data-ttu-id="aa36d-117">Ja joprojām tiek saņemtas kļūdas, atzīmējiet rūtiņu [Pārvaldīt lielus sarakstus un bibliotēkas](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span><span class="sxs-lookup"><span data-stu-id="aa36d-117">If you are still getting errors, check [Manage large lists and libraries](https://support.office.com/article/B8588DAE-9387-48C2-9248-C24122F07C59).</span></span>

1. <span data-ttu-id="aa36d-118">Atlasiet **nav** no **pirmā kārtot pēc kolonnas** un **pēc tam kārtojiet pēc kolonnas**.</span><span class="sxs-lookup"><span data-stu-id="aa36d-118">Select **None** from both **First sort by the column** and **Then sort by the column**.</span></span>
2. <span data-ttu-id="aa36d-119">Atlasiet **neviens** no **kolonnas pirmais grupā** un **pēc tam grupēt pēc kolonnas**.</span><span class="sxs-lookup"><span data-stu-id="aa36d-119">Select **None** from both **First group by the column** and **Then group by the column**.</span></span>
3. <span data-ttu-id="aa36d-120">Atlasiet **nav** visām kolonnām sadaļā **kopsummas** .</span><span class="sxs-lookup"><span data-stu-id="aa36d-120">Select **None** for all columns in the **Totals** section.</span></span>
4. <span data-ttu-id="aa36d-121">Noņemiet atlasi visām, izņemot vienu kolonnu parādīšanai no **kolonnu** sadaļas.</span><span class="sxs-lookup"><span data-stu-id="aa36d-121">Deselect all but one column for display from the **Columns** section.</span></span>

