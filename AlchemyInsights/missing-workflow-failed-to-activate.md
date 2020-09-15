---
title: Trūkst darbplūsmas neizdevās aktivizēt
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: e46ae8c5-3d81-457e-8c77-f7c1cbe267c4
ms.openlocfilehash: 604dc770c5c14ded6a8de1cec9e311b03b69f094
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47667093"
---
# <a name="missing-workflow-failed-to-activate"></a><span data-ttu-id="9f005-102">Trūkst darbplūsmas neizdevās aktivizēt</span><span class="sxs-lookup"><span data-stu-id="9f005-102">Missing Workflow Failed to Activate</span></span>

<span data-ttu-id="9f005-103">Microsoft SharePoint vietņu kolekcijā sarakstam vai bibliotēkai nevar pievienot globāli atkārtoti izmantojamas darbplūsmas (piemēram, "apstiprinājums-SharePoint 2010").</span><span class="sxs-lookup"><span data-stu-id="9f005-103">In a Microsoft SharePoint site collection, you can't add a globally reusable workflow (such as "Approval - SharePoint 2010") to a list or library.</span></span>
  
<span data-ttu-id="9f005-104">Lai atrisinātu šo problēmu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="9f005-104">To resolve this issue, follow these steps:</span></span> 
  
1. <span data-ttu-id="9f005-105">Atveriet vietņu kolekcijas saknes tīmekļa vietni programmā SharePoint Designer 2013.</span><span class="sxs-lookup"><span data-stu-id="9f005-105">Open the root website of the site collection in SharePoint Designer 2013.</span></span>
  
2. <span data-ttu-id="9f005-106">Sadaļā **vietnes objekti**atlasiet **darbplūsmas**.</span><span class="sxs-lookup"><span data-stu-id="9f005-106">Under **Site Objects**, select **Workflows**.</span></span> 
  
3. <span data-ttu-id="9f005-107">Sadaļā **jauna** **darbplūsmas** lente atlasiet **atkārtoti izmantojama darbplūsma**.</span><span class="sxs-lookup"><span data-stu-id="9f005-107">In the **New** section of the **Workflows** ribbon, select **Reusable Workflow**.</span></span> 
  
4. <span data-ttu-id="9f005-108">Veidlapā atkārtoti **izmantojamas darbplūsmas izveide** ievadiet nosaukumu \* \* *Repair2010* \* \*.</span><span class="sxs-lookup"><span data-stu-id="9f005-108">On the **Create Reusable Workflow** form, enter the name \*\* *Repair2010* \*\*.</span></span> <span data-ttu-id="9f005-109">**Platformas tipam**noklikšķiniet uz **SharePoint 2010 darbplūsma**un pēc tam noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="9f005-109">For **Platform Type**, click **SharePoint 2010 Workflow**, and then click **OK**.</span></span> 
  
1. <span data-ttu-id="9f005-110">**Darbplūsmas** lentes sadaļā **Saglabāt** atlasiet **publicēt**.</span><span class="sxs-lookup"><span data-stu-id="9f005-110">In the **Save** section of the **Workflow** ribbon, select **Publish**.</span></span> 
  
2. <span data-ttu-id="9f005-111">**Darbplūsmas** lentes sadaļā **pārvaldība** atlasiet **publicēt globāli**.</span><span class="sxs-lookup"><span data-stu-id="9f005-111">In the **Manage** section of the **Workflow** ribbon, select **Publish Globally**.</span></span> <span data-ttu-id="9f005-112">Apstiprinājuma dialoglodziņā, kas tiek parādīts, atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="9f005-112">In the confirmation dialog box that appears, select **OK**.</span></span> 
  
3. <span data-ttu-id="9f005-113">Tīmekļa pārlūkprogrammā atrodiet vietņu kolekcijas saknes tīmekļa vietni un pēc tam piekļūstiet **vietnes iestatījumu** \> **vietņu kolekcijas līdzekļiem**.</span><span class="sxs-lookup"><span data-stu-id="9f005-113">In a web browser, locate the root website of the site collection, and then access **Site Settings** \> **Site Collection Features**.</span></span> <span data-ttu-id="9f005-114">Pēc tam pārslēdziet **darbplūsmas** līdzekli:</span><span class="sxs-lookup"><span data-stu-id="9f005-114">Then, toggle the **Workflows** feature:</span></span> 
  
<span data-ttu-id="9f005-115">· Ja līdzeklis ir  *aktivizēts*  , noklikšķiniet uz **deaktivizēt** un pēc tam uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="9f005-115">· If the feature is  *Activated*  , click **Deactivate,** and then click **Activate**.</span></span> 
  
<span data-ttu-id="9f005-116">· Ja līdzeklis ir  *deaktivizēts*  , noklikšķiniet uz **Aktivizēt**.</span><span class="sxs-lookup"><span data-stu-id="9f005-116">· If the feature is  *Deactivated*  , click **Activate**.</span></span> 
  
<span data-ttu-id="9f005-117">Lai iegūtu papildinformāciju, lūdzu, skatiet šo [rakstu](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span><span class="sxs-lookup"><span data-stu-id="9f005-117">For more information please refer to the following [article](https://go.microsoft.com/fwlink/?linkid=2047770&amp;clcid=0x409).</span></span>
  

