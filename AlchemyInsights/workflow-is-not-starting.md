---
title: Darbplūsmu nevar sākt
ms.author: efrene
author: efrene
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
ms.openlocfilehash: efd17c302ae6d857207e87e94d74d3794e94a83a
ms.sourcegitcommit: 204be4a6ae03700b75eae6b09b4e9ab283089fbf
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/03/2019
ms.locfileid: "36171795"
---
# <a name="workflow-is-not-starting"></a><span data-ttu-id="9be73-102">Darbplūsmu nevar sākt</span><span class="sxs-lookup"><span data-stu-id="9be73-102">Workflow is not starting</span></span>

- <span data-ttu-id="9be73-103">SharePoint 2010 un SharePoint 2013 darbplūsmas nesākam.</span><span class="sxs-lookup"><span data-stu-id="9be73-103">SharePoint 2010 and SharePoint 2013 workflows are not starting.</span></span>

    <span data-ttu-id="9be73-104">Ja darbplūsmas nav sākusies, var būt pagaidu pakalpojumu jautājumu, kur lietotāji var rasties intermitējošs kavēšanos ar darbplūsmas norisi.</span><span class="sxs-lookup"><span data-stu-id="9be73-104">If your workflow is not starting, there may be a temporary service issue where users may experience intermittent delays with workflow progress.</span></span> <span data-ttu-id="9be73-105">Pārbaudiet [Pakalpojumu veselības Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) redzēt, ja jūsu organizācija ir ietekmētas.</span><span class="sxs-lookup"><span data-stu-id="9be73-105">Check the [Service Health Dashboard](https:/admin.microsoft.com/AdminPortal/Home#/servicehealth) to see if your organization is impacted.</span></span>

    <span data-ttu-id="9be73-106">Ja ilgāk par 24 stundām, ir pagājuši, kopš tu pirmo reizi redzēji šo jautājumu, lūdzu, piesakieties support ticket.</span><span class="sxs-lookup"><span data-stu-id="9be73-106">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="9be73-107">Daudzos gadījumos mēs jau strādājam pie risinājuma.</span><span class="sxs-lookup"><span data-stu-id="9be73-107">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="9be73-108">Lūdzu, sniedziet mums vismaz 24 stundas, lai pabeigtu risinājumu.</span><span class="sxs-lookup"><span data-stu-id="9be73-108">Please give us at least 24 hours to complete a solution.</span></span>

- <span data-ttu-id="9be73-109">SharePoint 2010 darbplūsmas atlikta uz start.</span><span class="sxs-lookup"><span data-stu-id="9be73-109">SharePoint 2010 workflows delayed on start.</span></span>

    <span data-ttu-id="9be73-110">Tas notiek tad, ja darbplūsma tiek nosūtīts lielām partijām.</span><span class="sxs-lookup"><span data-stu-id="9be73-110">This occurs if the workflow is triggered in large batches.</span></span> <span data-ttu-id="9be73-111">(piemēram, kad vairāki krājumi tiek pievienoti uzreiz).</span><span class="sxs-lookup"><span data-stu-id="9be73-111">(for example, when several items are added at once).</span></span>

    <span data-ttu-id="9be73-112">Darbplūsmas nav paredzēts darboties reālā laikā, tāpēc kavēšanās ir pēc konstrukcijas uzvedība.</span><span class="sxs-lookup"><span data-stu-id="9be73-112">Workflows are not designed to run real-time, so a delay is by-design behavior.</span></span>

    <span data-ttu-id="9be73-113">Ja darbplūsma ir komplekss paplašināmo objektu iezīmēšanas valodu (XMOL), apkopošanu var būt lēna.</span><span class="sxs-lookup"><span data-stu-id="9be73-113">If the Workflow is complex Extensible Object Markup Language (XMOL), compilation can be slow.</span></span> <span data-ttu-id="9be73-114">Pārbaudiet [šo](https://support.microsoft.com/en-us/kb/3043697) rakstu.</span><span class="sxs-lookup"><span data-stu-id="9be73-114">Check [this](https://support.microsoft.com/en-us/kb/3043697) article.</span></span>

    <span data-ttu-id="9be73-115">Būtu vienkāršot darbplūsmas vai pārstrādāt to, izmantojot Microsoft SharePoint 2013 darbplūsmas platformas tipa.</span><span class="sxs-lookup"><span data-stu-id="9be73-115">You should simplify the workflow or redesign it using the Microsoft SharePoint 2013 Workflow platform type.</span></span>

    <span data-ttu-id="9be73-116">Arī tad, ja darbplūsmas vēsture izaugusi liela, jūs varat Iztīrīt vienumus vai izveidot jaunu vēstures sarakstu.</span><span class="sxs-lookup"><span data-stu-id="9be73-116">Also, if your workflow history has grown large, you may want to purge the items or create a new history list.</span></span>

    <span data-ttu-id="9be73-117">Vairāk informācijas: [darbplūsmas vēstures iztīrīšana](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span><span class="sxs-lookup"><span data-stu-id="9be73-117">More Information : [Purge Workflow History](https://blogs.technet.microsoft.com/marj/2015/08/07/sharepoint-2010-workflows-best-practice-purge-workflow-history-list-items/)</span></span>


## <a name="related-topics"></a><span data-ttu-id="9be73-118">Saistītās tēmas</span><span class="sxs-lookup"><span data-stu-id="9be73-118">Related topics</span></span>
<span data-ttu-id="9be73-119">Vēlaties izmēģināt Micrsoft plūsmas SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="9be73-119">Want to try Micrsoft Flow in SharePoint Online?</span></span>
- [<span data-ttu-id="9be73-120">Radīt plūsmu</span><span class="sxs-lookup"><span data-stu-id="9be73-120">Create Flow</span></span>](https://support.office.com/article/Create-a-flow-for-a-list-or-library-in-SharePoint-Online-or-OneDrive-for-Business-a9c3e03b-0654-46af-a254-20252e580d01) 
- [<span data-ttu-id="9be73-121">SharePoint un plūsmas</span><span class="sxs-lookup"><span data-stu-id="9be73-121">SharePoint and Flow</span></span>](https://flow.microsoft.com/blog/sharepoint-and-flow/) 


