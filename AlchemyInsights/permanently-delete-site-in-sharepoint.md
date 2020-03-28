---
title: Neatgriezeniska vietnes izdzēšana SharePoint
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.custom: ''
ms.assetid:
- "5200006"
- "4391"
ms.openlocfilehash: 263317339d965d173a5a038fa006e0ce6f8476cc
ms.sourcegitcommit: da04e79b6072321caa16a6ceea6eb5f15de22394
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/25/2020
ms.locfileid: "42955164"
---
# <a name="permanently-delete-a-site-in-sharepoint"></a><span data-ttu-id="9279f-102">Neatgriezeniska vietnes izdzēšana SharePoint</span><span class="sxs-lookup"><span data-stu-id="9279f-102">Permanently delete a site in SharePoint</span></span>

<span data-ttu-id="9279f-103">Lai atkārtoti izmantotu vietrādi URL no izdzēstas vietnes (vietnes atkārtotai izveidei) vai neatgriezeniski izdzēstu vietni, jo tā vairs netiek lietota, varat **Neatgriezeniski dzēst** no jaunā SharePoint administrēšanas centra.</span><span class="sxs-lookup"><span data-stu-id="9279f-103">To reuse a URL from a deleted site (to recreate a site), or to permanently delete a site because it's no longer in use, you can use **Permanently Delete** from the New SharePoint Admin Center.</span></span> 

1. <span data-ttu-id="9279f-104">Dodieties uz [Izdzēstā vietņu lapa jaunā SharePoint administrēšanas centrā](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) un pierakstieties ar kontu, kuram ir administratora atļaujas jūsu organizācijai.</span><span class="sxs-lookup"><span data-stu-id="9279f-104">Go to the [Deleted sites page of the new SharePoint admin center](https://admin.microsoft.com/sharepoint?page=recycleBin&modern=true) and sign in with an account that has admin permissions for your organization.</span></span> 

2. <span data-ttu-id="9279f-105">Kreisajā kolonnā atlasiet vietni.</span><span class="sxs-lookup"><span data-stu-id="9279f-105">In the left column, select a site.</span></span> 

3. <span data-ttu-id="9279f-106">Noklikšķiniet uz **Neatgriezeniski izdzēst**.</span><span class="sxs-lookup"><span data-stu-id="9279f-106">Click **Permanently Delete**.</span></span> 

<span data-ttu-id="9279f-107">**Piezīme**: grupas savienotās vietnes nevar neatgriezeniski dzēst no jaunā SharePoint administrēšanas centra.</span><span class="sxs-lookup"><span data-stu-id="9279f-107">**Note**: Group-connected sites cannot be permanently deleted from the New SharePoint Admin Center.</span></span> <span data-ttu-id="9279f-108">Lai to izdarītu, ir jāizmanto [Noņemt SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite).</span><span class="sxs-lookup"><span data-stu-id="9279f-108">[Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-spodeletedsite) will need to be used instead.</span></span>  

<span data-ttu-id="9279f-109">Papildinformāciju skatiet rakstā [Neatgriezeniski dzēst vietni](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span><span class="sxs-lookup"><span data-stu-id="9279f-109">For more info, see [Permanently delete a site](https://docs.microsoft.com/sharepoint/delete-site-collection#permanently-delete-a-site).</span></span> 
