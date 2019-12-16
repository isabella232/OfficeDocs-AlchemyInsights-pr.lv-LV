---
title: Nevar pievienot 2010 apstiprinājuma darbplūsmu
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: 11ba9bf04f826b0d7465a9a81a36c327e79f4d13
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049560"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="cc4a7-102">Nevar pievienot 2010 apstiprinājuma darbplūsmu</span><span class="sxs-lookup"><span data-stu-id="cc4a7-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="cc4a7-103">Microsoft SharePoint vietņu kolekcijas sarakstu vai bibliotēku nevar pievienot globāli atkārtoti darbplūsmas (piemēram, "apstiprinājums-SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="cc4a7-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="cc4a7-104">Lai novērstu šo problēmu, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="cc4a7-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="cc4a7-105">Atveriet vietņu kolekcijas saknes vietnē programmā SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="cc4a7-106">Sadaļā **vietnes objekti**atlasiet **darbplūsmas**.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="cc4a7-107">**Jaunajā** sadaļā **darbplūsmas** lentē atlasiet **atkārtoti izmantojama darbplūsma**.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="cc4a7-108">Veidlapā **izveidot atkārtoti izmantojamu darbplūsmu** ievadiet nosaukumu \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="cc4a7-109">**Platformas tips**, noklikšķiniet uz **SharePoint 2010 darbplūsmā**, un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="cc4a7-110">**Darbplūsmas** lentes sadaļā **saglabāt** atlasiet **publicēt**.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="cc4a7-111">Sadaļā **pārvaldīt** **darbplūsmas** lentē atlasiet **publicēt globāli**.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="cc4a7-112">Apstiprinājuma parādītajā dialoglodziņā atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="cc4a7-113">Web pārlūkprogrammā atrodiet vietņu kolekcijas saknes vietni un pēc tam piekļūstiet **vietnes iestatījumu** \> **vietņu kolekcijas līdzekļiem**.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="cc4a7-114">Pārslēdziet līdzekli **darbplūsmas** :</span><span class="sxs-lookup"><span data-stu-id="cc4a7-114">Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="cc4a7-115">· Ja līdzeklis ir *aktivizēts* , noklikšķiniet uz **deaktivizēt** un pēc tam noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="cc4a7-116">· Ja līdzeklis ir *deaktivizēts* , noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="cc4a7-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="cc4a7-117">Lai iegūtu papildinformāciju, lūdzu, skatiet šo [rakstu](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="cc4a7-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

