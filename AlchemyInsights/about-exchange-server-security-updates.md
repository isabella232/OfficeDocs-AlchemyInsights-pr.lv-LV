---
title: Par Exchange Server drošības atjauninājumiem
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005482"
- "9005483"
- "9413"
- "9412"
ms.openlocfilehash: 87a5cf1ac4dfb96a5406f6b1431adb6ead074fd6
ms.sourcegitcommit: 6741a997fff871d263f92d3ff7fb61e7755956a9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50481951"
---
# <a name="about-exchange-server-security-updates"></a><span data-ttu-id="8014c-102">Par Exchange Server drošības atjauninājumiem</span><span class="sxs-lookup"><span data-stu-id="8014c-102">About Exchange Server Security updates</span></span>

<span data-ttu-id="8014c-103">Microsoft ir izlaidusi vairākus kritiskos drošības atjauninājumus Exchange Server lokālajā vidē.</span><span class="sxs-lookup"><span data-stu-id="8014c-103">Microsoft has released a series of critical security updates for Exchange Server on-premises.</span></span> <span data-ttu-id="8014c-104">Ietekmētās servera versijas ir jebkurš Exchange Server 2010, 2013, 2016 un 2019 atjaunināšanas līmenis.</span><span class="sxs-lookup"><span data-stu-id="8014c-104">The affected server versions are any update levels of Exchange Server 2010, 2013, 2016 and 2019.</span></span> <span data-ttu-id="8014c-105">Exchange Online netiek ietekmēts, bet, ja jums ir daži lokāli Exchange serveri hibrīdās konfigurācijas dēļ, tie ir potenciāli neaizsargāti.</span><span class="sxs-lookup"><span data-stu-id="8014c-105">Exchange Online is NOT impacted, but if you have some on-premises Exchange servers due to Hybrid configuration, they are potentially vulnerable.</span></span>

<span data-ttu-id="8014c-106">Lai atjauninātu lokālos serverus, būs jādarbojas vismaz šādām Exchange versijām:</span><span class="sxs-lookup"><span data-stu-id="8014c-106">To update your on-premises servers will have to be running at least the following versions of Exchange:</span></span>

- <span data-ttu-id="8014c-107">Exchange 2010 3. servisa pakotne</span><span class="sxs-lookup"><span data-stu-id="8014c-107">Exchange 2010 Service Pack 3</span></span>
- <span data-ttu-id="8014c-108">Exchange Server 2013 CU 23</span><span class="sxs-lookup"><span data-stu-id="8014c-108">Exchange Server 2013 CU 23</span></span>
- <span data-ttu-id="8014c-109">Exchange Server 2016 CU 19 vai CU 18</span><span class="sxs-lookup"><span data-stu-id="8014c-109">Exchange Server 2016 CU 19 or CU 18</span></span>
- <span data-ttu-id="8014c-110">Exchange Server 2019 CU 8 vai CU 7</span><span class="sxs-lookup"><span data-stu-id="8014c-110">Exchange Server 2019 CU 8 or CU 7</span></span>

<span data-ttu-id="8014c-111">Lūdzu, skatiet tālāk norādīto paziņojumu par labojumu atrašanās vietu: [izlaists: 2021 Exchange Server drošības atjauninājumi](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span><span class="sxs-lookup"><span data-stu-id="8014c-111">Please see the following announcement for location of fixes: [Released: March 2021 Exchange Server Security Updates](https://techcommunity.microsoft.com/t5/exchange-team-blog/released-march-2021-exchange-server-security-updates/ba-p/2175901)</span></span>

<span data-ttu-id="8014c-112">**Svarīgas piezīmes:**</span><span class="sxs-lookup"><span data-stu-id="8014c-112">**Important notes:**</span></span>

<span data-ttu-id="8014c-113">Atjauninājumu instalēšana nedarbosies, ja jūsu lokālajos serveros nedarbojas nepieciešamās Exchange versijas, kā norādīts iepriekš minētajā sarakstā.</span><span class="sxs-lookup"><span data-stu-id="8014c-113">Installation of updates will not work if your on-premises servers are not running required Exchange versions, as per the above list.</span></span>

<span data-ttu-id="8014c-114">Ja atjauninājumu instalēšana notiek manuāli, lūdzu, izlasiet sadaļu "zināmās problēmas" atjauniniet KB rakstu, lai iegūtu svarīgu informāciju.</span><span class="sxs-lookup"><span data-stu-id="8014c-114">If installing updates manually, please read the "Known issues" section of update KB articles for important information.</span></span> <span data-ttu-id="8014c-115">Drošības atjauninājumi ir jāpalaiž no paaugstināta CMD/PowerShell uzvednes.</span><span class="sxs-lookup"><span data-stu-id="8014c-115">Security updates MUST be run from elevated CMD/PowerShell prompt!</span></span>
