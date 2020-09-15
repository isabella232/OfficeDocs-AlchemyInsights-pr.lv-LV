---
title: Piekļuves ierobežošana koplietošanas vidē SharePoint vai pakalpojumā OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e9eb1822a7770bc206992cc5fb7e54a5c972b7e2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47700462"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="8ce40-102">Piekļuves ierobežošana koplietošanas vidē SharePoint vai pakalpojumā OneDrive</span><span class="sxs-lookup"><span data-stu-id="8ce40-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="8ce40-103">Pastāv vairāki veidi, kā ierobežot piekļuvi pakalpojumam SharePoint Online/OneDrive pakalpojumiem.</span><span class="sxs-lookup"><span data-stu-id="8ce40-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="8ce40-104">Tālāk ir minētas dažādas pieejas ierobežojumu metodes.</span><span class="sxs-lookup"><span data-stu-id="8ce40-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="8ce40-105">**Atļauju ierobežojums**</span><span class="sxs-lookup"><span data-stu-id="8ce40-105">**Permission Restriction**</span></span>

<span data-ttu-id="8ce40-106">Pakalpojumā SharePoint Online un OneDrive darbam mēs ierobežojam piekļuvi tādiem vienumiem kā vietnes, faili un mapes, piešķirot piekļuvi tikai tām grupām/personām, kurām ir jābūt piekļuvei.</span><span class="sxs-lookup"><span data-stu-id="8ce40-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="8ce40-107">SharePoint saraksta vai bibliotēkas atļauju pielāgošana</span><span class="sxs-lookup"><span data-stu-id="8ce40-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="8ce40-108">SharePoint vietnes atļauju pielāgošana</span><span class="sxs-lookup"><span data-stu-id="8ce40-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="8ce40-109">Atļauju maiņa apakšmapē</span><span class="sxs-lookup"><span data-stu-id="8ce40-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="8ce40-110">Piekļuves kontrolēšana no nepārvaldītām ierīcēm</span><span class="sxs-lookup"><span data-stu-id="8ce40-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="8ce40-111">Kā SharePoint vai globālais administrators varat bloķēt vai ierobežot piekļuvi SharePoint un OneDrive saturam no nepārvaldītām ierīcēm (kas nav hibrīda reklāma un nav saderīga ar Intune).</span><span class="sxs-lookup"><span data-stu-id="8ce40-111">As a SharePoint or global admin, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="8ce40-112">**Tīkla atrašanās vietas ierobežojums**</span><span class="sxs-lookup"><span data-stu-id="8ce40-112">**Network Location Restriction**</span></span>

<span data-ttu-id="8ce40-113">Kā IT administrators varat kontrolēt piekļuvi SharePoint un OneDrive resursiem, pamatojoties uz noteiktām tīkla vietām, kurām uzticaties.</span><span class="sxs-lookup"><span data-stu-id="8ce40-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="8ce40-114">To sauc arī par atrašanās vietu.</span><span class="sxs-lookup"><span data-stu-id="8ce40-114">This is also known as location-based policy.</span></span> <span data-ttu-id="8ce40-115">Lai iegūtu papildinformāciju, skatiet rakstu [piekļuves kontrolēšana SharePoint Online un OneDrive datiem, pamatojoties uz tīkla atrašanās vietu](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="8ce40-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="8ce40-116">**Vietnes bloķēšanas ierobežojums**</span><span class="sxs-lookup"><span data-stu-id="8ce40-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="8ce40-117">Pakalpojumā SharePoint Online jums ir iespēja bloķēt vietņu kolekciju, līdz ar to nevienam nav piekļuves.</span><span class="sxs-lookup"><span data-stu-id="8ce40-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="8ce40-118">To iestata, izmantojot PowerShell un [SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) , izmantojot [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState rekvizītu.</span><span class="sxs-lookup"><span data-stu-id="8ce40-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="8ce40-119">**Lietotāju ierobežošana, lai izveidotu vietnes vai apakšvietnes**</span><span class="sxs-lookup"><span data-stu-id="8ce40-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="8ce40-120">Kā SharePoint administrators vai globālais administrators varat ļaut lietotājiem izveidot un pārvaldīt savas SharePoint vietnes, noteikt, kādas vietnes var izveidot un norādīt vietņu atrašanās vietu.</span><span class="sxs-lookup"><span data-stu-id="8ce40-120">As a SharePoint admin or Global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="8ce40-121">Lai iegūtu papildinformāciju, lūdzu, skatiet rakstu [vietņu izveides pārvaldība pakalpojumā SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="8ce40-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

