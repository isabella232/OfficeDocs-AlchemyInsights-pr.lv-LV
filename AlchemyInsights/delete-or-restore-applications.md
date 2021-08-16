---
title: Lietojumprogrammu dzēšana vai atjaunošana
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004335"
- "7737"
ms.openlocfilehash: 0c7be98650ca87f36b66f0bb38fb665fc81525b7f3410da14b99fb67468c1e73
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54102578"
---
# <a name="delete-or-restore-applications"></a>Lietojumprogrammu dzēšana vai atjaunošana

**Lai izdzēstu lietojumprogrammu no Azure AD nomnieka:**

1. Azure **AD portālā atlasiet** **Enterprise lietojumprogrammas**. Pēc tam atrodiet un atlasiet lietojumprogrammu, kuru vēlaties izdzēst.
2. Kreisās **puses** rūts sadaļā Pārvaldība atlasiet **Rekvizīti**.
3. Atlasiet **Dzēst** un pēc tam atlasiet **Jā,** lai apstiprinātu, ka vēlaties dzēst lietojumprogrammu no Sava Azure AD nomnieka.

Papildinformāciju par to, kā izdzēst lietojumprogrammu, skatiet rakstā Īsā pamācība: lietojumprogrammas dzēšana [no Azure Active Directory (Azure AD) nomnieka.](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant)

PowerShell cmdlet [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) noņem lietojumprogrammas starpniekservera konfigurācijas no noteiktas programmas programmā Azure Active Directory un var pilnībā izdzēst lietojumprogrammu, ja tā ir norādīta.

Izdzēstu **lietojumprogrammu varat atjaunot,** izmantojot PowerShell. Kad ir identificēta lietojumprogramma, kuru vēlaties atjaunot, varat to atjaunot, izmantojot [restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
