---
title: Iespējot izmaksu pārvaldību
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003547"
- "6463"
ms.openlocfilehash: 0bbf1158f7f5fa8a22cfe7242c86760057fc7bab
ms.sourcegitcommit: 0f26f6b23b3d48c3c6cddf98bc41df484f16cb00
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677739"
---
# <a name="enable-cost-management"></a><span data-ttu-id="b9d79-102">Iespējot izmaksu pārvaldību</span><span class="sxs-lookup"><span data-stu-id="b9d79-102">Enable cost management</span></span>

<span data-ttu-id="b9d79-103">**Ko nozīmē jūsu organizācijas izmaksas ir atspējotas?**</span><span class="sxs-lookup"><span data-stu-id="b9d79-103">**What does 'costs are disabled for your organization' mean?**</span></span>

<span data-ttu-id="b9d79-104">Organizācijas, kas izmanto Enterprise Agreement (EA) vai Microsoft klientu līguma (MCA) kontus, var atspējot piekļuvi informācijai par izmaksām un cenām.</span><span class="sxs-lookup"><span data-stu-id="b9d79-104">Organizations using Enterprise Agreement (EA) or Microsoft Customer Agreement (MCA) accounts can disable access to cost information and pricing information.</span></span>

<span data-ttu-id="b9d79-105">Pēc pierakstīšanās Azure portālā viņi var izmantot norēķinu API, lai programmatiski iegūtu rēķinus (pēc pierakstīšanās) un izmantošanas informāciju.</span><span class="sxs-lookup"><span data-stu-id="b9d79-105">After logging in to Azure portal, they can use the Billing APIs to programmatically get invoices (once opted-in) and usage details.</span></span>

<span data-ttu-id="b9d79-106">**Kā atļaut papildu lietotājiem piekļūt rēķiniem**</span><span class="sxs-lookup"><span data-stu-id="b9d79-106">**How to allow additional users to access invoices**</span></span>

1. <span data-ttu-id="b9d79-107">Dodieties uz **abonementu diska** Azure portālā.</span><span class="sxs-lookup"><span data-stu-id="b9d79-107">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="b9d79-108">Atlasiet **rēķini** un pēc tam **piekļūstiet rēķiniem**.</span><span class="sxs-lookup"><span data-stu-id="b9d79-108">Select **Invoices** and then **Access to invoices**.</span></span>
3. <span data-ttu-id="b9d79-109">Ieslēdziet programmu Access, pēc tam saglabājot izmaiņas, lai atļautu lietotājiem abonementa atkārtotās lomas lejupielādēt rēķinus.</span><span class="sxs-lookup"><span data-stu-id="b9d79-109">Turn on the access, followed by saving the changes, to allow users in subscription-scoped roles to download invoices.</span></span>

> [!NOTE]
> <span data-ttu-id="b9d79-110">Konta administrators var arī konfigurēt, lai rēķini tiktu sūtīti pa e-pastu.</span><span class="sxs-lookup"><span data-stu-id="b9d79-110">The Account Administrator can also configure to have invoices sent via email.</span></span> <span data-ttu-id="b9d79-111">Lai uzzinātu vairāk, skatiet rakstu [rēķina saņemšana pa e-pastu](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span><span class="sxs-lookup"><span data-stu-id="b9d79-111">To learn more, see [Get your invoice in email](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?).</span></span>

<span data-ttu-id="b9d79-112">**Kā pievienot lietotājus norēķinu lasītāja lomai**</span><span class="sxs-lookup"><span data-stu-id="b9d79-112">**How to add users to the Billing Reader role**</span></span>

1. <span data-ttu-id="b9d79-113">Dodieties uz **abonementu diska** Azure portālā.</span><span class="sxs-lookup"><span data-stu-id="b9d79-113">Go to **Subscriptions blade** in Azure portal.</span></span>
2. <span data-ttu-id="b9d79-114">Atlasiet **piekļuves vadība (IAM)** un pēc tam noklikšķiniet uz **Pievienot**.</span><span class="sxs-lookup"><span data-stu-id="b9d79-114">Select **Access control (IAM)** and then click **Add**.</span></span>
3. <span data-ttu-id="b9d79-115">Lapā **Atlasīt lomu** izvēlieties **norēķinu lasītājs** .</span><span class="sxs-lookup"><span data-stu-id="b9d79-115">Choose **Billing Reader** in the **Select a role** page.</span></span>
4. <span data-ttu-id="b9d79-116">Ierakstiet tā lietotāja e-pasta adresi, kuru vēlaties uzaicināt, un pēc tam noklikšķiniet uz **Labi** , lai nosūtītu uzaicinājumu.</span><span class="sxs-lookup"><span data-stu-id="b9d79-116">Type the email of the user you want to invite, and then click **OK** to send the invitation.</span></span>
5. <span data-ttu-id="b9d79-117">Izpildiet norādījumus, kas sniegti uzaicinājuma e-pasta ziņojumā, lai pieteiktos kā norēķinu lasītājs.</span><span class="sxs-lookup"><span data-stu-id="b9d79-117">Follow instructions provided in the invite email to log in as a billing reader.</span></span> <span data-ttu-id="b9d79-118">Papildinformāciju skatiet rakstā [piekļuves piešķiršana norēķiniem](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span><span class="sxs-lookup"><span data-stu-id="b9d79-118">For more information, see [Grant access to Billing](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support#opt-in).</span></span>

<span data-ttu-id="b9d79-119">**Ieteicamie dokumenti**</span><span class="sxs-lookup"><span data-stu-id="b9d79-119">**Recommended documents**</span></span>

- [<span data-ttu-id="b9d79-120">DA un AO skatu iespējošana, izmantojot EA portālu</span><span class="sxs-lookup"><span data-stu-id="b9d79-120">Enable DA and AO views via EA portal</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/assign-access-acm-data?WT.mc_id=Portal-Microsoft_Azure_Support#enable-access-to-costs-in-the-ea-portal)
- [<span data-ttu-id="b9d79-121">Izmaksu vadībā iekļautās izmaksas</span><span class="sxs-lookup"><span data-stu-id="b9d79-121">Costs included in Cost Management</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#costs-included-in-cost-management)
- [<span data-ttu-id="b9d79-122">Atbalstītie Microsoft Azure piedāvājumi</span><span class="sxs-lookup"><span data-stu-id="b9d79-122">Supported Microsoft Azure Offers</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/understand-cost-mgt-data?WT.mc_id=Portal-Microsoft_Azure_Support#supported-microsoft-azure-offers)
- [<span data-ttu-id="b9d79-123">Izmaksu analīzes izmaksas</span><span class="sxs-lookup"><span data-stu-id="b9d79-123">Review costs in cost analysis</span></span>](https://docs.microsoft.com/azure/cost-management-billing/costs/quick-acm-cost-analysis?WT.mc_id=Portal-Microsoft_Azure_Support&tabs=azure-portal#review-costs-in-cost-analysis)
- [<span data-ttu-id="b9d79-124">Piekļuve norēķinu informācijai</span><span class="sxs-lookup"><span data-stu-id="b9d79-124">Provide access to billing information</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/manage-billing-access?WT.mc_id=Portal-Microsoft_Azure_Support)
- [<span data-ttu-id="b9d79-125">Piekļuves pārbaude Microsoft klienta līgumam</span><span class="sxs-lookup"><span data-stu-id="b9d79-125">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/download-azure-invoice-daily-usage-date?WT.mc_id=Portal-Microsoft_Azure_Support#check-access-to-a-microsoft-customer-agreement)






