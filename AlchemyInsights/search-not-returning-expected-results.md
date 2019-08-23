---
title: 1491-Search-not-returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 094da9d75013aae56ca219b7ae03e85736ce5ee0
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551422"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="d89e6-102">Satura meklēšana nav atgriešanās gaidāmie rezultāti</span><span class="sxs-lookup"><span data-stu-id="d89e6-102">Content Search not returning expected results</span></span>

<span data-ttu-id="d89e6-103">Braucot satura meklēšanu no & biroja 365 drošības ievērošanu centrs var saņemt negaidītu meklēšanas rezultātus.</span><span class="sxs-lookup"><span data-stu-id="d89e6-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="d89e6-104">Apsveriet šādas lietas, kas var ietekmēt meklēšanas rezultātus:</span><span class="sxs-lookup"><span data-stu-id="d89e6-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="d89e6-105">**Satura atrašanās vietu un meklēšanas nosacījumus**: pārliecinieties, vai esat izvēlējies atbilstošu satura atrašanās vietu un meklēšanas nosacījumiem.</span><span class="sxs-lookup"><span data-stu-id="d89e6-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="d89e6-106">Ja jūs vadīja lielu meklēšanas (ar daudzām vietām), uzskata, sadalot to vairākās meklēšanas.</span><span class="sxs-lookup"><span data-stu-id="d89e6-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="d89e6-107">**Daļēji indeksē vienumus**: [daļēji indeksē vienumus](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) no pastkastes paredzamo meklēšanas rezultātos tiek iekļautas.</span><span class="sxs-lookup"><span data-stu-id="d89e6-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="d89e6-108">Tomēr daļēji indeksē vienumus no vietas savā SharePoint un OneDrive netiek iekļauti meklēšanas budžetu.</span><span class="sxs-lookup"><span data-stu-id="d89e6-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="d89e6-109">**Meklēšanas kļūmes**: meklējot lielu skaitu pastkastītes (vairāk nekā 100000 pastkastes), jūs varat saņemt meklēšanas kļūdas, kļūdas kodus, piem., CS008-009 un CS012-002).</span><span class="sxs-lookup"><span data-stu-id="d89e6-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="d89e6-110">Šādā gadījumā mēģiniet vēlreiz tikai meklēt neizdevās satura atrašanās vietu.</span><span class="sxs-lookup"><span data-stu-id="d89e6-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="d89e6-111">Skatiet [šajā rakstā](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) plašāku informāciju.</span><span class="sxs-lookup"><span data-stu-id="d89e6-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
