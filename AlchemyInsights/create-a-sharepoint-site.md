---
title: Izveidotu SharePoint vietni
ms.author: kirks
author: Techwriter40
ms.date: 1/16/2019
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1386"
- "2303"
- "5200004"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 022f572aadae3b4d9f6665f9f8be871d79b51817
ms.sourcegitcommit: f81c56dd4ae7cb2eedc383dd671b9012f3089286
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/19/2019
ms.locfileid: "35802973"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="98c1e-102">Izveidotu SharePoint vietni</span><span class="sxs-lookup"><span data-stu-id="98c1e-102">Create a SharePoint site</span></span>

<span data-ttu-id="98c1e-103">Var apskatīt šādu informāciju par SharePoint vietņu izveides:</span><span class="sxs-lookup"><span data-stu-id="98c1e-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="98c1e-104">[Pārvaldīt vietnes jauno SharePoint administrēšanas centrā](https://docs.microsoft.com/sharepoint/manage-site-creation): uzzināt par vietnes izveides iespējas, tostarp kā klasisks vietā vai brigāžu vietā, kas nav iekļauta Office 365 grupu veidošanai.</span><span class="sxs-lookup"><span data-stu-id="98c1e-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="98c1e-105">[Izveidot darba grupas vietni koplietošanas vides SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Uzziniet, kā izveidot komandas Web vietu.</span><span class="sxs-lookup"><span data-stu-id="98c1e-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d?ui=en-US&amp;rs=en-US&amp;ad=US): Learn how to create a team site.</span></span>
- <span data-ttu-id="98c1e-106">[Izveidot komunikācijas vietni, SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Uzziniet, kā izveidot sakaru vietā.</span><span class="sxs-lookup"><span data-stu-id="98c1e-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="98c1e-107">[Pārvaldīt vietnes jauno SharePoint administrēšanas centrā](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Uzziniet, kā izveidot klasiskās vietas vai komandu vietā, kas nav iekļauta Office 365 grupa.</span><span class="sxs-lookup"><span data-stu-id="98c1e-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
> [! Padomi]
> - <span data-ttu-id="98c1e-109">Nevar izveidot vietni ar tādu pašu URL esošās vietas.</span><span class="sxs-lookup"><span data-stu-id="98c1e-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="98c1e-110">Ja izdzēsāt vietā un vēlas atkārtoti izmantot URL, ir iespējams dzēst vietņu joprojām pastāv saskaņā ar **izdzēsto vietām**.</span><span class="sxs-lookup"><span data-stu-id="98c1e-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="98c1e-111">Lai pārvaldītu dzēsti vietās skat. [izdzēst vietni](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="98c1e-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="98c1e-112">Pilnīgi noņemt vietni, izmantojot Powershell, skatiet [Remove SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet piemēru.</span><span class="sxs-lookup"><span data-stu-id="98c1e-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
> - <span data-ttu-id="98c1e-113">Daži lietotāji, iespējams, nevarēs izveidot vietni.</span><span class="sxs-lookup"><span data-stu-id="98c1e-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="98c1e-114">Skatiet [Manage vietņu izveide SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="98c1e-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
> - <span data-ttu-id="98c1e-115">Tas ir iespējams, šāda vietne tiek parādīta iestrēdzis pie **Creating** ilgāk, nekā gaidīts.</span><span class="sxs-lookup"><span data-stu-id="98c1e-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="98c1e-116">Ja ilgāk par 24 stundām, ir pagājuši, kopš tu pirmo reizi redzēji šo jautājumu, lūdzu, piesakieties support ticket.</span><span class="sxs-lookup"><span data-stu-id="98c1e-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="98c1e-117">Daudzos gadījumos mēs jau strādājam pie risinājuma.</span><span class="sxs-lookup"><span data-stu-id="98c1e-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="98c1e-118">Lūdzu, sniedziet mums vismaz 24 stundas, lai pabeigtu risinājumu.</span><span class="sxs-lookup"><span data-stu-id="98c1e-118">Please give us at least 24 hours to complete a solution.</span></span>
> - <span data-ttu-id="98c1e-119">Ja nepieciešams izveidot jaunu darba grupas vietni, kurš nav iekļauts Office 365 grupu,</span><span class="sxs-lookup"><span data-stu-id="98c1e-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


