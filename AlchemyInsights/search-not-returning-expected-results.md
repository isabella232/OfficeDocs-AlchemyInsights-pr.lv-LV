---
title: 1491-meklēšana-not-atgriešanās-sagaidāmais-rezultāti
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 57421d459ef03049d6f931db659a5f9b253f5002
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510579"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="c0c72-102">Satura meklēšana, kas neatgriež gaidtos rezultātus</span><span class="sxs-lookup"><span data-stu-id="c0c72-102">Content Search not returning expected results</span></span>

<span data-ttu-id="c0c72-103">Palaižot satura meklēšanu no Microsoft 365 drošības & atbilstības centrs, var tikt parādīts negaidīti meklēšanas rezultātos.</span><span class="sxs-lookup"><span data-stu-id="c0c72-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="c0c72-104">Apsveriet tālāk norādītās darbības, kas var ietekmēt meklēšanas rezultātus.</span><span class="sxs-lookup"><span data-stu-id="c0c72-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="c0c72-105">**Satura atrašanās vietas un meklēšanas nosacījumi**: pārliecinieties, vai esat atlasījis pareizās satura atrašanās vietas un meklēšanas nosacījumus.</span><span class="sxs-lookup"><span data-stu-id="c0c72-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="c0c72-106">Ja jums bija liela meklēšana (ar daudzām atrašanās vietām), apsveriet to sadalīšanu vairākās meklēšanām.</span><span class="sxs-lookup"><span data-stu-id="c0c72-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="c0c72-107">**Daļēji indeksēts vienumus**: [daļēji indeksētu vienumus](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) no pastkastēm tiek iekļauti aptuvenā meklēšanas rezultātos.</span><span class="sxs-lookup"><span data-stu-id="c0c72-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="c0c72-108">Tomēr daļēji indeksētu vienumus no vietnes SharePoint un OneDrive nav iekļauti meklēšanas novērtējums.</span><span class="sxs-lookup"><span data-stu-id="c0c72-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="c0c72-109">**Meklēšanas kļūmes**: meklējot lielu skaitu pastkastu (vairāk nekā 100 000 pastkastes), var tikt parādīts meklēšanas kļūdas ar kļūdu kodiem, piemēram, CS008-009 un CS012-002).</span><span class="sxs-lookup"><span data-stu-id="c0c72-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="c0c72-110">Šādā gadījumā vēlreiz mēģiniet meklēt tikai neizdevušos satura atrašanās vietas.</span><span class="sxs-lookup"><span data-stu-id="c0c72-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="c0c72-111">Skatiet [šo rakstu](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) , lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="c0c72-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
