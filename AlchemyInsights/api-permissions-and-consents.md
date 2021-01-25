---
title: API atļaujas un piekrišana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004343"
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974608"
---
# <a name="api-permissions-and-consent"></a><span data-ttu-id="a8ab9-102">API atļaujas un piekrišana</span><span class="sxs-lookup"><span data-stu-id="a8ab9-102">API permissions and consent</span></span>

<span data-ttu-id="a8ab9-103">Lietojumprogrammas, kas ir integrētas ar Microsoft identitātes platformu, atbilst autorizācijas modelim, kas sniedz lietotājiem un administratoriem iespēju kontrolēt datu piekļuves iespējas.</span><span class="sxs-lookup"><span data-stu-id="a8ab9-103">Applications that integrate with Microsoft identity platform follow an authorization model that gives users and administrators control over how data can be accessed.</span></span> <span data-ttu-id="a8ab9-104">Autorizācijas modeļa ieviešana ir atjaunināta Microsoft identitātes platformas galapunktā.</span><span class="sxs-lookup"><span data-stu-id="a8ab9-104">The implementation of the authorization model has been updated on the Microsoft identity platform endpoint.</span></span> <span data-ttu-id="a8ab9-105">Tas maina, kā lietojumprogrammai ir jāmijiedarbojas ar Microsoft identitātes platformu.</span><span class="sxs-lookup"><span data-stu-id="a8ab9-105">It changes how an app must interact with the Microsoft identity platform.</span></span> <span data-ttu-id="a8ab9-106">[Atļaujas un piekrišana Microsoft identitātes platformas galapunktā](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) attiecas uz šī autorizācijas modeļa pamatjēdzieniem, tostarp tvērumiem, atļaujām un piekrišanu.</span><span class="sxs-lookup"><span data-stu-id="a8ab9-106">[Permissions and consent in the Microsoft identity platform endpoint](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) covers the basic concepts of this authorization model, including scopes, permissions, and consent.</span></span>

<span data-ttu-id="a8ab9-107">[Azure Active Directory (AZURE AD) piekrišanas struktūra](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) ļauj viegli izveidot vairāku nomnieku tīmekļa un vietējo klientu lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="a8ab9-107">The [Azure Active Directory (Azure AD) consent framework](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) makes it easy to develop multi-tenant web and native client applications.</span></span> <span data-ttu-id="a8ab9-108">Šīs lietojumprogrammas ļauj pierakstīties lietotāju kontos no Azure AD nomnieka, kas atšķiras no tās, kurā ir reģistrēta lietojumprogramma.</span><span class="sxs-lookup"><span data-stu-id="a8ab9-108">These applications allow sign-in by user accounts from an Azure AD tenant that's different from the one where the application is registered.</span></span> <span data-ttu-id="a8ab9-109">Tiem, iespējams, būs jāpiekļūst arī tīmekļa API, piemēram, Microsoft Graph API (lai piekļūtu Azure AD, Intune un pakalpojumiem pakalpojumā Microsoft 365) un citos Microsoft pakalpojumu API papildus savam tīmekļa API.</span><span class="sxs-lookup"><span data-stu-id="a8ab9-109">They may also need to access web APIs such as the Microsoft Graph API (to access Azure AD, Intune, and services in Microsoft 365) and other Microsoft services' APIs, in addition to your own web APIs.</span></span>

