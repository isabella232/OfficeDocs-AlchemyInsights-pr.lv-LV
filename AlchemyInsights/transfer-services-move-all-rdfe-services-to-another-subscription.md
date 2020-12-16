---
title: Pakalpojumu pārsūtīšana — visu RDFE pakalpojumu pārvietošana uz citu abonementu
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
- "9004116"
- "7196"
ms.openlocfilehash: d6744484fe42f09f03de562a00fd56712607d418
ms.sourcegitcommit: ec88047d550006a1df4b6f10a3f513218113b9a5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692169"
---
# <a name="transfer-services---move-all-rdfe-services-to-another-subscription"></a><span data-ttu-id="485c4-102">Pakalpojumu pārsūtīšana — visu RDFE pakalpojumu pārvietošana uz citu abonementu</span><span class="sxs-lookup"><span data-stu-id="485c4-102">Transfer Services - Move all RDFE services to another subscription</span></span>

<span data-ttu-id="485c4-103">**Pārvietot resursus**</span><span class="sxs-lookup"><span data-stu-id="485c4-103">**Move resources**</span></span>

<span data-ttu-id="485c4-104">Azure resursus var pārvietot uz citu Azure abonementu vai resursu grupu zem tā paša abonementa, izmantojot Azure Portal, Azure PowerShell, Azure CLI vai REST API, lai pārvietotu resursus.</span><span class="sxs-lookup"><span data-stu-id="485c4-104">Azure resources can be moved to either another Azure subscription or resource group under the same subscription using Azure portal, Azure PowerShell, Azure CLI, or the REST API to move resources.</span></span>

<span data-ttu-id="485c4-105">Lai varētu pārvietot resursus, skatiet:</span><span class="sxs-lookup"><span data-stu-id="485c4-105">Before you can move resources, see:</span></span>

