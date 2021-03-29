---
title: Darbplūsma netiek startēta
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: e69f3e529e4a2202f641cb62f42b1a20d774a398
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403750"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="46325-102">Darbplūsma netiek startēta</span><span class="sxs-lookup"><span data-stu-id="46325-102">Workflow is not starting</span></span>

- <span data-ttu-id="46325-103">SharePoint 2010 un SharePoint 2013 darbplūsmas netiek startētas.</span><span class="sxs-lookup"><span data-stu-id="46325-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="46325-104">Ja darbplūsma netiek startēta, var rasties īslaicīga pakalpojuma problēma, kur lietotājiem var rasties neregulāras darbplūsmas norises aizkaves.</span><span class="sxs-lookup"><span data-stu-id="46325-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="46325-105">Pārbaudiet pakalpojuma [darbspējas informācijas paneli,](https://admin.microsoft.com/AdminPortal/Home/servicehealth) lai uzzinātu, vai jūsu organizācija tiek ietekmēta.</span><span class="sxs-lookup"><span data-stu-id="46325-105">Check the [Service Health Dashboard](https://admin.microsoft.com/AdminPortal/Home/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="46325-106">Ja kopš šīs problēmas pirmās izsakumēšanas ir pagājusi vairāk nekā 24 stundas, lūdzu, reģistrējiet atbalsta biļeti.</span><span class="sxs-lookup"><span data-stu-id="46325-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="46325-107">Daudzos gadījumos mēs jau strādājam, lai rastu risinājumu.</span><span class="sxs-lookup"><span data-stu-id="46325-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="46325-108">Lūdzu, sniedziet vismaz 24 stundas, lai pabeigtu risinājumu.</span><span class="sxs-lookup"><span data-stu-id="46325-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="46325-109">SharePoint 2010 darbplūsmas tiek aizkavētas sākumā.</span><span class="sxs-lookup"><span data-stu-id="46325-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="46325-110">Tas notiek, ja darbplūsma tiek izraisīta lielās paketēs.</span><span class="sxs-lookup"><span data-stu-id="46325-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="46325-111">(piemēram, ja vienlaikus tiek pievienoti vairāki vienumi).</span><span class="sxs-lookup"><span data-stu-id="46325-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="46325-112">Darbplūsmas nav paredzētas, lai darbinātu reāllaikā, tāpēc aizkave ir aizkave, kas darbojas pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="46325-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="46325-113">Ja darbplūsma ir sarežģīta paplašināmā objektu iezīmēšanas valoda (XMOL), kompilēšana var būt lēna.</span><span class="sxs-lookup"><span data-stu-id="46325-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="46325-114">Skatiet [šo](https://support.microsoft.com//kb/3043697) rakstu.</span><span class="sxs-lookup"><span data-stu-id="46325-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="46325-115">Jums vajadzētu vienkāršot darbplūsmu vai to pārveidot, izmantojot Microsoft SharePoint 2013 darbplūsmas platformas tipu.</span><span class="sxs-lookup"><span data-stu-id="46325-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="46325-116">Ja jūsu darbplūsmas vēsture ir pieaugusi, iespējams, vēlēsities iztīrīt vienumus vai izveidot jaunu vēstures sarakstu.</span><span class="sxs-lookup"><span data-stu-id="46325-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="46325-117">Papildinformācija: [iztīriet darbplūsmas vēsturi](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="46325-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="46325-118">Saistītās tēmas</span><span class="sxs-lookup"><span data-stu-id="46325-118">Related topics</span></span>
<span data-ttu-id="46325-119">Vai vēlaties izmēģināt Microsoft Flow koplietošanas vidē SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="46325-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="46325-120">Create Flow</span><span class="sxs-lookup"><span data-stu-id="46325-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="46325-121">SharePoint un Flow</span><span class="sxs-lookup"><span data-stu-id="46325-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 
