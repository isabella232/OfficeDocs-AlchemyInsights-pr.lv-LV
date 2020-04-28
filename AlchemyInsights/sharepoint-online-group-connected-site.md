---
title: Grupas pievienošana SharePoint vietnei
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 8ef33cbd44b01deaf0e45813d019f7696ef5def0
ms.sourcegitcommit: 286000b588adef1bbbb28337a9d9e087ec783fa2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/27/2020
ms.locfileid: "43912973"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="c6aa7-102">Problēmas, izveidojot grupu savienota vietnes SharePoint</span><span class="sxs-lookup"><span data-stu-id="c6aa7-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="c6aa7-103">Dažas bieži sastopamās problēmas radās, izveidojot vai atkārtoti izveidot savienojumu grupas vietni.</span><span class="sxs-lookup"><span data-stu-id="c6aa7-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="c6aa7-104">Ja esat izdzēsis grupu un tās Savienoto vietni un vēlaties izveidot citu vietni ar tādu pašu URL, jums vajadzēs neatgriezeniski noņemt iepriekšējo vietni.</span><span class="sxs-lookup"><span data-stu-id="c6aa7-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="c6aa7-105">Lejupielādēt [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="c6aa7-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="c6aa7-106">Papildinformāciju par darba sākšanu programmā PowerShell skatiet rakstā [Darba sākšana ar SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="c6aa7-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="c6aa7-107">Noņemt vietni no izdzēstās vietnes, izmantojot PowerShell cmdlet [Noņemt SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="c6aa7-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="c6aa7-108">PowerShell ir nepieciešams neatgriezeniski dzēst grupas vietnes.</span><span class="sxs-lookup"><span data-stu-id="c6aa7-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="c6aa7-109">Ja veidojat ar grupu saistītu vietni un saņemat brīdinājumu: **cita grupa ar tādu pašu aizstājvārdu jau pastāv**, pārbaudiet esošās grupas no [Microsoft 365 administrēšanas centra](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="c6aa7-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 Admin Center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="c6aa7-110">Lai novērstu šo problēmu, izdzēsiet esošo grupu, ja tā vairs nav nepieciešama vai izveidot vietni ar citu piešķirto aizstājvārdu.</span><span class="sxs-lookup"><span data-stu-id="c6aa7-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="c6aa7-111">Ir dažādi veidi, kā izveidot un izmantot modernas grupas ar SharePoint.</span><span class="sxs-lookup"><span data-stu-id="c6aa7-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="c6aa7-112">Esošās vietnes var savienot ar Microsoft 365 grupu.</span><span class="sxs-lookup"><span data-stu-id="c6aa7-112">You can connect existing sites to an Microsoft 365 group.</span></span> <span data-ttu-id="c6aa7-113">Papildinformāciju skatiet rakstā [Microsoft 365 grupas savienošana, izmantojot SharePoint lietotāja interfeisu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="c6aa7-113">For more info, see [Connect an Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="c6aa7-114">Izveidot savienojumu ar Microsoft 365 grupas vietni, jums vajadzēs izveidot [darba grupas vietni](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="c6aa7-114">To create an Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
