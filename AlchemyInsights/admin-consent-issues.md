---
title: Administratora piekrišanas problēmas
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
- "9004354"
- "7786"
ms.openlocfilehash: 6154b4b9cce51be3271cb25132f409319d8da14b
ms.sourcegitcommit: 113b802081101de70810fc73938ea92f7518d8c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901133"
---
# <a name="admin-consent-issues"></a><span data-ttu-id="e979d-102">Administratora piekrišanas problēmas</span><span class="sxs-lookup"><span data-stu-id="e979d-102">Admin consent issues</span></span>

1. <span data-ttu-id="e979d-103">Iespējojiet [administratora piekrišanas darbplūsmu](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) , lai atļautu lietotājiem pieprasīt administratora apstiprinājumu tieši no piekrišanas ekrāna.</span><span class="sxs-lookup"><span data-stu-id="e979d-103">Enable the [admin consent workflow](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-admin-consent-workflow) to allow users to request administrator approval directly from the consent screen.</span></span>

1. <span data-ttu-id="e979d-104">Ja jūs vai jūsu lietojumprogrammas lietotāji piekrišanas procesa laikā redz neparedzētas kļūdas, skatiet šo rakstu, lai uzzinātu problēmu novēršanas darbības: [neparedzēta kļūda, veicot piekrišanu lietojumprogrammai](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span><span class="sxs-lookup"><span data-stu-id="e979d-104">If you or your application's users are seeing unexpected errors during the consent process, see this article for troubleshooting steps: [Unexpected error when performing consent to an application](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).</span></span>

1. <span data-ttu-id="e979d-105">Uzziniet vairāk par [administratora piekrišanu Microsoft identitātes platformā](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), kā tiek [parādīta piekrišana](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) , kā arī kā [novērtēt pieprasījumu, kas saistīts ar nomnieka administratora piekrišanu](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span><span class="sxs-lookup"><span data-stu-id="e979d-105">Learn more about [Admin consent on the Microsoft identity platform](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent), how the [consent prompt](https://docs.microsoft.com/azure/active-directory/develop/v2-admin-consent) works, and how to [evaluate a request for tenant-wide admin consent](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent).</span></span>

1. <span data-ttu-id="e979d-106">Lietojumprogrammas, kas ir integrētas ar Microsoft identitātes platformu, atbilst autorizācijas modelim, kas sniedz lietotājiem un administratoriem iespēju kontrolēt datu piekļuves iespējas.</span><span class="sxs-lookup"><span data-stu-id="e979d-106">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="e979d-107">Autorizācijas modeļa ieviešana ir atjaunināta Microsoft identitātes platformas galapunktā, un tā maina, kā lietojumprogrammai ir jāmijiedarbojas ar Microsoft identitātes platformu.</span><span class="sxs-lookup"><span data-stu-id="e979d-107">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint, and it changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="e979d-108">Pārskatu par šo autorizācijas modeli, ieskaitot tvērumus, atļaujas un piekrišanu, skatiet [Microsoft identitātes platformas galapunktā atļaujas un piekrišana](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) .</span><span class="sxs-lookup"><span data-stu-id="e979d-108">See [Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/manage-apps/manage-consent-requests#evaluating-a-request-for-tenant-wide-admin-consent) for an overview of this authorization model, including scopes, permissions, and consent.</span></span>