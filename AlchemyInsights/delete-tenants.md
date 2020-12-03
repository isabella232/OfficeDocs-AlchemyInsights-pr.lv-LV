---
title: Nomnieka dzēšana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564617"
---
# <a name="delete-tenant"></a><span data-ttu-id="da7d3-102">Nomnieka dzēšana</span><span class="sxs-lookup"><span data-stu-id="da7d3-102">Delete tenant</span></span>

<span data-ttu-id="da7d3-103">Lai izdzēstu Azure AD, pārliecinieties, vai:</span><span class="sxs-lookup"><span data-stu-id="da7d3-103">To delete an Azure AD, ensure:</span></span>
- <span data-ttu-id="da7d3-104">Jūs esat globālais administrators direktorijā.</span><span class="sxs-lookup"><span data-stu-id="da7d3-104">You are a Global Administrator on the directory.</span></span>
- <span data-ttu-id="da7d3-105">Jūs neesat pierakstījies, izmantojot kontu, kuram ir noklusējuma direktorijs, piemēram, contoso.onmicrosoft.com parakstītajā kontā, piemēram, admin@contoso.onmicrosoft.com.</span><span class="sxs-lookup"><span data-stu-id="da7d3-105">You are NOT signed in with an account that has the default directory such as contoso.onmicrosoft.com in the signed--in account, such as admin@contoso.onmicrosoft.com.</span></span>
- <span data-ttu-id="da7d3-106">Noņemiet visas aktīvās lietojumprogrammas direktorijā pirms dzēšanas.</span><span class="sxs-lookup"><span data-stu-id="da7d3-106">Remove any active applications in the directory before deletion.</span></span> <span data-ttu-id="da7d3-107">Lai noņemtu aktīvās lietojumprogrammas, atveriet lietojumprogrammu reģistrācijas un noņemiet esošās lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="da7d3-107">To remove active applications, navigate to App registrations and remove the existing applications.</span></span>
- <span data-ttu-id="da7d3-108">Nevienam Microsoft tiešsaistes pakalpojumam, piemēram, Microsoft Azure, Office 365 vai Azure AD Premium, kas ir saistīts ar direktoriju, nav neviena aktīva abonementa.</span><span class="sxs-lookup"><span data-stu-id="da7d3-108">There are no active subscriptions for any Microsoft Online Services, such as Microsoft Azure, Office 365 or Azure AD Premium associated on the directory.</span></span> <span data-ttu-id="da7d3-109">Pārsūtiet savus abonementus vai Paātriniet aktīvo abonementu atcelšanu, izmantojot Azure atbalstu un norēķinus.</span><span class="sxs-lookup"><span data-stu-id="da7d3-109">Transfer your subscriptions or expedite cancellation of active subscriptions via Azure Support and Billing.</span></span> <span data-ttu-id="da7d3-110">Uzziniet vairāk par to, kā atcelt Office 365 un Azure abonementus.</span><span class="sxs-lookup"><span data-stu-id="da7d3-110">Learn more on How to Cancel Office 365 and Azure subscriptions.</span></span> <span data-ttu-id="da7d3-111">Norādījumus par to, kā nomniekam piesaistīt vai pievienot esošu abonementu, skatiet sadaļā [AZURE ad nomnieka saistīšana vai pievienošana](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span><span class="sxs-lookup"><span data-stu-id="da7d3-111">For guidance on associating or adding an existing subscription to a tenant, see [Associate or add an Azure subscription to your Azure AD tenant](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).</span></span>
- <span data-ttu-id="da7d3-112">Nav nevienas aktīvas licences.</span><span class="sxs-lookup"><span data-stu-id="da7d3-112">There are no Active license.</span></span> <span data-ttu-id="da7d3-113">Lai noņemtu licences, skatiet rakstu [kā noņemt abonementu, lai noņemtu licenci](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span><span class="sxs-lookup"><span data-stu-id="da7d3-113">To remove licenses, see [How to remove Subscription to Remove license](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).</span></span>
- <span data-ttu-id="da7d3-114">Nav citu aktīvu lietotāju direktorijā bez sevis kā globālais administrators, mēģinot izdzēst Azure AD.</span><span class="sxs-lookup"><span data-stu-id="da7d3-114">There are no other active users in the directory besides yourself as the Global Administrator when attempting to delete the Azure AD.</span></span> <span data-ttu-id="da7d3-115">Noņemiet visus pārējos aktīvos lietotājus, bet, ja vēlaties, ir jānoņem, piemēram, ar admin@contoso.com izveidotie lietotāji.</span><span class="sxs-lookup"><span data-stu-id="da7d3-115">Remove any other active users, and any dependencies on a custom domain name in the tenant will also need to be removed, such as users created with admin@contoso.com.</span></span>

<span data-ttu-id="da7d3-116">Detalizētāku informāciju par to, kā:</span><span class="sxs-lookup"><span data-stu-id="da7d3-116">For more detail steps on how to:</span></span>
- <span data-ttu-id="da7d3-117">Dzēst "Azure Active Directory" vai "abonementu", skatiet rakstu [Azure Active Directory dzēšana](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span><span class="sxs-lookup"><span data-stu-id="da7d3-117">Delete "Azure Active Directory" or "subscription",  see [Delete Azure Active Directory](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).</span></span>
- <span data-ttu-id="da7d3-118">Noņemot lietojumprogrammas direktorijā, skatiet rakstu [lietojumprogrammu noņemšana](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span><span class="sxs-lookup"><span data-stu-id="da7d3-118">Removing applications in the directory, see [Removing Applications](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app).</span></span> 
