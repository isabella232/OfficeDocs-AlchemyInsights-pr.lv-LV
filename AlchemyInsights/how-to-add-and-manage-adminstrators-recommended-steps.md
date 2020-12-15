---
title: Administratora ieteicamo darbību pievienošana un pārvaldība
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/07/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004114"
- "7194"
ms.openlocfilehash: 142bf1474ac0e0eac5cecb9dddd35e28b6b6631e
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677800"
---
# <a name="how-to-add-and-manage-adminstrators---recommended-steps"></a><span data-ttu-id="fa83b-102">Administratora ieteicamo darbību pievienošana un pārvaldība</span><span class="sxs-lookup"><span data-stu-id="fa83b-102">How to add and manage adminstrators - recommended steps</span></span>

<span data-ttu-id="fa83b-103">**Abonementa administratora vai sadarbības ar administratoru rediģēšana**</span><span class="sxs-lookup"><span data-stu-id="fa83b-103">**Edit the Subscription Administrator or Co-administrator**</span></span>

- <span data-ttu-id="fa83b-104">Konta administrators var rediģēt abas lomas, bet abonementa administrators var mainīt tikai sadarbības administratorus [Azure portālā](https://ms.portal.azure.com/#home).</span><span class="sxs-lookup"><span data-stu-id="fa83b-104">The Account Administrator can edit both roles whereas the Subscription Administrator can only change Co-administrators in the [Azure portal](https://ms.portal.azure.com/#home).</span></span>
- [<span data-ttu-id="fa83b-105">Azure abonementu administratoru pievienošana vai maiņa</span><span class="sxs-lookup"><span data-stu-id="fa83b-105">Add or change Azure subscription administrators</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/add-change-subscription-administrator)

<span data-ttu-id="fa83b-106">**Atjauniniet abonementa administratoru vai Co-Administrator iekšējiem (AIRS) abonementiem**</span><span class="sxs-lookup"><span data-stu-id="fa83b-106">**Update the Subscription Administrator or Co-Administrator for Internal (AIRS) Subscriptions**</span></span>

<span data-ttu-id="fa83b-107">Pakalpojumu administrators vai sadarbības administrators var pats veikt šo darbību, veicot tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="fa83b-107">The Service Administrator or the Co-administrator can self-serve this action by using the following steps:</span></span>

1. <span data-ttu-id="fa83b-108">Piesakieties [Azure portālā](https://ms.portal.azure.com/#home) un kreisajā pusē noklikšķiniet uz **izmaksu pārvaldība + norēķini** .</span><span class="sxs-lookup"><span data-stu-id="fa83b-108">Log in to the [Azure portal](https://ms.portal.azure.com/#home) and click **Cost Management + Billing** in the left blade.</span></span>
2. <span data-ttu-id="fa83b-109">Noklikšķiniet uz līnijas vienuma ar savu abonementu.</span><span class="sxs-lookup"><span data-stu-id="fa83b-109">Click on the line item with your subscription.</span></span> <span data-ttu-id="fa83b-110">Tiks atvērts pārskats par jūsu abonementu.</span><span class="sxs-lookup"><span data-stu-id="fa83b-110">This opens the Overview for your subscription.</span></span>
3. <span data-ttu-id="fa83b-111">**Abonementa** asmeņā noklikšķiniet uz **Rekvizīti**.</span><span class="sxs-lookup"><span data-stu-id="fa83b-111">On the **Subscription** blade, click **Properties**.</span></span> 
4. <span data-ttu-id="fa83b-112">Noklikšķiniet uz pogas **pakalpojumu administrators** .</span><span class="sxs-lookup"><span data-stu-id="fa83b-112">Click the **Service Admin** button.</span></span>
5. <span data-ttu-id="fa83b-113">Ievadiet tā lietotāja e-pasta adresi, kuru vēlaties iestatīt kā pakalpojuma administratoru, un noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="fa83b-113">Enter the email of the user whom you want to set as a Service Administrator and click **OK**.</span></span>

<span data-ttu-id="fa83b-114">**Pievienot/mainīt/noņemt administratoru**</span><span class="sxs-lookup"><span data-stu-id="fa83b-114">**Add/Change/Remove Co-administrator**</span></span>

1. <span data-ttu-id="fa83b-115">Piesakieties [Azure portālā](https://ms.portal.azure.com/#home) kā pakalpojumu administrators.</span><span class="sxs-lookup"><span data-stu-id="fa83b-115">Log in to the [Azure portal](https://ms.portal.azure.com/#home) as a Service Administrator.</span></span>
2. <span data-ttu-id="fa83b-116">Atveriet [abonementus](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) un atlasiet abonementu.</span><span class="sxs-lookup"><span data-stu-id="fa83b-116">Open [Subscriptions](https://ms.portal.azure.com/#blade/Microsoft_Azure_Billing/SubscriptionsBlade) and select a subscription.</span></span> <span data-ttu-id="fa83b-117">(Līdzstrādniekus var piešķirt tikai abonementa tvērumā).</span><span class="sxs-lookup"><span data-stu-id="fa83b-117">(Co-adminstrators can only be assigned at the subscription scope.)</span></span>
3. <span data-ttu-id="fa83b-118">Pārejiet uz **Access vadības (IAM)**  >  **klasiskajiem administratoriem**  >  **Pievienot**  >  **administratoru** , lai atvērtu rūti **Add-admin** (ja opcija Pievienot sadarbības administratoru ir atspējota, tas norāda, ka jums nav atļauju).</span><span class="sxs-lookup"><span data-stu-id="fa83b-118">Navigate to **Access control (IAM)** > **Classic administrators** > **Add** > **Add co-administrator** to open the **Add co-admin** pane (If the Add co-administrator option is disabled, it denotes that you do not have permissions).</span></span>
4. <span data-ttu-id="fa83b-119">Atlasiet lietotāju, kuru vēlaties pievienot, un noklikšķiniet uz **Pievienot**.</span><span class="sxs-lookup"><span data-stu-id="fa83b-119">Select the user whom you want to add and click **Add**.</span></span>

<span data-ttu-id="fa83b-120">**apgūt vairāk:**</span><span class="sxs-lookup"><span data-stu-id="fa83b-120">**Learn more:**</span></span>
- [<span data-ttu-id="fa83b-121">Pievienojiet sadarbības administratoru</span><span class="sxs-lookup"><span data-stu-id="fa83b-121">Add a Co-Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="fa83b-122">Administratora noņemšana</span><span class="sxs-lookup"><span data-stu-id="fa83b-122">Remove a co-administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="fa83b-123">Pakalpojuma administratora mainīšana</span><span class="sxs-lookup"><span data-stu-id="fa83b-123">Change the Service Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="fa83b-124">Konta administratora skatīšana</span><span class="sxs-lookup"><span data-stu-id="fa83b-124">View the Account Administrator</span></span>](https://docs.microsoft.com/azure/role-based-access-control/classic-administrators)
- [<span data-ttu-id="fa83b-125">Piekļuves pārvaldība, izmantojot RBAC un Azure portālu</span><span class="sxs-lookup"><span data-stu-id="fa83b-125">Manage access using RBAC and Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/role-assignments-portal)

<span data-ttu-id="fa83b-126">**Lietotāju pievienošana/dzēšana, izmantojot Azure Active Directory (AD)**</span><span class="sxs-lookup"><span data-stu-id="fa83b-126">**Add/delete users using Azure Active Directory (AD)**</span></span>

<span data-ttu-id="fa83b-127">Varat pievienot jaunus lietotājus vai izdzēst esošos lietotājus no pakalpojuma Azure Active Directory (Azure AD) organizācijas:</span><span class="sxs-lookup"><span data-stu-id="fa83b-127">You can add new users or delete existing users from your Azure Active Directory (Azure AD) organization:</span></span>

1. <span data-ttu-id="fa83b-128">Lai pievienotu jaunu lietotāju, piesakieties [Azure portālā](https://ms.portal.azure.com/#home) kā lietotāja administrators organizācijai.</span><span class="sxs-lookup"><span data-stu-id="fa83b-128">To add a new user, log in to the [Azure portal](https://ms.portal.azure.com/#home) as a User-administrator for the organization.</span></span>
2. <span data-ttu-id="fa83b-129">Atlasiet **Azure Active Directory**, atlasiet **lietotāji** un pēc tam noklikšķiniet uz **Jauns lietotājs**.</span><span class="sxs-lookup"><span data-stu-id="fa83b-129">Select **Azure Active Directory**, select **Users** and then click **New user**.</span></span>
3. <span data-ttu-id="fa83b-130">**Lietotāja** lapā aizpildiet nepieciešamo informāciju.</span><span class="sxs-lookup"><span data-stu-id="fa83b-130">On the **User** page, fill out the required information.</span></span> <span data-ttu-id="fa83b-131">Noklikšķiniet uz **izveidot**.</span><span class="sxs-lookup"><span data-stu-id="fa83b-131">Click **Create**.</span></span> <span data-ttu-id="fa83b-132">Lietotājs tiek izveidots un pievienots jūsu Azure AD nomniekam.</span><span class="sxs-lookup"><span data-stu-id="fa83b-132">The user is created and added to your Azure AD tenant.</span></span>

<span data-ttu-id="fa83b-133">**Papildinformācija**:</span><span class="sxs-lookup"><span data-stu-id="fa83b-133">**Learn more**:</span></span>

- [<span data-ttu-id="fa83b-134">Jauna lietotāja pievienošana</span><span class="sxs-lookup"><span data-stu-id="fa83b-134">Add a new user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="fa83b-135">Lietotāja dzēšana</span><span class="sxs-lookup"><span data-stu-id="fa83b-135">Delete a user</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/add-users-azure-active-directory)
- [<span data-ttu-id="fa83b-136">Lietotāja profila informācijas pievienošana vai atjaunināšana, izmantojot Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="fa83b-136">Add or update a user's profile information using Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-users-profile-azure-portal)

<span data-ttu-id="fa83b-137">**Ieteicamie dokumenti**</span><span class="sxs-lookup"><span data-stu-id="fa83b-137">**Recommended documents**</span></span>

- [<span data-ttu-id="fa83b-138">Kas ir lomu piekļuves vadība (RBAC)?</span><span class="sxs-lookup"><span data-stu-id="fa83b-138">What is role-based access control (RBAC)?</span></span>](https://docs.microsoft.com/azure/role-based-access-control/overview)
- [<span data-ttu-id="fa83b-139">Izpratne par dažādām Azure lomām</span><span class="sxs-lookup"><span data-stu-id="fa83b-139">Understand the different roles in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/rbac-and-directory-admin-roles)
- [<span data-ttu-id="fa83b-140">Administratora lomu atļaujas Azure Active Directory</span><span class="sxs-lookup"><span data-stu-id="fa83b-140">Administrator role permissions in Azure Active Directory</span></span>](https://docs.microsoft.com/azure/active-directory/roles/permissions-reference)
- [<span data-ttu-id="fa83b-141">Apmācība: piekļuves piešķiršana lietotājam, izmantojot RBAC un Azure portālu</span><span class="sxs-lookup"><span data-stu-id="fa83b-141">Tutorial: Grant access for a user using RBAC and the Azure portal</span></span>](https://docs.microsoft.com/azure/role-based-access-control/quickstart-assign-role-user-portal)
- [<span data-ttu-id="fa83b-142">RBAC problēmu novēršana pakalpojumā Azure</span><span class="sxs-lookup"><span data-stu-id="fa83b-142">Troubleshoot RBAC in Azure</span></span>](https://docs.microsoft.com/azure/role-based-access-control/troubleshooting)
- [<span data-ttu-id="fa83b-143">Resursu organizēšana, izmantojot Azure Management groups</span><span class="sxs-lookup"><span data-stu-id="fa83b-143">Organize your resources with Azure management groups</span></span>](https://docs.microsoft.com/azure/governance/management-groups/overview)
- [<span data-ttu-id="fa83b-144">Kā pieprasīt Azure rēķina kopiju pa e-pastu</span><span class="sxs-lookup"><span data-stu-id="fa83b-144">How to request copy of Azure invoice via email</span></span>](https://azure.microsoft.com/en-us/blog/azure-email-invoices/)
- [<span data-ttu-id="fa83b-145">Kredītkartes vai debetkartes pievienošana, atjaunināšana vai noņemšana no Azure</span><span class="sxs-lookup"><span data-stu-id="fa83b-145">How to add, update or remove a credit or debit card from Azure</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card)
- [<span data-ttu-id="fa83b-146">Pārvaldīt (atkārtoti aktivizēt/atcelt/mainīt) abonementu</span><span class="sxs-lookup"><span data-stu-id="fa83b-146">Manage (Reactivate/Cancel/Switch) subscription</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/subscription-disabled)



