---
title: Grupas pievienošana SharePoint vietnei
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: f7d730bf-0d6e-424c-970c-6137c71cb50b
ms.openlocfilehash: f0126f7f753275e9bbf8c3a09a6af5faf9a27862
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34758737"
---
# <a name="create-group-connected-site-in-sharepoint-online"></a><span data-ttu-id="442e6-102">Izveidot grupu pievienotās vietnes SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="442e6-102">Create group connected site in SharePoint Online</span></span>

<span data-ttu-id="442e6-103">Tur ir pāris raksturīgām problēmām, kas radās, kad veidot vai atkārtoti veidot grupu saistītas vietnes.</span><span class="sxs-lookup"><span data-stu-id="442e6-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="442e6-104">Ja jūs esat izdzēsis grupas un tās pievienoto vietni un vēlaties izveidot citā vietā ar tādu pašu URL, jums vajadzēs neatgriezeniski noņemt iepriekšējā vietā.</span><span class="sxs-lookup"><span data-stu-id="442e6-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="442e6-105">Lejupielādējiet [SPO pārvaldības čaulu](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="442e6-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="442e6-106">Lai iegūtu vairāk informācijas par iesākumam ar powershell, skatiet [Darba sākšana ar SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="442e6-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="442e6-107">Noņemiet vietni no Izdzēstie vietnēs, izmantojot [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span><span class="sxs-lookup"><span data-stu-id="442e6-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="442e6-108">Ja veidojat grupu pievienotās vietnes un saņemt brīdinājumu citu grupu ar tāds pats aizstājvārds jau pastāv, pārbaudiet esošās grupas no [Office 365 no administrēšanas centrs](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="442e6-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="442e6-109">Atrisinātu problēmu, izdzēst esošu grupu, ja tā vairs nav vajadzīga vai izveidot vietni ar citu aizstājvārdu piešķir.</span><span class="sxs-lookup"><span data-stu-id="442e6-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="442e6-110">Ir dažādi veidi, kā izveidot un lietot mūsdienu grupām ar SharePoint.</span><span class="sxs-lookup"><span data-stu-id="442e6-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="442e6-111">Esošajās vietnēs var pieslēgties Office 365 grupa.</span><span class="sxs-lookup"><span data-stu-id="442e6-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="442e6-112">Lai iegūtu vairāk informācijas, skatiet [savienojuma izveidošana Office 365 grupu, izmantojot SharePoint lietotāja ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="442e6-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="442e6-113">Lai izveidotu Office 365 grupa pievienotās vietnes, jums vajadzēs radāt darba grupas vietni.</span><span class="sxs-lookup"><span data-stu-id="442e6-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="442e6-114">Lai iegūtu vairāk informācijas, skatiet [Create darba grupas vietni koplietošanas vidē SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="442e6-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

