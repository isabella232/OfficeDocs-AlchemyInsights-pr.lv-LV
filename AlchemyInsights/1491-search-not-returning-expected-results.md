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
ms.custom: Adm_O365
ms.assetid: ''
ms.openlocfilehash: 881a579d7098578452c994b7ac66fe22a1d90dc2
ms.sourcegitcommit: 5182c9a73641079be59740e4524434b2e8be613a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29964911"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="1d222-102">Satura meklēšana nav atgriešanās gaidāmie rezultāti</span><span class="sxs-lookup"><span data-stu-id="1d222-102">Content Search not returning expected results</span></span>

<span data-ttu-id="1d222-p101">Braucot satura meklēšanu no & biroja 365 drošības ievērošanu centrs var saņemt negaidītu meklēšanas rezultātus. Apsveriet šādas lietas, kas var ietekmēt meklēšanas rezultātus:</span><span class="sxs-lookup"><span data-stu-id="1d222-p101">When running Content Searches from the Office 365 Security & Compliance Center, you may receive unexpected search results. Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="1d222-p102">**Satura atrašanās vietu un meklēšanas nosacījumus**: Pārliecinieties, vai esat izvēlējies atbilstošu satura atrašanās vietu un meklēšanas nosacījumiem. Ja jūs vadīja lielu meklēšanas (ar daudzām vietām), uzskata, sadalot to vairākās meklēšanas.</span><span class="sxs-lookup"><span data-stu-id="1d222-p102">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions. If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="1d222-p103">**Daļēji indeksē vienumus**: [daļēji indeksē vienumus](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) no pastkastes paredzamo meklēšanas rezultātos tiek iekļautas. Tomēr daļēji indeksē vienumus no vietas savā SharePoint un OneDrive netiek iekļauti meklēšanas budžetu.</span><span class="sxs-lookup"><span data-stu-id="1d222-p103">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/office365/securitycompliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results. However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="1d222-p104">**Meklēšanas kļūmes**: meklējot lielu skaitu pastkastītes (vairāk nekā 100000 pastkastes), jūs varat saņemt meklēšanas kļūdas, kļūdas kodus, piem., CS008-009 un CS012-002). Šādā gadījumā mēģiniet vēlreiz tikai meklēt neizdevās satura atrašanās vietu. Skatiet [šajā rakstā](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) plašāku informāciju.</span><span class="sxs-lookup"><span data-stu-id="1d222-p104">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002). In this case, retry the search only for the failed content locations. See  [this article](https://docs.microsoft.com/office365/securitycompliance/retry-failed-content-search) for more information.</span></span>
