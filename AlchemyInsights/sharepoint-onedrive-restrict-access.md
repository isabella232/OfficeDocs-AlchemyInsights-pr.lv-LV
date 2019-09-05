---
title: Piekļuves ierobežošana programmā SharePoint vai OneDrive
ms.author: pebaum
author: Techwriter40
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: bef0612903b9bb455aa34e90d35d6b7b9093b4e0
ms.sourcegitcommit: a65d196d00adb70045af5caca9828fe44b951f61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/04/2019
ms.locfileid: "36750671"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="81d68-102">Piekļuves ierobežošana programmā SharePoint vai OneDrive</span><span class="sxs-lookup"><span data-stu-id="81d68-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="81d68-103">Ir vairāki veidi, kā ierobežot piekļuvi SharePoint Online/OneDrive pakalpojumiem.</span><span class="sxs-lookup"><span data-stu-id="81d68-103">There are many ways to restrict access to SharePoint Online/OneDrive services.</span></span> <span data-ttu-id="81d68-104">Šīs dažādās pieejas ierobežošanas metodes ir izklāstītas turpmāk.</span><span class="sxs-lookup"><span data-stu-id="81d68-104">These various access restriction methods are outlined below.</span></span> 

<span data-ttu-id="81d68-105">**Atļauju ierobežojums**</span><span class="sxs-lookup"><span data-stu-id="81d68-105">**Permission Restriction**</span></span>

<span data-ttu-id="81d68-106">SharePoint Online un OneDrive uzņēmumiem, mēs ierobežojam piekļuvi tādiem vienumiem kā vietnes, faili un mapes, piešķirot piekļuvi tikai tām grupām/personām, kurām ir jābūt piekļuvei.</span><span class="sxs-lookup"><span data-stu-id="81d68-106">In SharePoint Online and OneDrive for Business, we restrict access to items like sites, files and folders by only granting access to those groups/individuals who should have access.</span></span>

- [<span data-ttu-id="81d68-107">Atļauju pielāgošana SharePoint sarakstam vai bibliotēkai</span><span class="sxs-lookup"><span data-stu-id="81d68-107">Customize permissions for a SharePoint list or library</span></span>](https://support.office.com/article/Customize-permissions-for-a-SharePoint-list-or-library-02d770f3-59eb-4910-a608-5f84cc297782)

- [<span data-ttu-id="81d68-108">SharePoint vietnes atļauju pielāgošana</span><span class="sxs-lookup"><span data-stu-id="81d68-108">Customize SharePoint site permissions</span></span>](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions)

- [<span data-ttu-id="81d68-109">Mainīt atļaujas apakšmapē</span><span class="sxs-lookup"><span data-stu-id="81d68-109">Change the permissions on a subfolder</span></span>](https://support.office.com/article/Change-the-permissions-on-a-subfolder-5427BD7C-F20A-4F75-8CF2-5359DD45A1A6)

- [<span data-ttu-id="81d68-110">Piekļuves kontrole no nepārvaldītām ierīcēm</span><span class="sxs-lookup"><span data-stu-id="81d68-110">Control access from unmanaged devices</span></span>](https://docs.microsoft.com/sharepoint/control-access-from-unmanaged-devices)

<span data-ttu-id="81d68-111">SharePoint vai globālās administrēšanas Office 365, varat bloķēt vai ierobežot piekļuvi SharePoint un OneDrive saturu no nepārvaldīts ierīces (kas nav hibrīds AD pievienojās vai atbilst InTune).</span><span class="sxs-lookup"><span data-stu-id="81d68-111">As a SharePoint or global admin in Office 365, you can block or limit access to SharePoint and OneDrive content from unmanaged devices (those not hybrid AD joined or compliant in Intune).</span></span>

<span data-ttu-id="81d68-112">**Tīkla atrašanās vietas ierobežojums**</span><span class="sxs-lookup"><span data-stu-id="81d68-112">**Network Location Restriction**</span></span>

<span data-ttu-id="81d68-113">Kā IT administrators varat kontrolēt piekļuvi SharePoint un OneDrive resursiem, pamatojoties uz definētajām tīkla vietām, kurām uzticaties.</span><span class="sxs-lookup"><span data-stu-id="81d68-113">As an IT admin, you can control access to SharePoint and OneDrive resources based on defined network locations that you trust.</span></span> <span data-ttu-id="81d68-114">Šī ir pazīstama arī kā politika, kuras pamatā ir atrašanās vieta.</span><span class="sxs-lookup"><span data-stu-id="81d68-114">This is also known as location-based policy.</span></span> <span data-ttu-id="81d68-115">Lai iegūtu papildinformāciju, lūdzu, skatiet [piekļuves kontrole SharePoint Online un OneDrive datus, pamatojoties uz tīkla atrašanās vietu](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span><span class="sxs-lookup"><span data-stu-id="81d68-115">For more information, please see [Control access to SharePoint Online and OneDrive data based on network location](https://docs.microsoft.com/sharepoint/control-access-based-on-network-location)</span></span>

<span data-ttu-id="81d68-116">**Vietnes bloķēšanas ierobežojums**</span><span class="sxs-lookup"><span data-stu-id="81d68-116">**Site Lock Restriction**</span></span> 

<span data-ttu-id="81d68-117">Programmā SharePoint Online jums ir iespēja bloķēt vietņu kolekciju, tāpēc nevienam nav piekļuves.</span><span class="sxs-lookup"><span data-stu-id="81d68-117">Within SharePoint Online you have the ability to lock down a site collection, so no one has access.</span></span> <span data-ttu-id="81d68-118">Tas ir iestatīts, izmantojot PowerShell un [SharePoint Online pārvaldības čaulu](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) , izmantojot rekvizītu [Set sposite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -lockstate.</span><span class="sxs-lookup"><span data-stu-id="81d68-118">This is set via PowerShell and the [SharePoint Online Management Shell](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps) using the [Set-SPOSite](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) -LockState property.</span></span>

<span data-ttu-id="81d68-119">**Aizliegt lietotājiem veidot vietnes vai apakšvietnes**</span><span class="sxs-lookup"><span data-stu-id="81d68-119">**Restrict users from creating sites or subsites**</span></span>

<span data-ttu-id="81d68-120">Kā SharePoint admin vai Office 365 globālais administrators varat ļaut lietotājiem izveidot un pārvaldīt savas SharePoint vietnes, noteikt, kādas vietnes viņi var izveidot, un norādīt vietņu atrašanās vietu.</span><span class="sxs-lookup"><span data-stu-id="81d68-120">As a SharePoint admin or Office 365 global admin, you can let your users create and administer their own SharePoint sites, determine what kind of sites they can create, and specify the location of the sites.</span></span> <span data-ttu-id="81d68-121">Lai iegūtu papildinformāciju, lūdzu, skatiet [pārvaldīt vietnes izveide SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span><span class="sxs-lookup"><span data-stu-id="81d68-121">For more information, please see [Manage site creation in SharePoint Online](https://docs.microsoft.com/sharepoint/manage-site-creation)</span></span>

