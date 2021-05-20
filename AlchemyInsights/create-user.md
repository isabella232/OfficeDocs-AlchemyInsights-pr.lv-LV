---
title: Lietotāja izveide
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/11/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003231"
- "9403"
ms.openlocfilehash: 800baae2d748708d8cb7a5fb0e73fce5dcf455cb
ms.sourcegitcommit: 2d617ae59eed0ce8b571339ceefce6473c03b94c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/19/2021
ms.locfileid: "52569738"
---
# <a name="create-user"></a><span data-ttu-id="9561f-102">Lietotāja izveide</span><span class="sxs-lookup"><span data-stu-id="9561f-102">Create user</span></span>

<span data-ttu-id="9561f-103">**PAZIŅOJUMS:**</span><span class="sxs-lookup"><span data-stu-id="9561f-103">**ANNOUNCEMENT:**</span></span>

- <span data-ttu-id="9561f-104">Google tīmekļa skata pierakstīšanās atbalsta noilgums, sākot no [2021. gada 4. janvāra.](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support)</span><span class="sxs-lookup"><span data-stu-id="9561f-104">[Deprecation of WebView sign-in support from Google starting January 4, 2021](/azure/active-directory/external-identities/google-federation#deprecation-of-webview-sign-in-support) .</span></span> <span data-ttu-id="9561f-105">Pārbaudiet, vai jūsu programmas var ietekmēt [Google norādījumi par](https://go.microsoft.com/fwlink/?linkid=2157323) testēšanu saderību.</span><span class="sxs-lookup"><span data-stu-id="9561f-105">Test whether your apps may be affected by following [Google’s guidance](https://go.microsoft.com/fwlink/?linkid=2157323) on testing compatibility.</span></span>
- <span data-ttu-id="9561f-106">Pārliecinieties, vai izmantojat sistēmas tīmekļa skatu vai sistēmas pārlūkprogrammu, pierakstoties lietotāju Google patērētāju kontos.</span><span class="sxs-lookup"><span data-stu-id="9561f-106">Make sure you use the system webview or system browser when signing in your users with consumer Google accounts.</span></span> <span data-ttu-id="9561f-107">Papildinformāciju skatiet rakstā [Problēmas ar pierakstīšanos lietojumprogrammās, kas izmanto tikai pārlūkprogrammu Chrome.](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications)</span><span class="sxs-lookup"><span data-stu-id="9561f-107">For more information, see [Issues signing in to application(s) using Chrome browser only](/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications).</span></span>

<span data-ttu-id="9561f-108">**Es nevaru izveidot jaunu lietotāju savā Azure AD direktorijā**</span><span class="sxs-lookup"><span data-stu-id="9561f-108">**I can't create a new user in my Azure AD directory**</span></span>

1. <span data-ttu-id="9561f-109">Pārliecinieties, vai esat pilnvarots izveidot jaunu standarta lietotāju.</span><span class="sxs-lookup"><span data-stu-id="9561f-109">Ensure that you are authorized to create a new standard user.</span></span> <span data-ttu-id="9561f-110">Jaunu standarta lietotāju var izveidot tikai globālā administratora vai Azure Active Directory administratora loma programmā Azure Active Directory (AD).</span><span class="sxs-lookup"><span data-stu-id="9561f-110">Only the Global administrator or User administrator role in Azure Active Directory (AD) can create a new standard user.</span></span> <span data-ttu-id="9561f-111">Ja jums nav šīs lomas, lūdziet administratoram jūs pievienot kādai no šīm lomām vai izveidot jaunu lietotāja kontu jūsu vietā.</span><span class="sxs-lookup"><span data-stu-id="9561f-111">If you're not in one of these roles, ask an administrator to add you to one of these roles or to create the new user account for you.</span></span>
1. <span data-ttu-id="9561f-112">Pārliecinieties, vai lietotājvārds ir domēnā, kas ir verificēts jūsu Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9561f-112">Ensure that the user name is in a domain that is verified in your Azure AD.</span></span> <span data-ttu-id="9561f-113">Ja jūsu Azure AD nav neviena verificēta pielāgoto domēnu nosaukumu, varat izmantot savu Azure AD sākotnējo domēnu, kas beidzas ar \*.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="9561f-113">If you do not have any verified custom domain names in your Azure AD, you can use your Azure AD initial domain, which ends with \*.onmicrosoft.com.</span></span>
1. <span data-ttu-id="9561f-114">Pārliecinieties, vai lietotājvārds ir domēnā, kas nav federēts uz Azure AD no jūsu lokālā AD.</span><span class="sxs-lookup"><span data-stu-id="9561f-114">Ensure that the user name is in a domain that is not federated to Azure AD from your on-premises AD.</span></span> <span data-ttu-id="9561f-115">Lietotājus nevar pievienot mākonī ar domēnu nosaukumiem, kas ir federatīvi no lokāla domēna.</span><span class="sxs-lookup"><span data-stu-id="9561f-115">Users cannot be added in the cloud with domain names that are federated from on-premises.</span></span>
1. <span data-ttu-id="9561f-116">Pārliecinieties, vai nevienam citam lietotājam vai kontaktpersonai nav lietotājvārda, ko vēlaties piešķirt jaunajam lietotājam.</span><span class="sxs-lookup"><span data-stu-id="9561f-116">Ensure that no other user or contact already has the user name that you want to assign to the new user.</span></span> <span data-ttu-id="9561f-117">Lietotājvārdiem ir jābūt unikāliem visā Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9561f-117">User names must be unique across Azure AD.</span></span>
1. <span data-ttu-id="9561f-118">Skatiet [Azure AD lomas un administratorus](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) savam Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9561f-118">See [Azure AD roles and administrators](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="9561f-119">Skatiet [sava](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) Azure AD domēnu nosaukumus.</span><span class="sxs-lookup"><span data-stu-id="9561f-119">See the [domain names](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) for your Azure AD.</span></span>
1. <span data-ttu-id="9561f-120">Pārskatiet [audita žurnālus,](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) lai skatītu detalizētu informāciju par nesen izveidotu vai izdzēstu lietotāju kā personu, kas veica šo darbību un kad.</span><span class="sxs-lookup"><span data-stu-id="9561f-120">Review [Audit logs](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/RolesAndAdministrators) to see more detailed information about a recently created or deleted user like who performed the action and when.</span></span>
1. <span data-ttu-id="9561f-121">Papildinformāciju par jaunu lietotāju [pievienošanu skatiet rakstā Azure portāla izmantošana, lai izveidotu jaunu lietotāju savā Azure AD.](/azure/active-directory/active-directory-users-create-azure-portal)</span><span class="sxs-lookup"><span data-stu-id="9561f-121">For more information on adding new users, see [Use the Azure portal to create a new user in your Azure AD](/azure/active-directory/active-directory-users-create-azure-portal).</span></span>
1. <span data-ttu-id="9561f-122">[Azure AD administratīvās lomas:](/azure/active-directory/active-directory-assign-admin-roles)Administratora lomu atļaujas Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="9561f-122">[Azure AD administrative roles](/azure/active-directory/active-directory-assign-admin-roles): Administrator role permissions in Azure Active Directory</span></span>
1. <span data-ttu-id="9561f-123">Varat arī izmantot [Azure AD PowerShell, lai izveidotu jaunu lietotāju.](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0)</span><span class="sxs-lookup"><span data-stu-id="9561f-123">You can also [use Azure AD PowerShell to create a new user](/powershell/module/azuread/new-azureaduser?view=azureadps-2.0).</span></span>
