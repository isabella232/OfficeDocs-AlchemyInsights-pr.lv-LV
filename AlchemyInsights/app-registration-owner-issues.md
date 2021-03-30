---
title: Lietojumprogrammu reģistrācijas īpašnieka problēmas
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
- "9004352"
- "9655"
ms.openlocfilehash: 9dc3b1d54bb263d5e53e02a4e4dadc8cf3c1e400
ms.sourcegitcommit: 1f43598a726cdb9904aa501eb8db87f143020d9e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/23/2021
ms.locfileid: "51404777"
---
# <a name="app-registration-owner-issues"></a><span data-ttu-id="b81f2-102">Lietojumprogrammu reģistrācijas īpašnieka problēmas</span><span class="sxs-lookup"><span data-stu-id="b81f2-102">App Registration Owner issues</span></span>

<span data-ttu-id="b81f2-103">Tālāk ir aprakstītas pieejamās metodes pamatdarbību pievienošanai programmu reģistrāciju īpašniekiem.</span><span class="sxs-lookup"><span data-stu-id="b81f2-103">Following are the available methods to add principals as owners for app registrations:</span></span>

- <span data-ttu-id="b81f2-104">Azure AD PowerShell moduļa izmantošana -</span><span class="sxs-lookup"><span data-stu-id="b81f2-104">Using Azure AD PowerShell Module -</span></span>

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    <span data-ttu-id="b81f2-105">Atsauce: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span><span class="sxs-lookup"><span data-stu-id="b81f2-105">Reference: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)</span></span>
- <span data-ttu-id="b81f2-106">Azure CLI lietošana - `az ad app owner add`</span><span class="sxs-lookup"><span data-stu-id="b81f2-106">Using Azure CLI - `az ad app owner add`</span></span>

    <span data-ttu-id="b81f2-107">Atsauce: [az ad lietojumprogrammas īpašnieks](https://docs.microsoft.com/cli/azure/ad/app/owner)</span><span class="sxs-lookup"><span data-stu-id="b81f2-107">Reference: [az ad app owner](https://docs.microsoft.com/cli/azure/ad/app/owner)</span></span>
- <span data-ttu-id="b81f2-108">MS Graph lietošana -</span><span class="sxs-lookup"><span data-stu-id="b81f2-108">Using MS Graph -</span></span>

    <span data-ttu-id="b81f2-109">Atsauce: [Īpašnieka pievienošana — Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span><span class="sxs-lookup"><span data-stu-id="b81f2-109">Reference: [Add owner - Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)</span></span>
- <span data-ttu-id="b81f2-110">Izmantojot Azure AD portālu — naviģējiet uz [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > lietojumprogrammu reģistrācijas > Atlasiet savu lietojumprogrammu > īpašniekiem > pievienot īpašniekus</span><span class="sxs-lookup"><span data-stu-id="b81f2-110">Using the Azure AD Portal - Navigate to [portal.azure.com](https://portal.azure.com/) > Azure Active directory > App Registration > Select your application > Owners > Add Owners</span></span>

<span data-ttu-id="b81f2-111">**Nevar skatīt programmu programmu reģistrācijas asmensmenī, pat ja esat šīs programmas īpašnieks?**</span><span class="sxs-lookup"><span data-stu-id="b81f2-111">**Cannot view your application on App Registrations blade even though you are the owner of that application?**</span></span>

<span data-ttu-id="b81f2-112">Lietojumprogrammas īpašnieks nav administratīvas loma.</span><span class="sxs-lookup"><span data-stu-id="b81f2-112">Owner of an app is not an administrative role.</span></span> <span data-ttu-id="b81f2-113">Ja ir [iespējots iestatījums Ierobežot](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) piekļuvi Azure AD administrēšanas portālam, tikai administrators var skatīt lietojumprogrammas programmu reģistrācijas portālā.</span><span class="sxs-lookup"><span data-stu-id="b81f2-113">If the setting [Restrict access to Azure AD administration portal](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) is enabled, then only admin will be able to view the applications on App Registration portal.</span></span> <span data-ttu-id="b81f2-114">Lai īpašnieks varētu skatīt lietojumprogrammas, atspējojiet šo iestatījumu (Iestatīt kā NĒ) vai piešķiriet administratora lomu īpašniekam tikai konkrētai lietojumprogrammai.</span><span class="sxs-lookup"><span data-stu-id="b81f2-114">For an owner to be able to view the applications, either disable this setting (Set this to NO) or assign admin role to the owner for only the specific application.</span></span> <span data-ttu-id="b81f2-115">Tomēr ir nepieciešama Azure AD Premium P2 licence un iespējota [priviliģēta identitātes pārvaldība.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)</span><span class="sxs-lookup"><span data-stu-id="b81f2-115">However for this, you will require an Azure AD Premium P2 license and enable [Privileged Identity Management](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure).</span></span>
