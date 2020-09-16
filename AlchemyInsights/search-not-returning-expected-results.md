---
title: 1491 — meklēšana — netiek atgriezti — sagaidāmie rezultāti
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1491"
- "3200003"
ms.assetid: ''
ms.openlocfilehash: 5c4452726c1dbe2232ee63e8a9ee4d089f5c76db
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47740481"
---
# <a name="content-search-not-returning-expected-results"></a><span data-ttu-id="886a3-102">Satura meklēšana neatgriež gaidītos rezultātus</span><span class="sxs-lookup"><span data-stu-id="886a3-102">Content Search not returning expected results</span></span>

<span data-ttu-id="886a3-103">Kad notiek satura meklēšana no Microsoft 365 drošības & atbilstības centra, iespējams, saņemsit negaidītus meklēšanas rezultātus.</span><span class="sxs-lookup"><span data-stu-id="886a3-103">When running Content Searches from the Microsoft 365 security & Compliance Center, you may receive unexpected search results.</span></span> <span data-ttu-id="886a3-104">Apsveriet tālāk norādītās darbības, kas var ietekmēt meklēšanas rezultātus.</span><span class="sxs-lookup"><span data-stu-id="886a3-104">Consider the following things that can affect your search results:</span></span>

- <span data-ttu-id="886a3-105">**Satura atrašanās vietas un meklēšanas nosacījumi**: Pārliecinieties, vai esat atlasījis atbilstošas satura atrašanās vietas un meklēšanas nosacījumus.</span><span class="sxs-lookup"><span data-stu-id="886a3-105">**Content locations and search conditions**: Make sure you have selected the proper content locations and search conditions.</span></span> <span data-ttu-id="886a3-106">Ja esat izpildījis lielu meklēšanu (ar daudzām atrašanās vietām), apsveriet iespēju to sadalīt vairākos meklējumos.</span><span class="sxs-lookup"><span data-stu-id="886a3-106">If you ran a large search (with many locations), consider splitting it into multiple searches.</span></span>

- <span data-ttu-id="886a3-107">**Daļēji indeksētie vienumi**: aprēķinātajos meklēšanas rezultātos tiek iekļauti  [daļēji indeksētie vienumi](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) no pastkastēm.</span><span class="sxs-lookup"><span data-stu-id="886a3-107">**Partially indexed items**:  [Partially indexed items](https://docs.microsoft.com/microsoft-365/compliance/partially-indexed-items-in-content-search) from mailboxes are included in the estimated search results.</span></span> <span data-ttu-id="886a3-108">Tomēr meklēšanas aplēsē nav iekļauta daļēji indeksētie vienumi no SharePoint un OneDrive vietnēm.</span><span class="sxs-lookup"><span data-stu-id="886a3-108">However, partially indexed items from sites in SharePoint and OneDrive aren't included in the search estimate.</span></span>

- <span data-ttu-id="886a3-109">**Meklēšanas kļūmes**: Ja meklējat lielu skaitu pastkastu (vairāk par 100 000 pastkastēm), varat saņemt meklēšanas kļūdas ar kļūdu kodiem, piemēram, CS008-009 un CS012-002).</span><span class="sxs-lookup"><span data-stu-id="886a3-109">**Search failures**: When searching a large number of mailboxes (over 100,000 mailboxes), you may get search errors, with error codes such as CS008-009 and CS012-002).</span></span> <span data-ttu-id="886a3-110">Šajā gadījumā atkārtoti mēģiniet meklēt tikai neveiksmīgajām satura atrašanās vietām.</span><span class="sxs-lookup"><span data-stu-id="886a3-110">In this case, retry the search only for the failed content locations.</span></span> <span data-ttu-id="886a3-111">Lai iegūtu papildinformāciju, skatiet  [šo rakstu](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) .</span><span class="sxs-lookup"><span data-stu-id="886a3-111">See  [this article](https://docs.microsoft.com/microsoft-365/compliance/retry-failed-content-search) for more information.</span></span>
