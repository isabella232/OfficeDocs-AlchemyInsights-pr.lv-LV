---
title: Trūkstošo darbplūsmu neizdevās aktivizēt
ms.author: pebaum
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: f03d7e1441465050c4b0608f4100f217b183d2e2
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36753803"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="d39ec-102">Trūkstošo darbplūsmu neizdevās aktivizēt</span><span class="sxs-lookup"><span data-stu-id="d39ec-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="d39ec-103">Microsoft SharePoint vietņu kolekcijas sarakstu vai bibliotēku nevar pievienot globāli atkārtoti darbplūsmas (piemēram, "apstiprinājums-SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="d39ec-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="d39ec-104">Lai novērstu šo problēmu, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="d39ec-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="d39ec-105">Atveriet vietņu kolekcijas saknes vietnē programmā SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="d39ec-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="d39ec-106">Sadaļā **vietnes objekti**atlasiet **darbplūsmas**.</span><span class="sxs-lookup"><span data-stu-id="d39ec-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="d39ec-107">**Jaunajā** sadaļā **darbplūsmas** lentē atlasiet **atkārtoti izmantojama darbplūsma**.</span><span class="sxs-lookup"><span data-stu-id="d39ec-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="d39ec-108">Veidlapā **izveidot atkārtoti izmantojamu darbplūsmu** ievadiet nosaukumu \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="d39ec-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="d39ec-109">**Platformas tips**, noklikšķiniet uz **SharePoint 2010 darbplūsmā**, un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="d39ec-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="d39ec-110">**Darbplūsmas** lentes sadaļā **saglabāt** atlasiet **publicēt**.</span><span class="sxs-lookup"><span data-stu-id="d39ec-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="d39ec-111">Sadaļā **pārvaldīt** **darbplūsmas** lentē atlasiet **publicēt globāli**.</span><span class="sxs-lookup"><span data-stu-id="d39ec-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="d39ec-112">Apstiprinājuma parādītajā dialoglodziņā atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="d39ec-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="d39ec-113">Web pārlūkprogrammā atrodiet vietņu kolekcijas saknes vietni un pēc tam piekļūstiet **vietnes iestatījumu** \> **vietņu kolekcijas līdzekļiem**.</span><span class="sxs-lookup"><span data-stu-id="d39ec-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="d39ec-114">Pēc tam pārslēdziet līdzekli **darbplūsmas** :</span><span class="sxs-lookup"><span data-stu-id="d39ec-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="d39ec-115">· Ja līdzeklis ir *aktivizēts* , noklikšķiniet uz **deaktivizēt** un pēc tam noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="d39ec-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="d39ec-116">· Ja līdzeklis ir *deaktivizēts* , noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="d39ec-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="d39ec-117">Lai iegūtu papildinformāciju, lūdzu, skatiet šo [rakstu](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="d39ec-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

