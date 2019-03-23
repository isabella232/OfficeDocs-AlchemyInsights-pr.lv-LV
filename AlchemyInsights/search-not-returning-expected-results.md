---
title: 1491-Search-not-Returning-Expected-Results
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 1491
ms.assetid: ''
ms.openlocfilehash: 517d9b75fc3aef09c0c2d5870aa695cc0ab10f06
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/22/2019
ms.locfileid: "30776088"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="b3b74-102">Satura meklēšana nav atgriešanās gaidāmie rezultāti</span><span class="sxs-lookup"><span data-stu-id="b3b74-102">Content Search not returning expected results</span></span>

<span data-ttu-id="b3b74-103">Braucot satura meklēšanu no & biroja 365 drošības ievērošanu centrs var saņemt negaidītu meklēšanas rezultātus.</span><span class="sxs-lookup"><span data-stu-id="b3b74-103">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="b3b74-104">Apsveriet šādas lietas, kas var ietekmēt meklēšanas rezultātus:</span><span class="sxs-lookup"><span data-stu-id="b3b74-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="b3b74-105">**Satura atrašanās vietu un meklēšanas nosacījumus**: Pārliecinieties, vai esat izvēlējies atbilstošu satura atrašanās vietu un meklēšanas nosacījumiem.</span><span class="sxs-lookup"><span data-stu-id="b3b74-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="b3b74-106">Ja jūs vadīja lielu meklēšanas (ar daudzām vietām), uzskata, sadalot to vairākās meklēšanas.</span><span class="sxs-lookup"><span data-stu-id="b3b74-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="b3b74-107">**Daļēji indeksē vienumus**: [daļēji indeksē vienumus](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) no pastkastes paredzamo meklēšanas rezultātos tiek iekļautas.</span><span class="sxs-lookup"><span data-stu-id="b3b74-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="b3b74-108">Tomēr daļēji indeksē vienumus no vietas savā SharePoint un OneDrive netiek iekļauti meklēšanas budžetu.</span><span class="sxs-lookup"><span data-stu-id="b3b74-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="b3b74-109">**Meklēšanas kļūmes**: meklējot lielu skaitu pastkastītes (vairāk nekā 100000 pastkastes), jūs varat saņemt meklēšanas kļūdas, kļūdas kodus, piem., CS008-009 un CS012-002).</span><span class="sxs-lookup"><span data-stu-id="b3b74-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="b3b74-110">Šādā gadījumā mēģiniet vēlreiz tikai meklēt neizdevās satura atrašanās vietu.</span><span class="sxs-lookup"><span data-stu-id="b3b74-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="b3b74-111">Skatiet [šajā rakstā](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) plašāku informāciju.</span><span class="sxs-lookup"><span data-stu-id="b3b74-111">See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
