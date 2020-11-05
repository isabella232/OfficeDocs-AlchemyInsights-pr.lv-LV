---
title: Azure norēķinu īpašumtiesību nodošana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003560"
- "6849"
ms.openlocfilehash: e9a1e74b321e2c2dda5f7a4f69681a0acf0635d5
ms.sourcegitcommit: a5ba4dc8c349ed79147f67b62bde544281f7c106
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/03/2020
ms.locfileid: "48922079"
---
# <a name="transfer-azure-billing-ownership"></a><span data-ttu-id="24c99-102">Azure norēķinu īpašumtiesību nodošana</span><span class="sxs-lookup"><span data-stu-id="24c99-102">Transfer Azure billing ownership</span></span>

<span data-ttu-id="24c99-103">Pierakstieties [Azure portālā](https://portal.azure.com/) kā norēķinu konta administrators ar abonementu, kuru vēlaties pārsūtīt.</span><span class="sxs-lookup"><span data-stu-id="24c99-103">Sign in to the [Azure portal](https://portal.azure.com/) as an administrator of the billing account that has the subscription that you want to transfer.</span></span> <span data-ttu-id="24c99-104">Ja neesat pārliecināts, vai esat administrators, vai jums ir nepieciešams noteikt, kas ir, skatiet rakstu [konta norēķinu administratora noteikšana](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span><span class="sxs-lookup"><span data-stu-id="24c99-104">If you're not sure if you're and administrator, or if you need to determine who is, see [Determine account billing administrator](https://docs.microsoft.com/azure/cost-management-billing/understand/subscription-transfer#whoisaa).</span></span>

- <span data-ttu-id="24c99-105">Meklējiet par **Cost Management + norēķiniem**.</span><span class="sxs-lookup"><span data-stu-id="24c99-105">Search on **Cost Management + Billing**.</span></span>
- <span data-ttu-id="24c99-106">Atlasiet **abonementi** no kreisās rūts.</span><span class="sxs-lookup"><span data-stu-id="24c99-106">Select **Subscriptions** from left pane.</span></span> <span data-ttu-id="24c99-107">Atkarībā no programmas Access, iespējams, būs jāatlasa norēķinu tvērums un pēc tam **abonementi** vai **Azure abonementi**.</span><span class="sxs-lookup"><span data-stu-id="24c99-107">Depending on the access, you may need to select a billing scope and then **Subscriptions** or **Azure subscriptions**.</span></span>
- <span data-ttu-id="24c99-108">Atlasiet **pārsūtīt norēķinu īpašumtiesības** abonementam, kuru vēlaties pārsūtīt</span><span class="sxs-lookup"><span data-stu-id="24c99-108">Select **Transfer billing ownership** for the subscription you want to transfer</span></span>
- <span data-ttu-id="24c99-109">Ievadiet tā lietotāja e-pasta adresi, kurš ir tā konta norēķinu administrators, kas būs jaunais abonementa īpašnieks, un pēc tam atlasiet **Sūtīt pārsūtīšanas pieprasījumu**</span><span class="sxs-lookup"><span data-stu-id="24c99-109">Enter the email address of a user who's a billing administrator of the account that will be the new owner for the subscription and then select **send transfer request**</span></span>
- <span data-ttu-id="24c99-110">Lietotājs saņem e-pasta ziņojumu ar norādījumiem par pārsūtīšanas pieprasījuma pārskatīšanu.</span><span class="sxs-lookup"><span data-stu-id="24c99-110">The user gets an email with instructions to review your transfer request.</span></span> <span data-ttu-id="24c99-111">Lai apstiprinātu pārsūtīšanas pieprasījumu, lietotājs atlasa saiti e-pasta ziņojumā un seko instrukcijām.</span><span class="sxs-lookup"><span data-stu-id="24c99-111">To approve the transfer request, the user selects the link in the email and follows the instructions.</span></span>

<span data-ttu-id="24c99-112">**Ņemiet vērā** : Ja pārsūtāt norēķinu īpašumtiesības uz lietotāja kontu citā Azure AD nomniekā, visi [lomu piekļuves vadības (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)uzdevumi, lai pārvaldītu abonementa resursus, tiek neatgriezeniski noņemti.</span><span class="sxs-lookup"><span data-stu-id="24c99-112">**Note** : If you transfer billing ownership of your subscription to a user's account in another Azure AD tenant, all [role-based access control (RBAC)](https://docs.microsoft.com/azure/role-based-access-control/overview?WT.mc_id=Portal-Microsoft_Azure_Support)assignments to manage resources in the subscription are permanently removed.</span></span> <span data-ttu-id="24c99-113">Tikai jaunajam īpašniekam būs piekļuve pārvaldīt resursus abonementā.</span><span class="sxs-lookup"><span data-stu-id="24c99-113">Only the new owner will have access to manage resources in the subscription.</span></span> <span data-ttu-id="24c99-114">Lai iegūtu papildinformāciju, skatiet rakstu [abonementa pārsūtīšana lietotājam citā AZURE ad nomniekā](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="24c99-114">For more information, see [Transferring subscription to a user in another Azure AD tenant](https://docs.microsoft.com/azure/active-directory/managed-identities-azure-resources/known-issues?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="24c99-115">**Ieteicamie dokumenti**</span><span class="sxs-lookup"><span data-stu-id="24c99-115">**Recommended Documents**</span></span>

- [<span data-ttu-id="24c99-116">Norēķinu īpašumtiesību uz Azure abonementu pārsūtīšana uz citu kontu</span><span class="sxs-lookup"><span data-stu-id="24c99-116">Transfer billing ownership of an Azure subscription to another account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/billing-subscription-transfer)
- [<span data-ttu-id="24c99-117">Par norēķinu īpašumtiesību nodošanu Azure abonementam</span><span class="sxs-lookup"><span data-stu-id="24c99-117">About transferring billing ownership for an Azure subscription</span></span>](https://docs.microsoft.com//azure/cost-management-billing/understand/subscription-transfer)
- [<span data-ttu-id="24c99-118">Visual Studio, Microsoft partneru tīkla (MPN) un pay as Go Dev/Test abonementu pārsūtīšana</span><span class="sxs-lookup"><span data-stu-id="24c99-118">Transferring Visual Studio, Microsoft Partner Network (MPN) and Pay as you go Dev/Test subscriptions</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#transferring-visual-studio-microsoft-partner-network-mpn-and-pay-as-you-go-devtest-subscriptions)
- [<span data-ttu-id="24c99-119">Bieži uzdotie jautājumi par īpašumtiesību nodošanu</span><span class="sxs-lookup"><span data-stu-id="24c99-119">Transfer Ownership FAQ</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#frequently-asked-questions-faq-for-senders)
- [<span data-ttu-id="24c99-120">Īpašumtiesību nodošanas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="24c99-120">Troubleshoot Transfer ownership issues</span></span>](https://docs.microsoft.com/azure/billing/billing-subscription-transfer?WT.mc_id=Portal-Microsoft_Azure_Support#troubleshooting)
