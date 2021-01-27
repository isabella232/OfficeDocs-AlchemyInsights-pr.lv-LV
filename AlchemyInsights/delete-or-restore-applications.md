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
ms.openlocfilehash: 4df9a98644f6bc7a30f9009719c5198db591afc9
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014903"
---
# <a name="delete-or-restore-applications"></a>Lietojumprogrammu dzēšana vai atjaunošana

**Lai izdzēstu lietojumprogrammu no AZURE ad nomnieka**:

1. **AZURE ad portālā** atlasiet **uzņēmuma lietojumprogrammas**. Pēc tam atrodiet un atlasiet lietojumprogrammu, kuru vēlaties izdzēst.
2. Kreisās rūts sadaļā **pārvaldība** atlasiet **Rekvizīti**.
3. Atlasiet **Dzēst** un pēc tam atlasiet **Jā** , lai apstiprinātu, ka vēlaties dzēst programmu no sava Azure AD nomnieka.

Lai iegūtu papildinformāciju par to, kā izdzēst programmu, skatiet rakstu [Quickstart: lietojumprogrammas dzēšana Azure Active Directory (AZURE AD) nomniekā](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).

Programmā PowerShell [noņemot-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet, tiek noņemtas lietojumprogrammu starpniekservera konfigurācijas no noteiktas lietojumprogrammas Azure Active Directory un var pilnībā izdzēst lietojumprogrammu, ja tas ir norādīts.

**Izdzēsto lietojumprogrammu varat atjaunot** , izmantojot PowerShell. Pēc tam, kad programma, kuru vēlaties atjaunot, ir atrasta, varat to atjaunot, izmantojot [atjaunošanu-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).
