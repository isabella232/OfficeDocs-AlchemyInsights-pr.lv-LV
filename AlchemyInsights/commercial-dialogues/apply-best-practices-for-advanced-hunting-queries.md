---
title: Labākās medību vaicājumu metodes lietošana
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: cd13e2e8801db3df91140ce371813d900d72e38b
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746185"
---
# <a name="apply-best-practices-for-advanced-hunting-queries"></a><span data-ttu-id="15a4a-102">Labākās medību vaicājumu metodes lietošana</span><span class="sxs-lookup"><span data-stu-id="15a4a-102">Apply best practices for advanced hunting queries</span></span>

<span data-ttu-id="15a4a-103">Lai iegūtu rezultātus ātrāk un lai izvairītos no taimautiem, palaižot sarežģītus vaicājumus, lietojiet šīs paraugprakses:</span><span class="sxs-lookup"><span data-stu-id="15a4a-103">To get results faster and to avoid timeouts while running complex queries, apply these best practices:</span></span>

- <span data-ttu-id="15a4a-104">Mēģinot izveidot jaunus vaicājumus, vienmēr izmantojiet ierobežojumu, lai izvairītos no ļoti lielām rezultātu kopām.</span><span class="sxs-lookup"><span data-stu-id="15a4a-104">When trying new queries, always use a limit, to avoid getting extremely large result sets.</span></span> <span data-ttu-id="15a4a-105">Izmantojiet arī, `count` lai veiktu sākotnējā rezultātu kopas lieluma novērtējumu.</span><span class="sxs-lookup"><span data-stu-id="15a4a-105">Also, use `count` to make an initial assessment of the result set's size.</span></span>
- <span data-ttu-id="15a4a-106">Vispirms izmantojiet laika filtrus.</span><span class="sxs-lookup"><span data-stu-id="15a4a-106">Use time filters first.</span></span> <span data-ttu-id="15a4a-107">Ideāli ierobežojiet vaicājumus līdz septiņām dienām.</span><span class="sxs-lookup"><span data-stu-id="15a4a-107">Ideally, limit your queries to seven days.</span></span>
- <span data-ttu-id="15a4a-108">Vaicājuma sākumā uzreiz pēc laika filtra pievienojiet filtrus, lai noņemtu lielāko daļu datu.</span><span class="sxs-lookup"><span data-stu-id="15a4a-108">In the beginning of a query, right after the time filter, add the filters expected to remove most of the data.</span></span>
- <span data-ttu-id="15a4a-109">Meklējot pilnas marķierierīces, izmantojiet `has` operatoru, nevis `contains` .</span><span class="sxs-lookup"><span data-stu-id="15a4a-109">When looking for full tokens, use the `has` operator rather than `contains`.</span></span>
- <span data-ttu-id="15a4a-110">Veiciet meklēšanu noteiktā kolonnā, nevis visās kolonnās.</span><span class="sxs-lookup"><span data-stu-id="15a4a-110">Run a search on a specific column rather than across all columns.</span></span>
- <span data-ttu-id="15a4a-111">Savienojot tabulas, vispirms norādiet tabulu, kurā ir mazāk rindu.</span><span class="sxs-lookup"><span data-stu-id="15a4a-111">When joining tables, first specify the table with fewer rows.</span></span>
- <span data-ttu-id="15a4a-112">`project` tikai nepieciešamās tabulas no Savienotajām tabulām.</span><span class="sxs-lookup"><span data-stu-id="15a4a-112">`project` only the necessary columns from the tables you've joined.</span></span>

<span data-ttu-id="15a4a-113">Lai uzzinātu vairāk, skatiet rakstu [papildu medību vaicājumu labākā prakse](https://go.microsoft.com/fwlink/?linkid=2144812).</span><span class="sxs-lookup"><span data-stu-id="15a4a-113">To learn more, see [Advanced hunting query best practices](https://go.microsoft.com/fwlink/?linkid=2144812).</span></span>
