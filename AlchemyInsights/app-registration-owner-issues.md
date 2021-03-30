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
# <a name="app-registration-owner-issues"></a>Lietojumprogrammu reģistrācijas īpašnieka problēmas

Tālāk ir aprakstītas pieejamās metodes pamatdarbību pievienošanai programmu reģistrāciju īpašniekiem.

- Azure AD PowerShell moduļa izmantošana -

    `Connect-AzureAd`

    `Add-AzureADApplicationOwner -ObjectId <Application ObjectId>-RefObjectId <ObjectID of principal to assign as owner>`

    Atsauce: [Add-AzureADApplicationOwner (AzureAD)](https://docs.microsoft.com/powershell/module/azuread/add-azureadapplicationowner)
- Azure CLI lietošana - `az ad app owner add`

    Atsauce: [az ad lietojumprogrammas īpašnieks](https://docs.microsoft.com/cli/azure/ad/app/owner)
- MS Graph lietošana -

    Atsauce: [Īpašnieka pievienošana — Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Izmantojot Azure AD portālu — naviģējiet uz [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > lietojumprogrammu reģistrācijas > Atlasiet savu lietojumprogrammu > īpašniekiem > pievienot īpašniekus

**Nevar skatīt programmu programmu reģistrācijas asmensmenī, pat ja esat šīs programmas īpašnieks?**

Lietojumprogrammas īpašnieks nav administratīvas loma. Ja ir [iespējots iestatījums Ierobežot](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) piekļuvi Azure AD administrēšanas portālam, tikai administrators var skatīt lietojumprogrammas programmu reģistrācijas portālā. Lai īpašnieks varētu skatīt lietojumprogrammas, atspējojiet šo iestatījumu (Iestatīt kā NĒ) vai piešķiriet administratora lomu īpašniekam tikai konkrētai lietojumprogrammai. Tomēr ir nepieciešama Azure AD Premium P2 licence un iespējota [priviliģēta identitātes pārvaldība.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
