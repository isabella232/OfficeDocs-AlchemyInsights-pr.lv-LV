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
# <a name="delete-or-restore-applications"></a><span data-ttu-id="88e86-102">Lietojumprogrammu dzēšana vai atjaunošana</span><span class="sxs-lookup"><span data-stu-id="88e86-102">Delete or restore applications</span></span>

<span data-ttu-id="88e86-103">**Lai izdzēstu lietojumprogrammu no AZURE ad nomnieka**:</span><span class="sxs-lookup"><span data-stu-id="88e86-103">**To delete an application from your Azure AD tenant**:</span></span>

1. <span data-ttu-id="88e86-104">**AZURE ad portālā** atlasiet **uzņēmuma lietojumprogrammas**.</span><span class="sxs-lookup"><span data-stu-id="88e86-104">In the **Azure AD portal**, select **Enterprise applications**.</span></span> <span data-ttu-id="88e86-105">Pēc tam atrodiet un atlasiet lietojumprogrammu, kuru vēlaties izdzēst.</span><span class="sxs-lookup"><span data-stu-id="88e86-105">Then find and select the application you want to delete.</span></span>
2. <span data-ttu-id="88e86-106">Kreisās rūts sadaļā **pārvaldība** atlasiet **Rekvizīti**.</span><span class="sxs-lookup"><span data-stu-id="88e86-106">In the **Manage** section in the left pane, select **Properties**.</span></span>
3. <span data-ttu-id="88e86-107">Atlasiet **Dzēst** un pēc tam atlasiet **Jā** , lai apstiprinātu, ka vēlaties dzēst programmu no sava Azure AD nomnieka.</span><span class="sxs-lookup"><span data-stu-id="88e86-107">Select **Delete**, and then select **Yes** to confirm you want to delete the app from your Azure AD tenant.</span></span>

<span data-ttu-id="88e86-108">Lai iegūtu papildinformāciju par to, kā izdzēst programmu, skatiet rakstu [Quickstart: lietojumprogrammas dzēšana Azure Active Directory (AZURE AD) nomniekā](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span><span class="sxs-lookup"><span data-stu-id="88e86-108">For more information on how to delete an app, see [Quickstart: Delete an application from your Azure Active Directory (Azure AD) tenant](https://docs.microsoft.com/azure/active-directory/manage-apps/delete-application-portal#delete-an-application-from-your-azure-ad-tenant).</span></span>

<span data-ttu-id="88e86-109">Programmā PowerShell [noņemot-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet, tiek noņemtas lietojumprogrammu starpniekservera konfigurācijas no noteiktas lietojumprogrammas Azure Active Directory un var pilnībā izdzēst lietojumprogrammu, ja tas ir norādīts.</span><span class="sxs-lookup"><span data-stu-id="88e86-109">In PowerShell, the [Remove-AzureADApplicationProxyApplication](https://docs.microsoft.com/powershell/module/azuread/remove-azureadapplicationproxyapplication) cmdlet removes Application Proxy configurations from a specific application in Azure Active Directory, and can delete the application completely if specified.</span></span>

<span data-ttu-id="88e86-110">**Izdzēsto lietojumprogrammu varat atjaunot** , izmantojot PowerShell.</span><span class="sxs-lookup"><span data-stu-id="88e86-110">You can **restore a deleted application** using PowerShell.</span></span> <span data-ttu-id="88e86-111">Pēc tam, kad programma, kuru vēlaties atjaunot, ir atrasta, varat to atjaunot, izmantojot [atjaunošanu-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span><span class="sxs-lookup"><span data-stu-id="88e86-111">Once the application you want to restore has been identified, you can restore it using [Restore-AzureADDeletedApplication](https://docs.microsoft.com/powershell/module/azuread/restore-azureaddeletedapplication).</span></span>
