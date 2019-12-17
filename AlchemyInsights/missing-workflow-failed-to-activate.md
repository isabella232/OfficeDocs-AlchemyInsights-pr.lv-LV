---
title: Trūkstošo darbplūsmu neizdevās aktivizēt
ms.author: pebaum
author: pebaum
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 3df1ddc1059c4cd6cc3f9f42dc157d20be79a63a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40052620"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="9c550-102">Trūkstošo darbplūsmu neizdevās aktivizēt</span><span class="sxs-lookup"><span data-stu-id="9c550-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="9c550-103">Microsoft SharePoint vietņu kolekcijas sarakstu vai bibliotēku nevar pievienot globāli atkārtoti darbplūsmas (piemēram, "apstiprinājums-SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="9c550-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="9c550-104">Lai novērstu šo problēmu, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="9c550-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="9c550-105">Atveriet vietņu kolekcijas saknes vietnē programmā SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="9c550-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="9c550-106">Sadaļā **vietnes objekti**atlasiet **darbplūsmas**.</span><span class="sxs-lookup"><span data-stu-id="9c550-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="9c550-107">**Jaunajā** sadaļā **darbplūsmas** lentē atlasiet **atkārtoti izmantojama darbplūsma**.</span><span class="sxs-lookup"><span data-stu-id="9c550-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="9c550-108">Veidlapā **izveidot atkārtoti izmantojamu darbplūsmu** ievadiet nosaukumu \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="9c550-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="9c550-109">**Platformas tips**, noklikšķiniet uz **SharePoint 2010 darbplūsmā**, un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="9c550-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="9c550-110">**Darbplūsmas** lentes sadaļā **saglabāt** atlasiet **publicēt**.</span><span class="sxs-lookup"><span data-stu-id="9c550-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="9c550-111">Sadaļā **pārvaldīt** **darbplūsmas** lentē atlasiet **publicēt globāli**.</span><span class="sxs-lookup"><span data-stu-id="9c550-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="9c550-112">Apstiprinājuma parādītajā dialoglodziņā atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="9c550-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="9c550-113">Web pārlūkprogrammā atrodiet vietņu kolekcijas saknes vietni un pēc tam piekļūstiet **vietnes iestatījumu** \> **vietņu kolekcijas līdzekļiem**.</span><span class="sxs-lookup"><span data-stu-id="9c550-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="9c550-114">Pēc tam pārslēdziet līdzekli **darbplūsmas** :</span><span class="sxs-lookup"><span data-stu-id="9c550-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="9c550-115">· Ja līdzeklis ir *aktivizēts* , noklikšķiniet uz **deaktivizēt** un pēc tam noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="9c550-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="9c550-116">· Ja līdzeklis ir *deaktivizēts* , noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="9c550-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="9c550-117">Lai iegūtu papildinformāciju, lūdzu, skatiet šo [rakstu](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="9c550-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

