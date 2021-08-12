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
ms.openlocfilehash: cd7533f09ed8361e134b81979532cdebbf49971c54553a0172c7527f30e319bb
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951140"
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

    Atsauce: [Pievienot īpašnieku — Microsoft Graph v1.0](https://docs.microsoft.com/graph/api/application-post-owners)
- Izmantojot Azure AD portālu — naviģējiet uz [portal.azure.com](https://portal.azure.com/) > Azure Active Directory > lietojumprogrammu reģistrācijas > Atlasiet savu lietojumprogrammu > īpašniekiem > pievienot īpašniekus

**Nevar skatīt programmu programmu reģistrācijas asmensmenī, pat ja esat šīs programmas īpašnieks?**

Lietojumprogrammas īpašnieks nav administratīvas loma. Ja ir [iespējots iestatījums Ierobežot](https://docs.microsoft.com/azure/active-directory/fundamentals/users-default-permissions) piekļuvi Azure AD administrēšanas portālam, tikai administrators var skatīt lietojumprogrammas programmu reģistrācijas portālā. Lai īpašnieks varētu skatīt lietojumprogrammas, atspējojiet šo iestatījumu (Iestatīt kā NĒ) vai piešķiriet administratora lomu īpašniekam tikai konkrētai lietojumprogrammai. Tomēr jums būs nepieciešama Azure AD Premium P2 licence un jāiespējo [Privileged Identity Management.](https://docs.microsoft.com/azure/active-directory/privileged-identity-management/pim-configure)
