---
title: Lietotāja nodrošināšanas atribūtu kartēšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/22/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7851"
- "9004348"
ms.openlocfilehash: 8bbf554c533d960a304901d7cbb492b87e9bec71
ms.sourcegitcommit: 953a8567ebcd9835f8c5c49472b223107c92549b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/22/2021
ms.locfileid: "49949766"
---
# <a name="user-provisioning-attribute-mapping"></a><span data-ttu-id="29f4c-102">Lietotāja nodrošināšanas atribūtu kartēšana</span><span class="sxs-lookup"><span data-stu-id="29f4c-102">User-provisioning attribute mapping</span></span>

1. <span data-ttu-id="29f4c-103">Lai novērstu zināmās atribūtu kartēšanas problēmas, skatiet rakstu [atribūtu kartēšana](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span><span class="sxs-lookup"><span data-stu-id="29f4c-103">To troubleshoot known attribute-mapping issues, see [Attribute mappings](https://docs.microsoft.com/azure/active-directory/app-provisioning/known-issues#attribute-mappings).</span></span> 
2. <span data-ttu-id="29f4c-104">Microsoft Azure Active Directory (AD) nodrošina lietotāju nodrošināšanas atbalstu trešo pušu SaaS lietojumprogrammām, piemēram, Salesforce, G Suite un citiem.</span><span class="sxs-lookup"><span data-stu-id="29f4c-104">Microsoft Azure Active Directory (AD) provides support for user provisioning to third-party SaaS applications such as Salesforce, G Suite and others.</span></span> <span data-ttu-id="29f4c-105">Ja iespējojat lietotāja nodrošināšanu trešās puses SaaS lietojumprogrammai, Azure portāls kontrolē tās atribūtu vērtības, izmantojot atribūtu kartējumus.</span><span class="sxs-lookup"><span data-stu-id="29f4c-105">If you enable user provisioning for a third-party SaaS application, the Azure portal controls its attribute values through attribute-mappings.</span></span> <span data-ttu-id="29f4c-106">Lai uzzinātu, kā pielāgot noklusējuma atribūtu kartējumus, skatiet rakstu [lietotāja nodrošinājuma atribūta pielāgošana San lietojumprogrammām Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span><span class="sxs-lookup"><span data-stu-id="29f4c-106">To learn how to customize the default attribute-mappings, see [Customize user provisioning attribute-mappings for SaaS applications in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/app-provisioning/customize-application-attributes).</span></span>
    - <span data-ttu-id="29f4c-107">Papildinformāciju par SaaS lietojumprogrammas lietotāju nodrošināšanu skatiet rakstā [kas ir automatizētās Saas lietojumprogrammas lietotāju nodrošinājums AZURE ad?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span><span class="sxs-lookup"><span data-stu-id="29f4c-107">To learn more about SaaS app user provisioning, see [What is automated SaaS app user provisioning in Azure AD?](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning)</span></span> 
3. <span data-ttu-id="29f4c-108">Pielāgojot atribūtu kartējumus lietotāju nodrošināšanai, var gadīties, ka atribūtu, kuru vēlaties kartēt, neparādās avota atribūtu sarakstā.</span><span class="sxs-lookup"><span data-stu-id="29f4c-108">When customizing attribute-mappings for user provisioning, you might find that the attribute you want to map doesn't appear in the Source attribute list.</span></span> <span data-ttu-id="29f4c-109">[Sinhronizējot atribūtu no lokālā Active Directory uz AZURE AD,](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) lai to piešķirtu lietojumprogrammas rakstam, tiek parādīts, kā pievienot trūkstošo atribūtu, sinhronizējot to no lokālās ad uz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="29f4c-109">The [Sync an attribute from your on-premises Active Directory to Azure AD for provisioning to an application](https://docs.microsoft.com/azure/active-directory/app-provisioning/user-provisioning-sync-attributes-for-mapping) article shows you how to add the missing attribute by synchronizing it from your on-premises AD to Azure AD.</span></span>
