---
title: Lietotāja piekrišanas problēmu novēršana
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
- "7785"
ms.openlocfilehash: 7249bafe1b047c66d9351a79f1782cfcc1a936a1
ms.sourcegitcommit: 7b213fd5e8a3fdb5c602673dc194d576d372ac96
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901188"
---
# <a name="troubleshoot-user-consent"></a><span data-ttu-id="2b628-102">Lietotāja piekrišanas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="2b628-102">Troubleshoot user consent</span></span>

1. <span data-ttu-id="2b628-103">Varat konfigurēt, kā lietotāji piekrīt lietojumprogrammām, izmantojot Azure portālu vai PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2b628-103">You can configure how end-users consent to applications through the Azure Portal or PowerShell.</span></span> <span data-ttu-id="2b628-104">Papildinformāciju skatiet sadaļā [lietotāju atļauju iestatījumi](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) .</span><span class="sxs-lookup"><span data-stu-id="2b628-104">See [User consent settings](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) for more information.</span></span>
1. <span data-ttu-id="2b628-105">Administrators var izmantot arī [Microsoft GRAPH API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) , lai piešķirtu piekrišanu pilnvarotām atļaujām viena lietotāja vārdā.</span><span class="sxs-lookup"><span data-stu-id="2b628-105">An administrator can also use the [Microsoft Graph API](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) to grant consent to delegated permissions on behalf of a single user.</span></span> <span data-ttu-id="2b628-106">Lai iegūtu papildinformāciju, skatiet rakstu [piekļuves iegūšana lietotāja vārdā](https://docs.microsoft.com/graph/auth-v2-user).</span><span class="sxs-lookup"><span data-stu-id="2b628-106">For more information, see [Get access on behalf of a user](https://docs.microsoft.com/graph/auth-v2-user).</span></span>
1. <span data-ttu-id="2b628-107">[Lietotāja piekrišanas kļūdas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): šajā rakstā ir aplūkotas kļūdas, kas var rasties, ja piekrītat lietojumprogrammai.</span><span class="sxs-lookup"><span data-stu-id="2b628-107">[User Consent Errors](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error): this article discusses errors that can occur during the process of consenting to an application.</span></span> <span data-ttu-id="2b628-108">Ja esat problēmu novēršana saistībā ar negaidītu piekrišanu, kas nesatur nevienu kļūdu ziņojumu, skatiet sadaļu [AZURE ad autentifikācijas scenāriji](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="2b628-108">If you are troubleshooting unexpected consent prompts that do not contain any error messages, see [Authentication Scenarios for Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>