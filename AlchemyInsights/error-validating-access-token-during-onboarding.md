---
title: Radās kļūda, pārbaudot piekļuves pilnvara kļūdas laikā darbvirsmas Analytics iekāpšanas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 7472af5c4e19e5697b5fb4802ed1cbb2c74f1d19
ms.sourcegitcommit: f1fad2129d09660ec42dbce03ce2c6b4cfc9555a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/18/2019
ms.locfileid: "40741220"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a><span data-ttu-id="65f46-102">"Radās kļūda, pārbaudot piekļuves pilnvara" kļūda darbvirsmas Analytics pārvietošana</span><span class="sxs-lookup"><span data-stu-id="65f46-102">"There was an error validating access token" error during Desktop Analytics onboarding</span></span>

<span data-ttu-id="65f46-103">Šī kļūda parasti tiek novērota, kad beidzas autentifikācijas pilnvara.</span><span class="sxs-lookup"><span data-stu-id="65f46-103">This error is normally observed when the authentication token expires.</span></span> <span data-ttu-id="65f46-104">Parasti lappuses atsvaidzināšana atsvaidzina marķieri.</span><span class="sxs-lookup"><span data-stu-id="65f46-104">Usually, refreshing the page refreshes the token.</span></span> <span data-ttu-id="65f46-105">Tomēr šī problēma var saglabāties, ja ir visas ierobežotas piekļuves politikas lieto uz borta Desktop Analytics izmanto kontu.</span><span class="sxs-lookup"><span data-stu-id="65f46-105">However, this issue can persist if there are any Conditional Access policies applied to the account being used to on-board Desktop Analytics.</span></span> <span data-ttu-id="65f46-106">Varat pārskatīt Azure AD pierakstīšanās žurnālos Azure portālā, lai redzētu, vai ir jebkādas pierakstīšanās kļūmes konts tiek izmantots darbvirsmas Analytics pārvietošana.</span><span class="sxs-lookup"><span data-stu-id="65f46-106">You can review the Azure AD Sign In logs in the Azure Portal to see if there are any sign-in failures for the account being used for Desktop Analytics onboarding.</span></span>

<span data-ttu-id="65f46-107">Lai iegūtu papildinformāciju par ierobežotu piekļuvi, apmeklējiet lapu [ierobežotas piekļuves izvietošanas plānošana](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span><span class="sxs-lookup"><span data-stu-id="65f46-107">For more information about Conditional Access, visit [Plan your Conditional Access deployment](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access).</span></span>