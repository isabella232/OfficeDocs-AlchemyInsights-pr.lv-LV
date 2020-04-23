---
title: Neparedzēta daudzfaktoru autentifikācija
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: ''
ms.custom:
- "1300007"
- "4372"
ms.openlocfilehash: a664bd709062ec1335ebcf1f9adddc8aef917ac1
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43766608"
---
# <a name="unexpected-multi-factor-authentication"></a><span data-ttu-id="54bbc-102">Neparedzēta daudzfaktoru autentifikācija</span><span class="sxs-lookup"><span data-stu-id="54bbc-102">Unexpected multi-factor authentication</span></span>

<span data-ttu-id="54bbc-103">Ja jūsu nomnieks tika izveidots pēc 2019. gada 21. oktobra un jūs pēkšņi MFA uzvedni, visticamāk jūsu nomniekam ir iespējoti [drošības noklusējumi](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="54bbc-103">If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span> 

<span data-ttu-id="54bbc-104">Lai pārvaldītu drošības noklusējumus:</span><span class="sxs-lookup"><span data-stu-id="54bbc-104">To Manage security defaults:</span></span>

1. <span data-ttu-id="54bbc-105">Pierakstieties [administrēšanas centrā](https://go.microsoft.com/fwlink/p/?linkid=834822), izmantojot globālā administratora akreditācijas datus.</span><span class="sxs-lookup"><span data-stu-id="54bbc-105">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="54bbc-106">Dodieties uz [Azure Active direktorija rekvizītiem](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="54bbc-106">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="54bbc-107">Lapas apakšdaļā noklikšķiniet uz **Drošības noklusējumu pārvaldība**.</span><span class="sxs-lookup"><span data-stu-id="54bbc-107">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="54bbc-108">Noklikšķiniet uz **Jā**, lai iespējotu drošības noklusējumus, un uz **Nē**, lai atspējotu drošības noklusējumus.</span><span class="sxs-lookup"><span data-stu-id="54bbc-108">Click **Yes** to enable security defaults and **No** to disable security defaults.</span></span>
