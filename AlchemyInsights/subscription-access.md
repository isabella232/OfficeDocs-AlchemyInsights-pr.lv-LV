---
title: Abonementa piekļuve
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
- "9003799"
- "6805"
ms.openlocfilehash: 166380cff09f2a2bd9b7e8914d5db4071b6c3f12
ms.sourcegitcommit: bec3554bf061ef28a009f460fb9d0a661b4fc008
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/27/2020
ms.locfileid: "48807436"
---
# <a name="unable-to-sign-in-azure-due-to-browser-issues-browser-hangs-keeps-spinning-does-not-load-etc"></a><span data-ttu-id="de0f3-102">Nevar pierakstīties Azure ar pārlūkprogrammu saistītu problēmu dēļ (pārlūkprogramma uzkaras, turpina vērpšanas, netiek ielādēts utt.)</span><span class="sxs-lookup"><span data-stu-id="de0f3-102">Unable to Sign-in Azure due to browser issues (Browser hangs, keeps spinning, does not load, etc.)</span></span>

<span data-ttu-id="de0f3-103">Iespējams, jūs ietekmēs pārtraukums.</span><span class="sxs-lookup"><span data-stu-id="de0f3-103">You might be impacted by an outage.</span></span> <span data-ttu-id="de0f3-104">Lūdzu, pārbaudiet, vai pastāv nepārtraukts pārtraukums: [Azure darbspējas statuss](https://status.azure.com/status/history/).</span><span class="sxs-lookup"><span data-stu-id="de0f3-104">Please check to see if there is an ongoing outage: [Azure Health Status](https://status.azure.com/status/history/).</span></span>

<span data-ttu-id="de0f3-105">Lūdzu, atsakieties no visām aktīvajām Azure sesijām.</span><span class="sxs-lookup"><span data-stu-id="de0f3-105">Please log out of all the active Azure sessions.</span></span> <span data-ttu-id="de0f3-106">Startējiet tīmekļa pārlūkprogrammas privātu vai inkognito režīmu.</span><span class="sxs-lookup"><span data-stu-id="de0f3-106">Start a in-private or incognito mode of your web browser.</span></span>

<span data-ttu-id="de0f3-107">Varat arī mēģināt atsvaidzināt pārlūkprogrammu, izmantot citu pārlūkprogrammu, dzēst kešatmiņas sīkfailus, ja tas nedarbojas.</span><span class="sxs-lookup"><span data-stu-id="de0f3-107">You could also try to Refresh browser, use another browser, delete cache cookies if above doesn't work.</span></span>

<span data-ttu-id="de0f3-108">Papildinformācija: [pierakstīšanās problēmu novēršana](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span><span class="sxs-lookup"><span data-stu-id="de0f3-108">Learn more: [Troubleshoot Sign-in Issues](https://support.microsoft.com/help/4042961/troubleshoot-why-you-can-t-sign-in-to-manage-your-azure-subscription)</span></span>

<span data-ttu-id="de0f3-109">**Nevar piekļūt abonementiem**</span><span class="sxs-lookup"><span data-stu-id="de0f3-109">**Unable to access subscriptions**</span></span>

<span data-ttu-id="de0f3-110">[Azure portālā](https://portal.azure.com/)pārliecinieties, vai no konta augšpusē pa labi ir atlasīts pareizs Azure direktorijs.</span><span class="sxs-lookup"><span data-stu-id="de0f3-110">In the [Azure portal](https://portal.azure.com/), make sure that the correct Azure directory is selected from the account at the top right.</span></span>

<span data-ttu-id="de0f3-111">[Azure kontu centrā](https://account.windowsazure.com/Subscriptions)pārliecinieties, vai izmantotais konts ir konta administrators.</span><span class="sxs-lookup"><span data-stu-id="de0f3-111">In the [Azure Account center](https://account.windowsazure.com/Subscriptions), make sure if the account used is the account admin.</span></span>

<span data-ttu-id="de0f3-112">Papildinformācija: [problēmu novēršana nav atrasti](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span><span class="sxs-lookup"><span data-stu-id="de0f3-112">Learn more: [Troubleshoot No Subscriptions found](https://docs.microsoft.com/azure/billing/billing-no-subscriptions-found?WT.mc_id=Portal-Microsoft_Azure_Support)</span></span>

<span data-ttu-id="de0f3-113">**Nevar piekļūt norēķinu vēsturei**</span><span class="sxs-lookup"><span data-stu-id="de0f3-113">**Unable to access billing history**</span></span>

<span data-ttu-id="de0f3-114">Konta administratoram ir jāpārliecinās, ka lietotājs piekļūst norēķinu informācijai, Azure Active Directory tiek pievienots kā vieslietotājs: [pievienojiet vai dzēsiet jaunu lietotāju](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="de0f3-114">The account admin needs to make sure the user accessing the billing information is added in the Azure Active directory as a guest user: [Add or delete a new user](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="de0f3-115">Pēc tam lietotājam ir jāpiešķir globālā administratora loma: [piešķirt lomai lietotājiem](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="de0f3-115">The user then needs to be given a Global admin role: [Assign role to users](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-assign-role-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="de0f3-116">Ziņas izlikšana lietotājam var piešķirt norēķinu piekļuvi, izmantojot RBAC politikas: [piešķirt piekļuvi norēķiniem](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="de0f3-116">Post this, the user can be given billing access using RBAC policies: [Grant access to billing](https://docs.microsoft.com/azure/billing/billing-manage-access?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="de0f3-117">**Ieteicamie dokumenti**</span><span class="sxs-lookup"><span data-stu-id="de0f3-117">**Recommended Documents**</span></span>

-   [<span data-ttu-id="de0f3-118">Nevaru pierakstīties, lai pārvaldītu savu Azure abonementu</span><span class="sxs-lookup"><span data-stu-id="de0f3-118">I can't sign in to manage my Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-cannot-login-subscription?WT.mc_id=Portal-Microsoft_Azure_Support)