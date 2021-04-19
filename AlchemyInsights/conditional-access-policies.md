---
title: Nosacījumpiekļuves politikas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002357"
- "4583"
ms.openlocfilehash: af95627d07d41add54f03c9254562b9be4e05d9b
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51817287"
---
# <a name="conditional-access-policies"></a><span data-ttu-id="b1832-102">Nosacījumpiekļuves politikas</span><span class="sxs-lookup"><span data-stu-id="b1832-102">Conditional Access policies</span></span>

<span data-ttu-id="b1832-103">Nosacījumpiekļuves iespēja ir Azure AD iespēja, kas ļauj ieviest vadīklas piekļuvei programmām jūsu vidē, ņemot vērā noteiktus nosacījumus, kas tiek pārvaldīti no centrālās atrašanās vietas.</span><span class="sxs-lookup"><span data-stu-id="b1832-103">Conditional Access is a capability of Azure AD that enables you to enforce controls on the access to apps in your environment, all based on specific conditions and managed from a central location.</span></span>

<span data-ttu-id="b1832-104">Papildinformācija par [Azure AD nosacījuma piekļuvi](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span><span class="sxs-lookup"><span data-stu-id="b1832-104">Learn more about [Azure AD Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/).</span></span>  

<span data-ttu-id="b1832-105">**Piezīme**: Ja jūsu nomnieks tika izveidots pēc 2019. gada 21. oktobra un jūs pēkšņi MFA uzvedni, visticamāk jūsu nomniekam ir iespējoti [drošības noklusējumi](https://aka.ms/securitydefaults).</span><span class="sxs-lookup"><span data-stu-id="b1832-105">**Note**: If your tenant was created after October 21st, 2019 and you're unexpectedly getting prompted for MFA, you likely have [security defaults](https://aka.ms/securitydefaults) enabled in your tenant.</span></span>

<span data-ttu-id="b1832-106">**Lai pārvaldītu drošības noklusējumus**</span><span class="sxs-lookup"><span data-stu-id="b1832-106">**To Manage security defaults**</span></span>

1. <span data-ttu-id="b1832-107">Pierakstieties [administrēšanas centrā](https://go.microsoft.com/fwlink/p/?linkid=834822), izmantojot globālā administratora akreditācijas datus.</span><span class="sxs-lookup"><span data-stu-id="b1832-107">Sign in to the [admin center](https://go.microsoft.com/fwlink/p/?linkid=834822) with your Global admin credentials.</span></span>

2. <span data-ttu-id="b1832-108">Dodieties uz [Azure Active direktorija rekvizītiem](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span><span class="sxs-lookup"><span data-stu-id="b1832-108">Go to [Azure Active Directory Properties](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/Properties).</span></span>

3. <span data-ttu-id="b1832-109">Lapas apakšdaļā noklikšķiniet uz **Drošības noklusējumu pārvaldība**.</span><span class="sxs-lookup"><span data-stu-id="b1832-109">At the bottom of the page, click **Manage Security defaults**.</span></span>

4. <span data-ttu-id="b1832-110">Noklikšķiniet uz **Jā**, lai iespējotu drošības noklusējumus vai uz **Nē**, lai atspējotu drošības noklusējumus.</span><span class="sxs-lookup"><span data-stu-id="b1832-110">Click **Yes** to enable security defaults or **No** to disable security defaults.</span></span>
