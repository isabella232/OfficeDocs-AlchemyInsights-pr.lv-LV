---
title: Kā pievienot un pārvaldīt administratorus-MCA FL/CL
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
- "9004114"
- "7424"
ms.openlocfilehash: f5791cb12e565cb04f7ac6bc9bb401fcca3e4e9e
ms.sourcegitcommit: dd9eb38bf9403de29f46c844cb64bc1d4c515afc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2020
ms.locfileid: "49692305"
---
# <a name="how-to-add-and-manage-admins---mca-flcl"></a><span data-ttu-id="afd61-102">Kā pievienot un pārvaldīt administratorus-MCA FL/CL</span><span class="sxs-lookup"><span data-stu-id="afd61-102">How to add and manage admins - MCA FL/CL</span></span>

<span data-ttu-id="afd61-103">Lai pārvaldītu savu norēķinu kontu Microsoft klienta līgumam (MCA), varat izmantot atšķirīgas lomas ar vēlamo piekļuves līmeni.</span><span class="sxs-lookup"><span data-stu-id="afd61-103">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="afd61-104">Šīs lomas ir papildus iebūvētajām Azure pakalpojumu lomām, kas palīdz pārvaldīt resursus.</span><span class="sxs-lookup"><span data-stu-id="afd61-104">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="afd61-105">**Lai pievienotu norēķinu lomas Azure portālā:**</span><span class="sxs-lookup"><span data-stu-id="afd61-105">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="afd61-106">Pierakstieties [Azure portālā](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="afd61-106">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="afd61-107">Meklējiet *izmaksu pārvaldību + norēķini*.</span><span class="sxs-lookup"><span data-stu-id="afd61-107">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="afd61-108">Atlasiet piekļuves vadība (IAM) tādā tvērumā kā norēķinu konts, norēķinu profils vai rēķina sadaļa, kurā vēlaties piešķirt piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="afd61-108">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="afd61-109">Piekļuves vadības (IAM) lapā ir uzskaitīti lietotāji un grupas, kas piešķirti katrai lomai šajā tvērumā.</span><span class="sxs-lookup"><span data-stu-id="afd61-109">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="afd61-110">Lai piešķirtu piekļuvi lietotājam, lapas augšdaļā atlasiet **Pievienot** .</span><span class="sxs-lookup"><span data-stu-id="afd61-110">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="afd61-111">Nolaižamajā sarakstā *lomai* atlasiet lomu.</span><span class="sxs-lookup"><span data-stu-id="afd61-111">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="afd61-112">Ievadiet tā lietotāja e-pasta adresi, kuram vēlaties piešķirt piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="afd61-112">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="afd61-113">Atlasiet **Saglabāt** , lai piešķirtu lomu.</span><span class="sxs-lookup"><span data-stu-id="afd61-113">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="afd61-114">Lai lietotājam noņemtu piekļuvi, atlasiet lietotāju, kura lomu vēlaties noņemt.</span><span class="sxs-lookup"><span data-stu-id="afd61-114">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="afd61-115">Atlasiet **Noņemt**.</span><span class="sxs-lookup"><span data-stu-id="afd61-115">Select **Remove**.</span></span>

<span data-ttu-id="afd61-116">**Ieteicamie dokumenti**</span><span class="sxs-lookup"><span data-stu-id="afd61-116">**Recommended Documents**</span></span>

- [<span data-ttu-id="afd61-117">Norēķinu lomu definīcijas</span><span class="sxs-lookup"><span data-stu-id="afd61-117">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="afd61-118">Norēķinu konta lomas un uzdevumi</span><span class="sxs-lookup"><span data-stu-id="afd61-118">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="afd61-119">Darba sākšana ar MCA norēķinu kontu</span><span class="sxs-lookup"><span data-stu-id="afd61-119">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="afd61-120">Piekļuves pārbaude Microsoft klienta līgumam</span><span class="sxs-lookup"><span data-stu-id="afd61-120">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
