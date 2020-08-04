---
title: Problēmas, izmantojot Intune administrēšanas konsoli
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/29/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1790"
- "9000214"
ms.openlocfilehash: 7a36d502a92d360b06336ccfa6183f666f0260ab
ms.sourcegitcommit: ffbed67c0a16ec423fa1d79b71e48ea4e2d320e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/29/2020
ms.locfileid: "46555385"
---
# <a name="problems-using-the-intune-admin-console"></a><span data-ttu-id="da70c-102">Problēmas, izmantojot Intune administrēšanas konsoli</span><span class="sxs-lookup"><span data-stu-id="da70c-102">Problems using the Intune admin console</span></span>

<span data-ttu-id="da70c-103">**"Piekļuve liegta", naviģējot uz Intune administrēšanas portālu.**</span><span class="sxs-lookup"><span data-stu-id="da70c-103">**"Access denied" when navigating the Intune admin portal.**</span></span>

- <span data-ttu-id="da70c-104">Ja esat Intune pielāgotās lomas dalībnieks, pārliecinieties, vai jūsu kontam ir piešķirta Windows Intune vai Enterprise Mobility Suite (EMS) licence.</span><span class="sxs-lookup"><span data-stu-id="da70c-104">If you are a member of an Intune custom role, ensure that an Intune or Enterprise Mobility Suite (EMS) license is assigned to your account.</span></span>
- <span data-ttu-id="da70c-105">Ja izmantojat konfigurācijas pārvaldnieku, lai pārvaldītu ierīces, pārbaudiet, vai jums nav daļa no Intune lietotāju kolekcijas konfigurēšanas pārvaldnieka MDM.</span><span class="sxs-lookup"><span data-stu-id="da70c-105">If you are using Configuration Manager to manage devices, verify you are not part of the Intune user collection for Configuration Manager MDM.</span></span>
- <span data-ttu-id="da70c-106">Pārbaudiet, vai jums ir piešķirtas atbilstošas administrēšanas vadīklas (RBAC) atļaujas Windows Intune lomas asmeņā.</span><span class="sxs-lookup"><span data-stu-id="da70c-106">Verify that you have been assigned the appropriate role-based administration control (RBAC) permissions in the Intune roles blade.</span></span>
- <span data-ttu-id="da70c-107">Pārbaudiet, vai izmantotā grupa nav adresātu saraksts.</span><span class="sxs-lookup"><span data-stu-id="da70c-107">Verify the group used is not a distribution list.</span></span> <span data-ttu-id="da70c-108">Windows Intune Azure portālā atbalsta tikai to lietotāju kontus, kas pieder Azure Active Directory drošības grupām.</span><span class="sxs-lookup"><span data-stu-id="da70c-108">Intune in the Azure portal only supports user accounts that belong to Azure Active Directory security groups.</span></span> <span data-ttu-id="da70c-109">Pārskatiet savas grupas Azure portālā > **Intune**  >  **groups**vai Azure portālā > **Azure Active Directory**.</span><span class="sxs-lookup"><span data-stu-id="da70c-109">Review your groups in the Azure portal > **Intune** > **Groups**, or in Azure portal > **Azure Active Directory**.</span></span>

<span data-ttu-id="da70c-110">**Lietotājam ir pārāk daudz atļauju piešķirtajai Intune lomai**</span><span class="sxs-lookup"><span data-stu-id="da70c-110">**User has too many permissions for assigned Intune role**</span></span>

<span data-ttu-id="da70c-111">Ieteikt lietotājam pāriet uz **Intune**  >  **Intune lomām**  >  **manas atļaujas**  >  **Eksportēt** , lai pārskatītu piešķirtās atļaujas.</span><span class="sxs-lookup"><span data-stu-id="da70c-111">Advise the user to go to **Intune** > **Intune roles** > **My permissions** > **Export** to review granted permissions.</span></span>

<span data-ttu-id="da70c-112">**Esmu pievienojis tvēruma grupu lomai, taču šīs lomas lietotāji joprojām redz citus lietotājus vai ierīces.**</span><span class="sxs-lookup"><span data-stu-id="da70c-112">**I added a scope group to a role, but users in that role still see other users or devices.**</span></span>

<span data-ttu-id="da70c-113">Tvērumu grupas nefiltrē lietotājus vai ierīces.</span><span class="sxs-lookup"><span data-stu-id="da70c-113">Scope groups do not filter out users or devices.</span></span> <span data-ttu-id="da70c-114">Tvērumu grupas:</span><span class="sxs-lookup"><span data-stu-id="da70c-114">Scope groups:</span></span>

- <span data-ttu-id="da70c-115">Ierobežojiet to, kam lietotāji var piešķirt politikas vai lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="da70c-115">Limit who users can assign policies or applications to.</span></span>
- <span data-ttu-id="da70c-116">Atļaut tikai konkrētiem lietotājiem palaist attālos uzdevumus ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="da70c-116">Allow only specific users to run remote tasks on devices.</span></span>

<span data-ttu-id="da70c-117">Papildinformāciju par tvērumu grupām skatiet rakstā [lomu piekļuves vadība (RBAC) ar Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="da70c-117">For more information about scope groups, see  [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="da70c-118">**Pievienoju lietotāju Intune lomai, bet joprojām ir pilna piekļuve Intune administrēšanas konsolei.**</span><span class="sxs-lookup"><span data-stu-id="da70c-118">**I added a user to an Intune role but they still have full access to the Intune admin console.**</span></span>

<span data-ttu-id="da70c-119">Pārejiet uz Intune > **lietotājiem** Azure portālā un pārbaudiet, vai lietotājam nav piešķirta neviena no šīm lomām Azure portālā:</span><span class="sxs-lookup"><span data-stu-id="da70c-119">Navigate to Intune > **Users** in the Azure portal and verify that the user is not assigned to any of the following roles in the Azure portal:</span></span>

- <span data-ttu-id="da70c-120">Globālais administrators</span><span class="sxs-lookup"><span data-stu-id="da70c-120">Global administrator</span></span>
- <span data-ttu-id="da70c-121">Intune pakalpojuma administrators</span><span class="sxs-lookup"><span data-stu-id="da70c-121">Intune service administrator</span></span>
- <span data-ttu-id="da70c-122">SharePoint administrators</span><span class="sxs-lookup"><span data-stu-id="da70c-122">SharePoint administrator</span></span>

<span data-ttu-id="da70c-123">Papildinformāciju skatiet rakstā [lomu piekļuves vadība (RBAC) ar Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span><span class="sxs-lookup"><span data-stu-id="da70c-123">For more info, see [Role-based access control (RBAC) with Microsoft Intune](https://docs.microsoft.com/intune/role-based-access-control).</span></span>

<span data-ttu-id="da70c-124">**Access problēmas**</span><span class="sxs-lookup"><span data-stu-id="da70c-124">**Access Issues**</span></span>

<span data-ttu-id="da70c-125">Papildinformāciju skatiet rakstā [nevar pierakstīties pakalpojumā Office 365, Azure vai Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span><span class="sxs-lookup"><span data-stu-id="da70c-125">For more info, see [You can't sign in to Office 365, Azure, or Intune](https://support.microsoft.com/help/2412085/you-can-t-sign-in-to-office-365-azure-or-intune).</span></span>