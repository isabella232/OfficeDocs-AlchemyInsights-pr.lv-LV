---
title: Izveidot SharePoint vietni
ms.author: pebaum
author: todmccoy
ms.audience: Admin
ms.topic: article
ms.collection: Adm_O365
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: e1e71ae9401448ed18058f6307302dcbaf773649
ms.sourcegitcommit: 317eeed39c7777a922442992d67733726c41d9e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/04/2020
ms.locfileid: "41770862"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="11f9c-102">Izveidot SharePoint vietni</span><span class="sxs-lookup"><span data-stu-id="11f9c-102">Create a SharePoint site</span></span>

<span data-ttu-id="11f9c-103">Izveidot vai pārvaldīt vietnes no [aktīvās vietnes](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) SharePoint administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="11f9c-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="11f9c-104">Papildinformāciju skatiet sadaļā [vietņu pārvaldīšana jaunajā SharePoint administrēšanas centrā](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="11f9c-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="11f9c-105">Padomi:</span><span class="sxs-lookup"><span data-stu-id="11f9c-105">Tips:</span></span>

- <span data-ttu-id="11f9c-106">**Nevar** izveidot vietni ar tādu pašu esošas vietnes vietrādi URL.</span><span class="sxs-lookup"><span data-stu-id="11f9c-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="11f9c-107">Ja jūs svītrots vietu un vēlas atkārtoti izmantot URL, tas ir iespējams svītrots vietā joprojām pastāv saskaņā [svītrots vietās](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span><span class="sxs-lookup"><span data-stu-id="11f9c-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="11f9c-108">Vietne būs neatgriezeniski jādzēš, lai atkārtoti izmantotu vietrādi URL.</span><span class="sxs-lookup"><span data-stu-id="11f9c-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="11f9c-109">Lai pilnībā noņemtu vietni ar PowerShell, skatiet [Noņemt SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet piemērs.</span><span class="sxs-lookup"><span data-stu-id="11f9c-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="11f9c-110">Daži lietotāji, iespējams, nevarēs izveidot vietni.</span><span class="sxs-lookup"><span data-stu-id="11f9c-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="11f9c-111">[Skatiet pārvaldīt vietnes izveide SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="11f9c-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="11f9c-112">Tas ir iespējams, vietā, šķiet iestrēdzis **radīt** ilgāk, nekā gaidīts.</span><span class="sxs-lookup"><span data-stu-id="11f9c-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="11f9c-113">Ja kopš pirmās šīs problēmas instalēšanas ir pagājušas vairāk nekā 24 stundas, lūdzu, piesakieties atbalsta biļetei.</span><span class="sxs-lookup"><span data-stu-id="11f9c-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="11f9c-114">Daudzos gadījumos mēs jau strādājam pie risinājuma.</span><span class="sxs-lookup"><span data-stu-id="11f9c-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="11f9c-115">Lūdzu, sniedziet mums vismaz 24 stundas, lai pabeigtu risinājumu.</span><span class="sxs-lookup"><span data-stu-id="11f9c-115">Please give us at least 24 hours to complete a solution.</span></span>
