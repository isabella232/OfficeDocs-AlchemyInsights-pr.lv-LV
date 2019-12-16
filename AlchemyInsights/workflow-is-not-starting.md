---
title: Darbplūsma netiek sākta
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.date: 8/2/2019
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000144"
- "1670"
ms.openlocfilehash: cf7bd95e9a8f1d0842f0abcf82c758d649e80c0f
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049344"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="61736-102">Darbplūsma netiek sākta</span><span class="sxs-lookup"><span data-stu-id="61736-102">Workflow is not starting</span></span>

- <span data-ttu-id="61736-103">SharePoint 2010 un SharePoint 2013 darbplūsmas nav sākuma.</span><span class="sxs-lookup"><span data-stu-id="61736-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="61736-104">Ja darbplūsma netiek sākta, iespējams, pastāv pagaidu pakalpojuma problēma, kuras dēļ lietotāji var saskarties ar neregulāru kavēšanos ar darbplūsmas norisi.</span><span class="sxs-lookup"><span data-stu-id="61736-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="61736-105">Pārbaudiet [pakalpojuma darbspējas informācijas paneli](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , lai noskaidrotu, vai jūsu organizācija ir ietekmēta.</span><span class="sxs-lookup"><span data-stu-id="61736-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="61736-106">Ja kopš pirmās šīs problēmas instalēšanas ir pagājušas vairāk nekā 24 stundas, lūdzu, piesakieties atbalsta biļetei.</span><span class="sxs-lookup"><span data-stu-id="61736-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="61736-107">Daudzos gadījumos mēs jau strādājam pie risinājuma.</span><span class="sxs-lookup"><span data-stu-id="61736-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="61736-108">Lūdzu, sniedziet mums vismaz 24 stundas, lai pabeigtu risinājumu.</span><span class="sxs-lookup"><span data-stu-id="61736-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="61736-109">SharePoint 2010 darbplūsmas kavējas sākuma.</span><span class="sxs-lookup"><span data-stu-id="61736-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="61736-110">Tā notiek, ja darbplūsma tiek aktivizēta lielās partijās.</span><span class="sxs-lookup"><span data-stu-id="61736-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="61736-111">(piemēram, vienlaicīgi pievienojot vairākus elementus).</span><span class="sxs-lookup"><span data-stu-id="61736-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="61736-112">Darbplūsmas nav paredzētas reāllaika palaišanai, tāpēc aizkavēšanās ir pēc noformējuma.</span><span class="sxs-lookup"><span data-stu-id="61736-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="61736-113">Ja darbplūsma ir sarežģīta paplašināmās objektu iezīmēšanas valoda (XMOL), kompilēšana var būt lēna.</span><span class="sxs-lookup"><span data-stu-id="61736-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="61736-114">Pārbaudiet [šo](https://support.microsoft.com//kb/3043697) rakstu.</span><span class="sxs-lookup"><span data-stu-id="61736-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="61736-115">Jums vajadzētu vienkāršot darbplūsmu vai pārprojektējot to, izmantojot Microsoft SharePoint 2013 darbplūsmas platformas tips.</span><span class="sxs-lookup"><span data-stu-id="61736-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="61736-116">Ja darbplūsmas vēsture ir pieaugusi, iespējams, vēlēsities iztīrīt vienumus vai izveidot jaunu vēstures sarakstu.</span><span class="sxs-lookup"><span data-stu-id="61736-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="61736-117">Papildinformācija: [darbplūsmu vēstures iztīrīšanas](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="61736-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="61736-118">Saistītās tēmas</span><span class="sxs-lookup"><span data-stu-id="61736-118">Related topics</span></span>
<span data-ttu-id="61736-119">Vai vēlaties izmēģināt Microsoft Flow pakalpojumā SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="61736-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="61736-120">Izveidot plūsmu</span><span class="sxs-lookup"><span data-stu-id="61736-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="61736-121">SharePoint un plūsmas</span><span class="sxs-lookup"><span data-stu-id="61736-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


