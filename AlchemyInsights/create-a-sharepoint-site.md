---
title: SharePoint vietnes izveide
ms.author: pebaum
author: pebaum
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ms.collection: Adm_O365
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "5200004"
- "3911416"
- "1386"
- "2303"
ms.assetid: e62b9f80-b017-42dc-9464-f4e32c19d6c9
ms.openlocfilehash: 5ebaa342ca9864bc31a9ef26eebcf42d96523871
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806946"
---
# <a name="create-a-sharepoint-site"></a><span data-ttu-id="be591-102">SharePoint vietnes izveide</span><span class="sxs-lookup"><span data-stu-id="be591-102">Create a SharePoint site</span></span>

<span data-ttu-id="be591-103">Izveidot vai pārvaldīt vietnes no SharePoint administrēšanas centra [aktīvajām vietnēm](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) .</span><span class="sxs-lookup"><span data-stu-id="be591-103">Create or manage sites from [Active Sites](https://admin.microsoft.com/sharepoint?page=sitemanagement&modern=true) in the SharePoint Admin Center.</span></span> <span data-ttu-id="be591-104">Papildinformāciju skatiet rakstā [vietņu pārvaldība jaunajā SharePoint administrēšanas centrā](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="be591-104">For more info, see [Manage sites in the new SharePoint admin center](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span> 

## <a name="tips"></a><span data-ttu-id="be591-105">Padomi</span><span class="sxs-lookup"><span data-stu-id="be591-105">Tips:</span></span>

- <span data-ttu-id="be591-106">**Nevar** izveidot vietni ar vienu un to pašu savas esošas vietnes vietrādi URL.</span><span class="sxs-lookup"><span data-stu-id="be591-106">You **cannot** create a site with the same URL of an existing site.</span></span> <span data-ttu-id="be591-107">Ja izdzēšat vietni un vēlaties atkārtoti izmantot vietrādi URL, iespējams, izdzēstās [vietnes](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true)joprojām pastāv.</span><span class="sxs-lookup"><span data-stu-id="be591-107">If you deleted a site and are wishing to re-use the URL, it's possible the deleted site still exists under [Deleted sites](https://admin.microsoft.com/sharepoint?page=recyclebin&modern=true).</span></span> <span data-ttu-id="be591-108">Lai atkārtoti izmantotu vietrādi URL, vietne ir jādzēš neatgriezeniski.</span><span class="sxs-lookup"><span data-stu-id="be591-108">The site will need to be permanently deleted to re-use the URL.</span></span> <span data-ttu-id="be591-109">Lai pilnībā noņemtu vietni, izmantojot PowerShell, skatiet sadaļu [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet piemērs.</span><span class="sxs-lookup"><span data-stu-id="be591-109">To completely remove a site with Powershell, see the [Remove-SPSite](https://docs.microsoft.com/sharepoint/manage-sites-in-new-admin-center#delete-a-site) cmdlet example.</span></span>
- <span data-ttu-id="be591-110">Daži lietotāji, iespējams, nevarēs izveidot vietni.</span><span class="sxs-lookup"><span data-stu-id="be591-110">Some users may not be able to create a site.</span></span> <span data-ttu-id="be591-111">[Skatiet rakstu vietņu izveides pārvaldība pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span><span class="sxs-lookup"><span data-stu-id="be591-111">[See Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation).</span></span>
- <span data-ttu-id="be591-112">Iespējams, vietne ir iestrēgusi pie **izveidot** ilgāku laiku, nekā paredzēts.</span><span class="sxs-lookup"><span data-stu-id="be591-112">It's possible the site appears stuck at **Creating** longer than expected.</span></span> <span data-ttu-id="be591-113">Ja kopš pirmoreiz redzējāt šo problēmu, ir pagājušas vairāk nekā 24 stundas, lūdzu, piesakieties atbalsta biļetē.</span><span class="sxs-lookup"><span data-stu-id="be591-113">If more than 24 hours have passed since you first saw this issue, please log a support ticket.</span></span> <span data-ttu-id="be591-114">Daudzos gadījumos mēs jau strādājam pie risinājuma.</span><span class="sxs-lookup"><span data-stu-id="be591-114">In many cases, we're already working on a solution.</span></span> <span data-ttu-id="be591-115">Lai pabeigtu risinājumu, lūdzu, sniedziet mums vismaz 24 stundas.</span><span class="sxs-lookup"><span data-stu-id="be591-115">Please give us at least 24 hours to complete a solution.</span></span>