- [<span data-ttu-id="485c4-106">Kontrolsaraksts pirms resursu pārvietošanas</span><span class="sxs-lookup"><span data-stu-id="485c4-106">Checklist before moving resources</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#checklist-before-moving-resources)
- [<span data-ttu-id="485c4-107">Pakalpojumi, kurus var pārvietot</span><span class="sxs-lookup"><span data-stu-id="485c4-107">Services that can be moved</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-support-resources?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="485c4-108">Kā validēt pārvietošanu</span><span class="sxs-lookup"><span data-stu-id="485c4-108">How to validate the move</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#validate-move)
- [<span data-ttu-id="485c4-109">Norādījumi par pakalpojumu pārvietošanu</span><span class="sxs-lookup"><span data-stu-id="485c4-109">Move guidance for services</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/move-limitations/app-service-move-limitations?WT.mc_id=Portal-Microsoft_Azure_Support)

<span data-ttu-id="485c4-110">Lai pārvietotu esošos resursus uz citu resursu grupu vai abonementu, varat izmantot:</span><span class="sxs-lookup"><span data-stu-id="485c4-110">To move existing resources to another resource group or subscription, you can use:</span></span>

- [<span data-ttu-id="485c4-111">Azure Portal</span><span class="sxs-lookup"><span data-stu-id="485c4-111">Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-the-portal)
- [<span data-ttu-id="485c4-112">Azure PowerShell</span><span class="sxs-lookup"><span data-stu-id="485c4-112">Azure PowerShell</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-powershell)
- [<span data-ttu-id="485c4-113">Azure CLI</span><span class="sxs-lookup"><span data-stu-id="485c4-113">Azure CLI</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-azure-cli)
- [<span data-ttu-id="485c4-114">REST API</span><span class="sxs-lookup"><span data-stu-id="485c4-114">REST API</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources?WT.mc_id=Portal-Microsoft_Azure_Support#use-rest-api)

<span data-ttu-id="485c4-115">Apmācība: [Azure resursu pārvietošana uz citu resursu grupu vai abonementu](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span><span class="sxs-lookup"><span data-stu-id="485c4-115">Tutorial: [Move Azure resources to another resource group or subscription](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-tutorial-move-resources)</span></span>

<span data-ttu-id="485c4-116">**Problēmu novēršana saistībā ar Azure Resource Manager**</span><span class="sxs-lookup"><span data-stu-id="485c4-116">**Troubleshoot errors with Azure Resource Manager**</span></span>

<span data-ttu-id="485c4-117">Skatiet tālāk norādītos rakstus, lai uzzinātu par dažām tipiskām Azure izvietošanas kļūdām un saņemtu informāciju par to atrisināšanu.</span><span class="sxs-lookup"><span data-stu-id="485c4-117">Refer to the articles below to learn about some common Azure deployment errors and receive information to resolve them.</span></span> <span data-ttu-id="485c4-118">Ja nevarat atrast kļūdas kodu jūsu izvietošanas kļūdai, skatiet tēmu [kļūdas koda atrašana](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span><span class="sxs-lookup"><span data-stu-id="485c4-118">If you can't find the error code for your deployment error, see [Find error code](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors?WT.mc_id=Portal-Microsoft_Azure_Support#find-error-code).</span></span>

- [<span data-ttu-id="485c4-119">Izvietošanas kļūdu novēršana</span><span class="sxs-lookup"><span data-stu-id="485c4-119">Troubleshoot deployment errors</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-manager-common-deployment-errors)
- [<span data-ttu-id="485c4-120">Problēmu novēršana, pārvietojot Azure resursus uz jauno resursu grupu vai abonementu</span><span class="sxs-lookup"><span data-stu-id="485c4-120">Troubleshoot moving Azure resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/troubleshoot-move)

<span data-ttu-id="485c4-121">Ņemiet vērā, ka, ja vēlaties jaunināt savu Azure abonementu, piemēram, pārejat no bezmaksas uz Pay-you-go, ir jākonvertē savs abonements.</span><span class="sxs-lookup"><span data-stu-id="485c4-121">Note that if you would like to upgrade your Azure subscription, such as switching from free to pay-as-you-go, you will need to convert your subscription.</span></span>

- <span data-ttu-id="485c4-122">Lai jauninātu bezmaksas izmēģinājumversiju, skatiet rakstu [bezmaksas izmēģinājumversijas vai Microsoft Imagine Azure abonementa jaunināšana uz Pay-you-go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span><span class="sxs-lookup"><span data-stu-id="485c4-122">To upgrade a free trial, see [Upgrade your Free Trial or Microsoft Imagine Azure subscription to Pay-As-You-Go](https://docs.microsoft.com/azure/billing/billing-upgrade-azure-subscription).</span></span>
- <span data-ttu-id="485c4-123">Lai mainītu apmaksas-as-Go kontu, skatiet rakstu [Azure pay-as-Go abonementa maiņa uz citu piedāvājumu](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span><span class="sxs-lookup"><span data-stu-id="485c4-123">To change a pay-as-you-go account, see [Change your Azure Pay-As-You-Go subscription to a different offer](https://docs.microsoft.com/azure/billing/billing-how-to-switch-azure-offer).</span></span>

<span data-ttu-id="485c4-124">**Lai pievienotu vai asociētu Azure abonementu Azure Active Directory nomniekam:**</span><span class="sxs-lookup"><span data-stu-id="485c4-124">**To add or associate an Azure subscription to your Azure Active Directory tenant:**</span></span>

1. <span data-ttu-id="485c4-125">Pierakstieties un atlasiet abonementu, kuru vēlaties izmantot [Azure portāla lapā abonementi](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span><span class="sxs-lookup"><span data-stu-id="485c4-125">Sign in and select the subscription you want to use from the [Subscriptions page in Azure portal](https://portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade).</span></span>
2. <span data-ttu-id="485c4-126">Atlasiet **mainīt direktoriju**.</span><span class="sxs-lookup"><span data-stu-id="485c4-126">Select **Change directory**.</span></span>
3. <span data-ttu-id="485c4-127">Pārskatiet brīdinājumus, kas tiek parādīti, un pēc tam atlasiet **mainīt**.</span><span class="sxs-lookup"><span data-stu-id="485c4-127">Review any warnings that appear, and then select **Change**.</span></span>
4. <span data-ttu-id="485c4-128">Direktorijs ir mainīts abonementam, un jūs saņemsit ziņojumu par veiksmīgu izdošanos.</span><span class="sxs-lookup"><span data-stu-id="485c4-128">The directory is changed for the subscription and you will get a success message.</span></span>
5. <span data-ttu-id="485c4-129">Izmantojiet *direktoriju* pārslēdzēju, lai pārietu uz jauno direktoriju.</span><span class="sxs-lookup"><span data-stu-id="485c4-129">Use the *Directory* switcher to go to your new directory.</span></span> <span data-ttu-id="485c4-130">Lai viss tiktu rādīts pareizi, var būt nepieciešamas līdz pat 10 minūtēm.</span><span class="sxs-lookup"><span data-stu-id="485c4-130">It may take up to 10 minutes for everything to show up properly.</span></span>

<span data-ttu-id="485c4-131">**Ieteicamie dokumenti**</span><span class="sxs-lookup"><span data-stu-id="485c4-131">**Recommended Documents**</span></span>

- [<span data-ttu-id="485c4-132">Azure abonementa īpašumtiesību nodošana</span><span class="sxs-lookup"><span data-stu-id="485c4-132">Transferring ownership of an Azure subscription</span></span>](https://docs.microsoft.com/azure/billing-subscription-transfer)
- [<span data-ttu-id="485c4-133">Pārvietot resursus uz jauno resursu grupu vai abonementu</span><span class="sxs-lookup"><span data-stu-id="485c4-133">Move resources to new resource group or subscription</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-move-resources)
- [<span data-ttu-id="485c4-134">Resursu pārvaldība, izmantojot Azure Portal</span><span class="sxs-lookup"><span data-stu-id="485c4-134">Manage resources using Azure portal</span></span>](https://docs.microsoft.com/azure/azure-resource-manager/resource-group-portal)
