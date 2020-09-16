---
title: Grupas pievienošana SharePoint vietnei
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: 9bec2f71465e43e1c3cba038e0e68949672ceb8a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771215"
---
# <a name="issues-when-creating-a-group-connected-site-in-sharepoint"></a><span data-ttu-id="568e9-102">Problēmas, veidojot grupas savienotu vietni koplietošanas vidē SharePoint</span><span class="sxs-lookup"><span data-stu-id="568e9-102">Issues when creating a group connected site in SharePoint</span></span>

1. <span data-ttu-id="568e9-103">Dažas bieži sastopamas problēmas, kas rodas, veidojot vai atkārtoti izveidojot grupu savienotu vietni.</span><span class="sxs-lookup"><span data-stu-id="568e9-103">Some common issues encountered when creating or re-creating a group connected site.</span></span>
<span data-ttu-id="568e9-104">Ja esat izdzēsis grupu un tās pievienoto vietni un vēlaties izveidot citu vietni ar vienu un to pašu vietrādi URL, ir jānoņem iepriekšējā vietne.</span><span class="sxs-lookup"><span data-stu-id="568e9-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

   - <span data-ttu-id="568e9-105">Lejupielādēt [spo pārvaldības čaulu](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="568e9-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>
   - <span data-ttu-id="568e9-106">Lai iegūtu papildinformāciju par darba sākšanu pakalpojumā PowerShell, skatiet rakstu [Darba sākšana ar SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span><span class="sxs-lookup"><span data-stu-id="568e9-106">For more info on getting started with Powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite).</span></span>
   - <span data-ttu-id="568e9-107">Noņemiet vietni no izdzēstajām vietnēm, izmantojot funkciju [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) PowerShell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="568e9-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) Powershell cmdlet.</span></span> <span data-ttu-id="568e9-108">PowerShell ir nepieciešama, lai neatgriezeniski dzēstu grupas vietnes.</span><span class="sxs-lookup"><span data-stu-id="568e9-108">Powershell is required to permanently delete group sites.</span></span>

1. <span data-ttu-id="568e9-109">Ja izveidojat grupai pievienotu vietni un saņemat brīdinājumu: **cita grupa ar tādu pašu aizstājvārdu jau pastāv**, atzīmējiet esošās grupas no [Microsoft 365 administrēšanas centra](https://admin.microsoft.com/AdminPortal/Home#/groups).</span><span class="sxs-lookup"><span data-stu-id="568e9-109">If you're creating a group connected site and receive a warning: **Another group with the same alias already exists**, check the existing groups from the [Microsoft 365 admin center](https://admin.microsoft.com/AdminPortal/Home#/groups).</span></span> <span data-ttu-id="568e9-110">Lai atrisinātu šo problēmu, izdzēsiet esošo grupu, ja tā vairs nav vajadzīga, vai izveidojiet vietni ar atšķirīgu aizstājvārdu.</span><span class="sxs-lookup"><span data-stu-id="568e9-110">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

1. <span data-ttu-id="568e9-111">Pastāv vairāki veidi, kā izveidot un izmantot mūsdienīgas grupas ar SharePoint.</span><span class="sxs-lookup"><span data-stu-id="568e9-111">There are different ways to create and use modern groups with SharePoint.</span></span>

   - <span data-ttu-id="568e9-112">Esošās vietnes varat savienot ar Microsoft 365 grupu.</span><span class="sxs-lookup"><span data-stu-id="568e9-112">You can connect existing sites to a Microsoft 365 group.</span></span> <span data-ttu-id="568e9-113">Papildinformāciju skatiet rakstā [Microsoft 365 grupas savienošana, izmantojot SharePoint lietotāja interfeisu](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="568e9-113">For more info, see [Connect a Microsoft 365 group using the SharePoint user interface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>
   - <span data-ttu-id="568e9-114">Lai izveidotu savienotu Microsoft 365 grupu, ir jāizveido [grupas vietne](https://admin.microsoft.com/sharepoint).</span><span class="sxs-lookup"><span data-stu-id="568e9-114">To create a Microsoft 365 group connected site, you'll need to create a [Team Site](https://admin.microsoft.com/sharepoint).</span></span>
