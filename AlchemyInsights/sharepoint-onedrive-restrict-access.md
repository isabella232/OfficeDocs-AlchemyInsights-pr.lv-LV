---
title: Ierobežot piekļuvi SharePoint vai OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: 84f2d4b6e5fd2380a2fa96e30953c68aab203cd3
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36559884"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="d43ea-102">Ierobežot piekļuvi SharePoint vai OneDrive</span><span class="sxs-lookup"><span data-stu-id="d43ea-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="d43ea-103">Ir daudzi veidi, kā ierobežot piekļuvi SharePoint Online/OneDrive pakalpojumus.</span><span class="sxs-lookup"><span data-stu-id="d43ea-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="d43ea-104">Šīs dažādās piekļuves ierobežošanas metodes ir izklāstīti turpmāk.</span><span class="sxs-lookup"><span data-stu-id="d43ea-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="d43ea-105">**Ierobežot atļaujas**</span><span class="sxs-lookup"><span data-stu-id="d43ea-105">**Permission Restriction**</span></span>

<span data-ttu-id="d43ea-106">SharePoint Online un OneDrive uzņēmējdarbībai, mums ierobežot piekļuvi precēm, piemēram, vietnēm, failus un mapes tikai piešķirot piekļuvi šīm grupām/personām, vajadzētu būt pieejamai.</span><span class="sxs-lookup"><span data-stu-id="d43ea-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="d43ea-107">Pielāgot SharePoint saraksta vai bibliotēkas atļauju</span><span class="sxs-lookup"><span data-stu-id="d43ea-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="d43ea-108">Pielāgot SharePoint vietnes atļaujas</span><span class="sxs-lookup"><span data-stu-id="d43ea-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="d43ea-109">Mainīt atļaujas apakšmapi</span><span class="sxs-lookup"><span data-stu-id="d43ea-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="d43ea-110">No nepārvaldītiem ierīču piekļuves kontrole</span><span class="sxs-lookup"><span data-stu-id="d43ea-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="d43ea-111">Kā SharePoint vai globālās administrēšanas Office 365, var bloķēt vai ierobežot piekļuvi SharePoint un OneDrive saturu no nepārvaldītiem ierīču (tām nav hibrīds AD pievienojās vai atbilstošu Intune).</span><span class="sxs-lookup"><span data-stu-id="d43ea-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="d43ea-112">**Tīkla atrašanās vietas ierobežojums**</span><span class="sxs-lookup"><span data-stu-id="d43ea-112">**Network Location Restriction**</span></span>

<span data-ttu-id="d43ea-113">Kā IT administrators, jūs varat kontrolēt piekļuvi SharePoint un OneDrive resursus, balstoties uz noteiktiem tīkla vietas, kurām uzticaties.</span><span class="sxs-lookup"><span data-stu-id="d43ea-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="d43ea-114">Tas ir arī pazīstams kā politikas atkarībā no atrašanās vietas.</span><span class="sxs-lookup"><span data-stu-id="d43ea-114">This is also known as location-based policy.</span></span> <span data-ttu-id="d43ea-115">Plašāku informāciju skatiet [SharePoint Online un OneDrive datus, pamatojoties uz tīkla atrašanās vietas piekļuves kontrole](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="d43ea-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="d43ea-116">**Bloķēt vietnes ierobežojumu**</span><span class="sxs-lookup"><span data-stu-id="d43ea-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="d43ea-117">Programmā SharePoint Online, jums ir iespēja, lai bloķētu vietņu kolekciju, lai nevienam nav piekļuves.</span><span class="sxs-lookup"><span data-stu-id="d43ea-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="d43ea-118">Tas tiek iestatīts, izmantojot PowerShell un [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) , izmantojot [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) - LockState īpašumu.</span><span class="sxs-lookup"><span data-stu-id="d43ea-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="d43ea-119">**Aizliegtu lietotājiem veidot vietnes vai apakšvietņu**</span><span class="sxs-lookup"><span data-stu-id="d43ea-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="d43ea-120">Kā SharePoint administrēšanas vai Office 365 globālās administrēšanas, jūs varat ļaut lietotājiem izveidot un administrēt savas SharePoint vietnes, nosakiet, kāda veida portālos tie var radīt, un norādiet vietnes atrašanās vietu.</span><span class="sxs-lookup"><span data-stu-id="d43ea-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="d43ea-121">Plašāku informāciju skatiet [Manage vietņu izveide SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="d43ea-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

