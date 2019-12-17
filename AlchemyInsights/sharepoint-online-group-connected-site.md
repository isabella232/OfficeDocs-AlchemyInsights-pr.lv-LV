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
ms.openlocfilehash: 14ad9dd094902c85eaf0398c76003cea20ad4c0a
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051108"
---
# <a name="issues-when-creating-or-group-connected-sites-in-sharepoint-online"></a><span data-ttu-id="75e44-102">Problēmas, veidojot vai grupu pievienotās vietnes SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="75e44-102">Issues when creating or group connected sites in SharePoint Online</span></span>

<span data-ttu-id="75e44-103">Ir pāris bieži sastopamas problēmas, veidojot vai atkārtoti izveidot savienojumu grupas vietni.</span><span class="sxs-lookup"><span data-stu-id="75e44-103">There are a couple of common issues encountered when creating or re-creating a group connected site.</span></span>

 <span data-ttu-id="75e44-104">Ja esat izdzēsis grupu un tās Savienoto vietni un vēlaties izveidot citu vietni ar tādu pašu URL, jums vajadzēs neatgriezeniski noņemt iepriekšējo vietni.</span><span class="sxs-lookup"><span data-stu-id="75e44-104">If you have deleted a group and its connected site and wish to create another site with the same URL, you'll need to permanently remove the previous site.</span></span>

<span data-ttu-id="75e44-105">Lejupielādēt [spo Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span><span class="sxs-lookup"><span data-stu-id="75e44-105">Download [SPO Management Shell](https://support.office.com/article/introduction-to-the-sharepoint-online-management-shell-c16941c3-19b4-4710-8056-34c034493429)</span></span>

 <span data-ttu-id="75e44-106">Papildinformāciju par darba sākšanu programmā PowerShell skatiet rakstā [Darba sākšana ar SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span><span class="sxs-lookup"><span data-stu-id="75e44-106">For more info on getting started with powershell, see [Getting started with SharePoint Online Management Shell](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps)</span></span>

<span data-ttu-id="75e44-107">Noņemt vietni no izdzēstās vietnes, izmantojot PowerShell cmdlet [Noņemt SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) .</span><span class="sxs-lookup"><span data-stu-id="75e44-107">Remove the Site from Deleted Sites using the [Remove-SPODeletedSite](https://docs.microsoft.com/powershell/module/sharepoint-online/remove-sposite?view=sharepoint-ps) powershell cmdlet.</span></span>

<span data-ttu-id="75e44-108">Ja veidojat ar grupu saistītu vietni un saņemat brīdinājumu, tad jau pastāv cita grupa ar šādu aizstājvārdu, pārbaudiet esošās grupas no [Office 365 no administrēšanas centra](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span><span class="sxs-lookup"><span data-stu-id="75e44-108">If you're creating a group connected site and receive a warning Another group with the same alias already exists, check the existing groups from the [Office 365 from the Admin Center](https://admin.microsoft.com/Adminportal/Home?source=applauncher#/groups).</span></span> <span data-ttu-id="75e44-109">Lai novērstu šo problēmu, izdzēsiet esošo grupu, ja tā vairs nav nepieciešama vai izveidot vietni ar citu piešķirto aizstājvārdu.</span><span class="sxs-lookup"><span data-stu-id="75e44-109">To resolve the issue, delete the existing group if it's no longer needed or create the site with a different alias assigned.</span></span>

<span data-ttu-id="75e44-110">Ir dažādi veidi, kā izveidot un izmantot modernas grupas ar SharePoint.</span><span class="sxs-lookup"><span data-stu-id="75e44-110">There are different ways to create and use modern groups with SharePoint.</span></span>

<span data-ttu-id="75e44-111">Esošās vietnes var savienot ar Office 365 grupu.</span><span class="sxs-lookup"><span data-stu-id="75e44-111">You can connect existing sites to an Office 365 group.</span></span> <span data-ttu-id="75e44-112">Papildinformāciju skatiet rakstā [Office 365 grupas savienošana, izmantojot SharePoint lietotāja ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span><span class="sxs-lookup"><span data-stu-id="75e44-112">For more info, see [Connect an Office 365 group using the SharePoint user ineterface](https://docs.microsoft.com/sharepoint/dev/transform/modernize-connect-to-office365-group#connect-an-office-365-group-using-the-sharepoint-user-interface).</span></span>

<span data-ttu-id="75e44-113">Lai izveidotu Office 365 grupu, kas ir savienota ar vietni, ir jāizveido darba grupas vietne.</span><span class="sxs-lookup"><span data-stu-id="75e44-113">To create an Office 365 group connected site, you'll need to create a Team Site.</span></span> <span data-ttu-id="75e44-114">Papildinformāciju skatiet sadaļā [grupas vietnes izveide pakalpojumā SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span><span class="sxs-lookup"><span data-stu-id="75e44-114">For more info, see [Create a team site in SharePoint](https://support.office.com/article/create-a-team-site-in-sharepoint-ef10c1e7-15f3-42a3-98aa-b5972711777d).</span></span>

