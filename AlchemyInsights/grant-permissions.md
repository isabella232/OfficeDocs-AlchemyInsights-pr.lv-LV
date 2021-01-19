---
title: Atļauju piešķiršana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7784"
ms.openlocfilehash: 9e686bd33414512b0a3a2bc24477832a508537a8
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901185"
---
# <a name="grant-permissions"></a><span data-ttu-id="c85f5-102">Atļauju piešķiršana</span><span class="sxs-lookup"><span data-stu-id="c85f5-102">Grant permissions</span></span>

1. <span data-ttu-id="c85f5-103">**Nomnieka mēroga administratora piekrišanas piešķiršana**: skatiet rakstu [nomnieka mēroga administratora piekrišana lietojumprogrammai](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) , lai saņemtu pakāpeniskus norādījumus par nomnieka administratora piekrišanas piešķiršanu no Azure portāla, izmantojot Azure AD PowerShell, vai arī no piekrišanas uzvednes.</span><span class="sxs-lookup"><span data-stu-id="c85f5-103">**Granting tenant-wide admin consent**: See [Grant tenant-wide admin consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/grant-admin-consent) for step-by-step instructions for granting tenant-wide admin consent from the Azure portal, using Azure AD PowerShell, or from the consent prompt itself.</span></span>
1. <span data-ttu-id="c85f5-104">**Piešķirt piekrišanu noteikta lietotāja vārdā**: tā vietā, lai piešķirtu piekrišanu visai organizācijai, administrators var izmantot arī [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) , lai piešķirtu piekrišanu pilnvarotām atļaujām viena lietotāja vārdā.</span><span class="sxs-lookup"><span data-stu-id="c85f5-104">**Granting consent on behalf of a specific user**: Instead of granting consent for the entire organization, an administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/graph/use-the-api) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="c85f5-105">Lai iegūtu papildinformāciju, skatiet rakstu [piekļuves iegūšana lietotāja vārdā](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="c85f5-105">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>