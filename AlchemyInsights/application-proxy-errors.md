---
title: Ar lietojumprogrammu starpniekserveri saistīto kļūdu novēršana
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004356"
- "9686"
ms.openlocfilehash: fe0bae35942af9925e8a5f90f966e204d7f84fd2
ms.sourcegitcommit: a6ab402f59e5ee1492bcf5ab7f18714fc251717d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/22/2021
ms.locfileid: "51036749"
---
# <a name="troubleshoot-errors-related-to-application-proxy"></a><span data-ttu-id="260d9-102">Ar lietojumprogrammu starpniekserveri saistīto kļūdu novēršana</span><span class="sxs-lookup"><span data-stu-id="260d9-102">Troubleshoot errors related to Application Proxy</span></span>

- <span data-ttu-id="260d9-103">Lai uzzinātu biežāk sastopamās kļūdas, kas rodas, izmantojot Kerberos iestatīšanu un konfigurēšanu, un ieteikumus par risinājumu skatiet rakstā [lietojumprogrammu starpniekservera problēmu novēršana un kļūdu ziņojumi](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-troubleshoot#kerberos-errors).</span><span class="sxs-lookup"><span data-stu-id="260d9-103">To learn about the more common errors that come from Kerberos setup and configuration, and suggestions for resolution, see [Troubleshoot Application Proxy problems and error messages](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-troubleshoot#kerberos-errors).</span></span>
- <span data-ttu-id="260d9-104">Lietojumprogrammas starpniekservera 404 kļūdas skatiet rakstā [lietojumprogrammu lapa netiek rādīta pareizi lietojumprogrammu starpniekserverim | Microsoft dokumenti](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-page-appearance-broken-problem).</span><span class="sxs-lookup"><span data-stu-id="260d9-104">For App Proxy 404 errors, see [App page doesn't display correctly for Application Proxy app | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-page-appearance-broken-problem).</span></span>
- <span data-ttu-id="260d9-105">Azure Active Directory (Azure AD), konfigurējot lielu skaitu lokālās lietojumprogrammas, var ātri kļūt nepārvaldāms un rada nevajadzīgus riskus konfigurācijas kļūdām, ja daudziem no tiem ir nepieciešami vieni un tie paši iestatījumi.</span><span class="sxs-lookup"><span data-stu-id="260d9-105">In Azure Active Directory (Azure AD), configuring a large number of on-premises applications can quickly become unmanageable and introduces unnecessary risks for configuration errors if many of them require the same settings.</span></span> <span data-ttu-id="260d9-106">Izmantojot [AZURE ad lietojumprogrammas starpniekserveri](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy), varat novērst šo problēmu, izmantojot aizstājējzīmju lietojumprogrammu publicēšanu, lai vienlaikus publicētu un pārvaldītu vairākas lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="260d9-106">With [Azure AD Application Proxy](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy), you can address this issue by using wildcard application publishing to publish and manage many applications at once.</span></span> <span data-ttu-id="260d9-107">Papildinformāciju skatiet rakstā [aizstājējzīmju lietojumprogrammas AZURE ad lietojumprogrammas starpniekserverī | Microsoft dokumenti](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard).</span><span class="sxs-lookup"><span data-stu-id="260d9-107">For more information, see [Wildcard applications in the Azure AD Application Proxy | Microsoft Docs](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-wildcard).</span></span>
