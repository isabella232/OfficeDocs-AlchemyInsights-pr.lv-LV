---
title: Trūkst darbplūsmas neizdevās aktivizēt
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: ce088227a3206fa05b99331fdb022fbe4886203f
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32418440"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="52f6c-102">Trūkst darbplūsmas neizdevās aktivizēt</span><span class="sxs-lookup"><span data-stu-id="52f6c-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="52f6c-103">Microsoft SharePoint vietņu kolekcijas sarakstam vai bibliotēkai nevar pievienot globāli atkārtoti darbplūsmai (piemēram, "apstiprināšana - SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="52f6c-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="52f6c-104">Lai atrisinātu šo problēmu, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="52f6c-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="52f6c-105">Saknes tīmekļa vietņu kolekcijas atvēršana SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="52f6c-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="52f6c-106">Zem **Vietnes objektus**, atlasiet **darbplūsmas**.</span><span class="sxs-lookup"><span data-stu-id="52f6c-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="52f6c-107">**Jaunā** sadaļā **darbplūsmas** lentes, atlasiet **Izmantojama darbplūsmas**.</span><span class="sxs-lookup"><span data-stu-id="52f6c-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="52f6c-108">Formā **Izveidot izmantojama darbplūsmas** ievadiet nosaukumu \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="52f6c-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="52f6c-109">**Platformas tips**noklikšķiniet uz **SharePoint 2010 darbplūsma**un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="52f6c-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="52f6c-110">Sadaļā **Saglabāt** **darbplūsmas** lentes, atlasiet **publicēt**.</span><span class="sxs-lookup"><span data-stu-id="52f6c-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="52f6c-111">**Darbplūsmā** lentei sadaļā **Pārvaldīt** atlasiet **Publicēt globāli**.</span><span class="sxs-lookup"><span data-stu-id="52f6c-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="52f6c-112">Apstiprinājuma dialoglodziņā, kas parādās, izvēlieties **Labi**.</span><span class="sxs-lookup"><span data-stu-id="52f6c-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="52f6c-113">Web pārlūkprogrammā, atrast saknes tīmekļa vietņu kolekcijas, un pēc tam piekļūt **Vietnes iestatījumus** \> **Vietņu kolekcijas līdzekļus**.</span><span class="sxs-lookup"><span data-stu-id="52f6c-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="52f6c-114">Tad, pretēji **darbplūsmas** līdzeklis:</span><span class="sxs-lookup"><span data-stu-id="52f6c-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="52f6c-115">· Ja līdzeklis tiek *aktivizēts* , noklikšķiniet uz **deaktivizēt,** un pēc tam noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="52f6c-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="52f6c-116">· Ja līdzeklis ir *Deactivated* , noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="52f6c-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="52f6c-117">Plašāku informāciju skatiet šādu [pantu](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="52f6c-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

