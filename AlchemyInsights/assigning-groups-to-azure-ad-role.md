---
title: Grupu piešķiršana Azure AD lomai
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7898"
- "9003230"
ms.openlocfilehash: feca81fe785bc45e47f6faa876230b5c7701713d
ms.sourcegitcommit: 6dc6f999e840c90694a246b90062950205679420
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885070"
---
# <a name="assigning-groups-to-azure-ad-role"></a><span data-ttu-id="7ad40-102">Grupu piešķiršana Azure AD lomai</span><span class="sxs-lookup"><span data-stu-id="7ad40-102">Assigning groups to Azure AD role</span></span>

<span data-ttu-id="7ad40-103">Lai pakalpojumā Azure AD piešķirtu Azure AD grupu ar administratora reklāmas pilnvarām, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="7ad40-103">To assign an Azure AD group with source of authority in Azure AD to an Azure AD role, perform the following steps:</span></span>

1. <span data-ttu-id="7ad40-104">Izveidot jaunu grupu — lai izveidotu jaunu grupu:</span><span class="sxs-lookup"><span data-stu-id="7ad40-104">Create a new group - To create a new group:</span></span>

    <span data-ttu-id="7ad40-105">izveide.</span><span class="sxs-lookup"><span data-stu-id="7ad40-105">a.</span></span> <span data-ttu-id="7ad40-106">Pierakstieties Azure AD administrēšanas centrā ar **privileģētās lomas administratoru** vai **globālā administratora** atļaujām.</span><span class="sxs-lookup"><span data-stu-id="7ad40-106">Sign in to the Azure AD admin center with **privileged role administrator** or **global administrator** permissions.</span></span>
    <span data-ttu-id="7ad40-107">b.</span><span class="sxs-lookup"><span data-stu-id="7ad40-107">b.</span></span> <span data-ttu-id="7ad40-108">Atlasiet **Azure Active Directory > grupas > visas grupas > jauna grupa**.</span><span class="sxs-lookup"><span data-stu-id="7ad40-108">Select **Azure Active Directory > Groups > All groups > New group**.</span></span>
    <span data-ttu-id="7ad40-109">c.</span><span class="sxs-lookup"><span data-stu-id="7ad40-109">c.</span></span> <span data-ttu-id="7ad40-110">Izveidot grupu.</span><span class="sxs-lookup"><span data-stu-id="7ad40-110">Create the group.</span></span>

2. <span data-ttu-id="7ad40-111">Piešķiriet lomu grupai grupas izveides laikā vai pēc tam, kad grupa ir izveidota.</span><span class="sxs-lookup"><span data-stu-id="7ad40-111">Assign the role to the group either during group creation or after the group is created.</span></span>

    <span data-ttu-id="7ad40-112">izveide.</span><span class="sxs-lookup"><span data-stu-id="7ad40-112">a.</span></span> <span data-ttu-id="7ad40-113">Lai piešķirtu grupai lomu grupas izveides laikā, pārslēdzieties uz pārslēgšanas **AZURE ad lomām var piešķirt grupai** un izveidot grupu.</span><span class="sxs-lookup"><span data-stu-id="7ad40-113">To assign a role to the group at the time of group creation, switch on the toggle **Azure AD roles can be assigned to the group** and create the group.</span></span>
    <span data-ttu-id="7ad40-114">b.</span><span class="sxs-lookup"><span data-stu-id="7ad40-114">b.</span></span> <span data-ttu-id="7ad40-115">Lai piešķirtu lomu grupai pēc tās izveides, pārejiet uz jaunizveidotās grupas cilni **piešķirtās lomas** un piešķiriet lomai grupu.</span><span class="sxs-lookup"><span data-stu-id="7ad40-115">To assign a role to the group after it has been created, navigate to the **Assigned roles** tab for the newly created group, and assign the role to the group.</span></span>  

<span data-ttu-id="7ad40-116">**Azure AD lomai piešķirtas grupas dalības pārvaldība**</span><span class="sxs-lookup"><span data-stu-id="7ad40-116">**Manage membership of a group that is assigned to Azure AD role**</span></span>

<span data-ttu-id="7ad40-117">Lai izvairītos no privilēģiju palielināšanas, pēc noklusējuma tikai privileģētas lomas administratori un globālie administratori var modificēt lomai piešķirtās grupas dalību.</span><span class="sxs-lookup"><span data-stu-id="7ad40-117">To prevent elevation of privileges, by default, only privileged role administrators and global administrators can modify the membership of a group that is assigned to a role.</span></span> <span data-ttu-id="7ad40-118">Tomēr viņi var izvēlēties piešķirt šīs grupas īpašnieku un deleģēt šo uzdevumu.</span><span class="sxs-lookup"><span data-stu-id="7ad40-118">They can, however, choose to assign an owner for such a group and delegate this task.</span></span>

<span data-ttu-id="7ad40-119">Lai iegūtu papildinformāciju par mākoņa grupu piešķiršanu Azure AD lomām, skatiet rakstu [reklāmas lomu piešķiršana mākonī](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span><span class="sxs-lookup"><span data-stu-id="7ad40-119">For more details on assigning cloud groups to Azure AD roles, see [Assign a AD roles to Cloud Group](https://docs.microsoft.com/azure/active-directory/roles/groups-concept).</span></span> <span data-ttu-id="7ad40-120">Lai iegūtu papildinformāciju par mākoņa grupām piešķirtām lomām, skatiet sadaļu [mākoņu grupām piešķirto lomu problēmu novēršana](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span><span class="sxs-lookup"><span data-stu-id="7ad40-120">For more details on troubleshooting roles assigned to cloud groups, see [Troubleshoot roles assigned to cloud groups](https://docs.microsoft.com/azure/active-directory/roles/groups-faq-troubleshooting).</span></span>





