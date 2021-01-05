---
title: Kā pievienot un pārvaldīt administratorus
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
ms.openlocfilehash: 25fc25392778ae71ec0553e8d8718ec487738acb
ms.sourcegitcommit: 04bf13605a30ad4a2218ad9e94dcffcee4cc9aa6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/05/2021
ms.locfileid: "49755502"
---
# <a name="how-to-add-and-manage-admins"></a><span data-ttu-id="5ee99-102">Kā pievienot un pārvaldīt administratorus</span><span class="sxs-lookup"><span data-stu-id="5ee99-102">How to add and manage admins</span></span>

<span data-ttu-id="5ee99-103">Ņemot vērā jūsu problēmas aprakstu, mēs esam atraduši risinājumu.</span><span class="sxs-lookup"><span data-stu-id="5ee99-103">Based on your issue description, we’ve found a solution for you.</span></span> <span data-ttu-id="5ee99-104">Lielākā daļa klientu varēja atrisināt šo problēmu patstāvīgi pēc mūsu dokumentācijas.</span><span class="sxs-lookup"><span data-stu-id="5ee99-104">Most customers were able to resolve their issue on their own after following our documentation.</span></span>

<span data-ttu-id="5ee99-105">Lai pārvaldītu savu norēķinu kontu Microsoft klienta līgumam (MCA), varat izmantot atšķirīgas lomas ar vēlamo piekļuves līmeni.</span><span class="sxs-lookup"><span data-stu-id="5ee99-105">To manage your billing account for a Microsoft Customer Agreement (MCA), you can use different roles with the desired level of access.</span></span> <span data-ttu-id="5ee99-106">Šīs lomas ir papildus iebūvētajām Azure pakalpojumu lomām, kas palīdz pārvaldīt resursus.</span><span class="sxs-lookup"><span data-stu-id="5ee99-106">These roles are in addition to the built-in Azure service roles which help you control your resources.</span></span>

<span data-ttu-id="5ee99-107">**Lai pievienotu norēķinu lomas Azure portālā:**</span><span class="sxs-lookup"><span data-stu-id="5ee99-107">**To add billing roles in the Azure portal:**</span></span>

1. <span data-ttu-id="5ee99-108">Pierakstieties [Azure portālā](https://portal.azure.com/).</span><span class="sxs-lookup"><span data-stu-id="5ee99-108">Sign in to the [Azure portal](https://portal.azure.com/).</span></span>
2. <span data-ttu-id="5ee99-109">Meklējiet *izmaksu pārvaldību + norēķini*.</span><span class="sxs-lookup"><span data-stu-id="5ee99-109">Search for *Cost Management + Billing*.</span></span>
3. <span data-ttu-id="5ee99-110">Atlasiet piekļuves vadība (IAM) tādā tvērumā kā norēķinu konts, norēķinu profils vai rēķina sadaļa, kurā vēlaties piešķirt piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="5ee99-110">Select Access control (IAM) at a scope such as billing account, billing profile, or invoice section where you want to give access.</span></span>
4. <span data-ttu-id="5ee99-111">Piekļuves vadības (IAM) lapā ir uzskaitīti lietotāji un grupas, kas piešķirti katrai lomai šajā tvērumā.</span><span class="sxs-lookup"><span data-stu-id="5ee99-111">The Access control (IAM) page lists users and groups that are assigned to each role for that scope.</span></span>
5. <span data-ttu-id="5ee99-112">Lai piešķirtu piekļuvi lietotājam, lapas augšdaļā atlasiet **Pievienot** .</span><span class="sxs-lookup"><span data-stu-id="5ee99-112">To give access to a user, select **Add** from the top of the page.</span></span> <span data-ttu-id="5ee99-113">Nolaižamajā sarakstā *lomai* atlasiet lomu.</span><span class="sxs-lookup"><span data-stu-id="5ee99-113">In the *Role* drop-down list, select a role.</span></span> <span data-ttu-id="5ee99-114">Ievadiet tā lietotāja e-pasta adresi, kuram vēlaties piešķirt piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="5ee99-114">Enter the email address of the user to whom you want to give access.</span></span> <span data-ttu-id="5ee99-115">Atlasiet **Saglabāt** , lai piešķirtu lomu.</span><span class="sxs-lookup"><span data-stu-id="5ee99-115">Select **Save** to assign the role.</span></span>
6. <span data-ttu-id="5ee99-116">Lai lietotājam noņemtu piekļuvi, atlasiet lietotāju, kura lomu vēlaties noņemt.</span><span class="sxs-lookup"><span data-stu-id="5ee99-116">To remove access for a user, select the user with the role assignment you want to remove.</span></span> <span data-ttu-id="5ee99-117">Atlasiet **Noņemt**.</span><span class="sxs-lookup"><span data-stu-id="5ee99-117">Select **Remove**.</span></span>

<span data-ttu-id="5ee99-118">**Ieteiktie dokumenti**</span><span class="sxs-lookup"><span data-stu-id="5ee99-118">**Recommended Documents**</span></span>

- [<span data-ttu-id="5ee99-119">Norēķinu lomu definīcijas</span><span class="sxs-lookup"><span data-stu-id="5ee99-119">Billing role definitions</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles)
- [<span data-ttu-id="5ee99-120">Norēķinu konta lomas un uzdevumi</span><span class="sxs-lookup"><span data-stu-id="5ee99-120">Billing account roles and tasks</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/understand-mca-roles#billing-account-roles-and-tasks)
- [<span data-ttu-id="5ee99-121">Darba sākšana ar MCA norēķinu kontu</span><span class="sxs-lookup"><span data-stu-id="5ee99-121">Get started with your MCA billing account</span></span>](https://docs.microsoft.com/azure/cost-management-billing/understand/mca-overview)
- [<span data-ttu-id="5ee99-122">Piekļuves pārbaude Microsoft klienta līgumam</span><span class="sxs-lookup"><span data-stu-id="5ee99-122">Check access to a Microsoft Customer Agreement</span></span>](https://docs.microsoft.com/azure/cost-management-billing/manage/change-credit-card?WT.mc_id=Portal-Microsoft_Azure_Support%22%20%5Cl%20%22manage-credit-cards-for-a-microsoft-customer-agreement%22%20%5Ct%20%22_blank#check-the-type-of-your-account)
