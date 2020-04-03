---
title: Nosacījumpiekļuves politikas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: 8ce41d007988f2a45f1ded385ae50ac3def97c1b
ms.sourcegitcommit: 9923ce61344e22c4490549b12f65fa2896490b1f
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/01/2020
ms.locfileid: "43100512"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="13294-102">Nosacījumpiekļuves politikas</span><span class="sxs-lookup"><span data-stu-id="13294-102">Conditional Access policies</span></span>

<span data-ttu-id="13294-103">Nosacījumpiekļuves iespēja ir Azure AD iespēja, kas ļauj ieviest vadīklas piekļuvei programmām jūsu vidē, ņemot vērā noteiktus nosacījumus, kas tiek pārvaldīti no centrālās atrašanās vietas.</span><span class="sxs-lookup"><span data-stu-id="13294-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="13294-104">Papildinformācija par [Azure AD nosacījuma piekļuvi](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="13294-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="13294-105">**Piezīme**: Ja jūsu nomnieks tika izveidots pēc 2019. gada 21. oktobra un jūs pēkšņi MFA uzvedni, visticamāk jūsu nomniekam ir iespējoti [drošības noklusējumi](http://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="13294-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](http://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="13294-106">**Lai pārvaldītu drošības noklusējumus**</span><span class="sxs-lookup"><span data-stu-id="13294-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="13294-107">Pierakstieties [administrēšanas centrā](https://go.microsoft.com/fwlink/p/?linkid=834822), izmantojot globālā administratora akreditācijas datus.</span><span class="sxs-lookup"><span data-stu-id="13294-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="13294-108">Dodieties uz [Azure Active direktorija rekvizītiem](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="13294-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="13294-109">Lapas apakšdaļā noklikšķiniet uz **Drošības noklusējumu pārvaldība**.</span><span class="sxs-lookup"><span data-stu-id="13294-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="13294-110">Noklikšķiniet uz **Jā**, lai iespējotu drošības noklusējumus vai uz **Nē**, lai atspējotu drošības noklusējumus.</span><span class="sxs-lookup"><span data-stu-id="13294-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
