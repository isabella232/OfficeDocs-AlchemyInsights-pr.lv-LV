---
title: Nevar pievienot 2010 apstiprinājuma darbplūsmu
ms.author: kirks
author: Techwriter40
ms.date: 12/3/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 0df65cf9-7eae-4de7-88e9-1914635c8d11
ms.openlocfilehash: a83a9621ca0f7764d3f2c0a698dbffd80d55e80c
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28301058"
---
# <a name="unable-to-add-2010-approval-workflow"></a><span data-ttu-id="36e66-102">Nevar pievienot 2010 apstiprinājuma darbplūsmu</span><span class="sxs-lookup"><span data-stu-id="36e66-102">Unable to add 2010 Approval Workflow</span></span>

<span data-ttu-id="36e66-103">Microsoft SharePoint vietņu kolekcijas sarakstam vai bibliotēkai nevar pievienot globāli atkārtoti darbplūsmai (piemēram, "apstiprināšana - SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="36e66-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="36e66-104">Lai atrisinātu šo problēmu, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="36e66-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="36e66-105">Saknes tīmekļa vietņu kolekcijas atvēršana SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="36e66-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="36e66-106">Zem **Vietnes objektus**, atlasiet **darbplūsmas**.</span><span class="sxs-lookup"><span data-stu-id="36e66-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="36e66-107">**Jaunā** sadaļā **darbplūsmas** lentes, atlasiet **Izmantojama darbplūsmas**.</span><span class="sxs-lookup"><span data-stu-id="36e66-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="36e66-p101">Formā **Izveidot izmantojama darbplūsmas** ievadiet nosaukumu \* \* *Repair2010* \* \*. **Platformas tips**noklikšķiniet uz **SharePoint 2010 darbplūsma**un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="36e66-p101">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*. For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="36e66-110">Sadaļā **Saglabāt** **darbplūsmas** lentes, atlasiet **publicēt**.</span><span class="sxs-lookup"><span data-stu-id="36e66-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="36e66-p102">**Darbplūsmā** lentei sadaļā **Pārvaldīt** atlasiet **Publicēt globāli**. Apstiprinājuma dialoglodziņā, kas parādās, izvēlieties **Labi**.</span><span class="sxs-lookup"><span data-stu-id="36e66-p102">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**. In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="36e66-p103">Web pārlūkprogrammā, atrast saknes tīmekļa vietņu kolekcijas, un pēc tam piekļūt **Vietnes iestatījumus** \> **Vietņu kolekcijas līdzekļus**. Pārslēgt **darbplūsmas** līdzeklis:</span><span class="sxs-lookup"><span data-stu-id="36e66-p103">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**. Toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="36e66-115">· Ja līdzeklis tiek *aktivizēts* , noklikšķiniet uz **deaktivizēt,** un pēc tam noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="36e66-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="36e66-116">· Ja līdzeklis ir *Deactivated* , noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="36e66-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="36e66-117">Plašāku informāciju skatiet šādu [pantu](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="36e66-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

