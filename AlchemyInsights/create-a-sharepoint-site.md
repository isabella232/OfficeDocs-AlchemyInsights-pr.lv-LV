---
title: Izveidot SharePoint vietni
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 2611c3ed9cfe78c82c9b123ea26b6fe8f951b458
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40049884"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="7c7a0-102">Izveidot SharePoint vietni</span><span class="sxs-lookup"><span data-stu-id="7c7a0-102">Create a SharePoint site</span></span>

<span data-ttu-id="7c7a0-103">Informāciju par SharePoint vietnes izveidi var skatīt šādi:</span><span class="sxs-lookup"><span data-stu-id="7c7a0-103">You can see the following for information about SharePoint site creation:</span></span>
- <span data-ttu-id="7c7a0-104">[Vietņu pārvaldīšana jaunajā SharePoint administrēšanas centrā](https://docs.microsoft.com/sharepoint/manage-site-creation): Uzziniet par vietnes izveides opcijām, tostarp par to, kā izveidot klasisko vietni vai darba grupu vietni, kurā nav iekļauta Office 365 grupa.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-104">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation): Learn about site creation options, including how to create a classic site or a teams site that doesn't include an Office 365 group.</span></span>
- <span data-ttu-id="7c7a0-105">[Izveidot darba grupas vietni SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Uzziniet, kā izveidot grupas vietni.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-105">[Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d): Learn how to create a team site.</span></span>
- <span data-ttu-id="7c7a0-106">[Izveidot saziņas vietnes SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Uzziniet, kā izveidot saziņas vietnes.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-106">[Create a communication site in SharePoint Online](https://support.office.com/article/7fb44b20-a72f-4d2c-9173-fc8f59ba50eb): Learn how to create a communications site.</span></span>
- <span data-ttu-id="7c7a0-107">[Vietņu pārvaldīšana jaunajā SharePoint administrēšanas centrā](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site): Uzziniet, kā izveidot klasisko vietni vai grupas vietni, kurā nav iekļauta Office 365 grupa.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-107">[Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#create-a-site):  Learn how to create a classic site or a team site that doesn't include an Office 365 group.</span></span>


  
<span data-ttu-id="7c7a0-108">**Padomi:**</span><span class="sxs-lookup"><span data-stu-id="7c7a0-108">**Tips:**</span></span>
- <span data-ttu-id="7c7a0-109">Nevar izveidot vietni ar tādu pašu esošas vietnes vietrādi URL.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-109">You cannot create a site with the same URL of an existing site.</span></span> <span data-ttu-id="7c7a0-110">Ja jūs svītrots vietu un vēlas atkārtoti izmantot URL, tas ir iespējams svītrots vietā joprojām pastāv saskaņā **svītrots vietās**.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-110">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under **Deleted sites**.</span></span> <span data-ttu-id="7c7a0-111">Lai pārvaldītu izdzēstās vietnes skatiet, [dzēsiet vietni](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="7c7a0-111">To manage deleted sites see, [Delete a Site](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site).</span></span> <span data-ttu-id="7c7a0-112">Lai pilnībā noņemtu vietni ar PowerShell, skatiet [Noņemt SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet piemērs.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-112">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="7c7a0-113">Daži lietotāji, iespējams, nevarēs izveidot vietni.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-113">Some users may not be able to create a site.</span></span> <span data-ttu-id="7c7a0-114">Skatiet [pārvaldīt vietnes izveide SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="7c7a0-114">See [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="7c7a0-115">Tas ir iespējams, vietā, šķiet iestrēdzis **radīt** ilgāk, nekā gaidīts.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-115">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="7c7a0-116">Ja kopš pirmās šīs problēmas instalēšanas ir pagājušas vairāk nekā 24 stundas, lūdzu, piesakieties atbalsta biļetei.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-116">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="7c7a0-117">Daudzos gadījumos mēs jau strādājam pie risinājuma.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-117">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="7c7a0-118">Lūdzu, sniedziet mums vismaz 24 stundas, lai pabeigtu risinājumu.</span><span class="sxs-lookup"><span data-stu-id="7c7a0-118">Please give us at least 24 hours to complete a solution.</span></span>
- <span data-ttu-id="7c7a0-119">Ja nepieciešams izveidot jaunu darba grupas vietni, kurā nav iekļauta Office 365 grupa,</span><span class="sxs-lookup"><span data-stu-id="7c7a0-119">If you need to create a new team site that doesn't include an Office 365 group,</span></span> 


