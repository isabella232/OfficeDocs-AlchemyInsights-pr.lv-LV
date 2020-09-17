---
title: Darbplūsma netiek sākta
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
ms.openlocfilehash: e3b8777ed74b812b31338784999eea43a95d3456
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47794774"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="5acf4-102">Darbplūsma netiek sākta</span><span class="sxs-lookup"><span data-stu-id="5acf4-102">Workflow is not starting</span></span>

- <span data-ttu-id="5acf4-103">SharePoint 2010 un SharePoint 2013 darbplūsmas netiek sāktas.</span><span class="sxs-lookup"><span data-stu-id="5acf4-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    - <span data-ttu-id="5acf4-104">Ja darbplūsma nestartējas, iespējams, pastāv pagaidu pakalpojumu problēma, kur lietotāji var rasties neregulāras aizkaves ar darbplūsmas norisi.</span><span class="sxs-lookup"><span data-stu-id="5acf4-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="5acf4-105">Pārbaudiet [Pakalpojuma darbspējas informācijas paneli](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) , lai noskaidrotu, vai jūsu organizācija ir ietekmēta.</span><span class="sxs-lookup"><span data-stu-id="5acf4-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    - <span data-ttu-id="5acf4-106">Ja kopš pirmoreiz redzējāt šo problēmu, ir pagājušas vairāk nekā 24 stundas, lūdzu, piesakieties atbalsta biļetē.</span><span class="sxs-lookup"><span data-stu-id="5acf4-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="5acf4-107">Daudzos gadījumos mēs jau strādājam pie risinājuma.</span><span class="sxs-lookup"><span data-stu-id="5acf4-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="5acf4-108">Lai pabeigtu risinājumu, lūdzu, sniedziet mums vismaz 24 stundas.</span><span class="sxs-lookup"><span data-stu-id="5acf4-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="5acf4-109">SharePoint 2010 darbplūsmas kavējas sākuma ekrānā.</span><span class="sxs-lookup"><span data-stu-id="5acf4-109">SharePoint 2010 workflows delayed on start.</span></span>

    - <span data-ttu-id="5acf4-110">Tas notiek tad, ja darbplūsma ir aktivizēta lielās paketēs.</span><span class="sxs-lookup"><span data-stu-id="5acf4-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="5acf4-111">(piemēram, ja vienlaikus tiek pievienoti vairāki vienumi).</span><span class="sxs-lookup"><span data-stu-id="5acf4-111">(for example, when several items are added at once).</span></span>

    - <span data-ttu-id="5acf4-112">Darbplūsmas nav paredzētas darbībai reālajā laikā, tāpēc atlikšanai ir jānotiek ar noformēšanas darbību.</span><span class="sxs-lookup"><span data-stu-id="5acf4-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

   -  <span data-ttu-id="5acf4-113">Ja darbplūsma ir sarežģīta eXtensible Object Markup Language (XMOL), kompilēšana var būt lēna.</span><span class="sxs-lookup"><span data-stu-id="5acf4-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="5acf4-114">Atzīmējiet [šo](https://support.microsoft.com//kb/3043697) rakstu.</span><span class="sxs-lookup"><span data-stu-id="5acf4-114">Check [this](https://support.microsoft.com//kb/3043697) article.</span></span>

    - <span data-ttu-id="5acf4-115">Jums ir jāvienkāršo darbplūsma vai jāpārveido tā, izmantojot Microsoft SharePoint 2013 darbplūsmas platformas tipu.</span><span class="sxs-lookup"><span data-stu-id="5acf4-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    - <span data-ttu-id="5acf4-116">Ja jūsu darbplūsmas vēsture ir kļuvusi liela, iespējams, vēlēsities iztīrīt vienumus vai izveidot jaunu vēstures sarakstu.</span><span class="sxs-lookup"><span data-stu-id="5acf4-116">If your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

        <span data-ttu-id="5acf4-117">Papildinformācija: [Dzēst darbplūsmas vēsturi](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="5acf4-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="5acf4-118">Saistītās tēmas</span><span class="sxs-lookup"><span data-stu-id="5acf4-118">Related topics</span></span>
<span data-ttu-id="5acf4-119">Vai vēlaties izmēģināt Microsoft plūsmu pakalpojumā SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="5acf4-119">Want to try Microsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="5acf4-120">Izveidot plūsmu</span><span class="sxs-lookup"><span data-stu-id="5acf4-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="5acf4-121">SharePoint un plūsma</span><span class="sxs-lookup"><span data-stu-id="5acf4-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


