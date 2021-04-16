---
title: Radās kļūda, validējot piekļuves pilnvaru kļūdu desktop Analytics lietošanas laikā
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813695"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="1f435-102">Darbvirsmas analīzes instalēšanas laikā radās kļūda "Validējot piekļuves pilnvaru".</span><span class="sxs-lookup"><span data-stu-id="1f435-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="1f435-103">Šī kļūda parasti tiek novērota, kad beidzas autentifikācijas pilnvaras derīgums.</span><span class="sxs-lookup"><span data-stu-id="1f435-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="1f435-104">Parasti lapas atsvaidzināšana atsvaidzina pilnvaru.</span><span class="sxs-lookup"><span data-stu-id="1f435-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="1f435-105">Tomēr šī problēma var saglabāties, ja pastāv nosacījum piekļuves politikas, kas tiek lietotas kontam, kas tiek izmantots darbvirsmas analītikai.</span><span class="sxs-lookup"><span data-stu-id="1f435-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="1f435-106">Varat pārskatīt Azure AD pierakstīšanās žurnālus Azure portālā, lai uzzinātu, vai nav pieteikšanās kļūmju kontā, kas tiek izmantots Desktop Analytics pievienošanai.</span><span class="sxs-lookup"><span data-stu-id="1f435-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="1f435-107">Lai iegūtu papildinformāciju par nosacījum piekļuvi, apmeklējiet [vietni Nosacījum piekļuves izvietošanas plānošana.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)</span><span class="sxs-lookup"><span data-stu-id="1f435-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>