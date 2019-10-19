---
title: Piekļuves ierobežošana programmā SharePoint vai OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 037331d71f06750d972c0b6278b23bb15c4806ca
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/18/2019
ms.locfileid: "36551458"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="707a8-102">Piekļuves ierobežošana programmā SharePoint vai OneDrive</span><span class="sxs-lookup"><span data-stu-id="707a8-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="707a8-103">Programmā SharePoint un OneDrive varat ierobežot piekļuvi tādiem vienumiem kā faili, mapes un saraksti, piešķirot piekļuvi tikai tām grupām vai personām, kurām vēlaties piekļūt.</span><span class="sxs-lookup"><span data-stu-id="707a8-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="707a8-104">Pēc noklusējuma SharePoint atļaujas tiek pārmantotas no hierarhijas augstāk.</span><span class="sxs-lookup"><span data-stu-id="707a8-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="707a8-105">Tāpēc fails pārmanto atļaujas no mapes, kura pārmanto atļaujas no bibliotēkas, kura pārmanto atļaujas no vietnes.</span><span class="sxs-lookup"><span data-stu-id="707a8-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="707a8-106">Varat kopīgot augstākā līmenī (piemēram, koplietojot visu vietni) un pēc tam pārtraukt pārmantošanu, ja nevēlaties kopīgot visus vietnes vienumus.</span><span class="sxs-lookup"><span data-stu-id="707a8-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="707a8-107">Tomēr mēs neiesakām šo, jo tas padara saglabāt atļaujas sarežģītāka un mulsinoša nākotnē.</span><span class="sxs-lookup"><span data-stu-id="707a8-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="707a8-108">Lūk, ko jūs varētu darīt tā vietā:</span><span class="sxs-lookup"><span data-stu-id="707a8-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="707a8-109">Ja, piemēram, vēlaties koplietot visu mapes saturu, izņemot vienu failu, pārvietojiet šo failu uz jaunu atrašanās vietu, kas netiek koplietota.</span><span class="sxs-lookup"><span data-stu-id="707a8-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="707a8-110">Ja mapē ir divas apakšmapes un vēlaties koplietot vienu apakšmapi ar A un B grupām un atļaut tikai grupēt piekļuvi otrajai apakšmapei, koplietojiet vecākmapi ar A grupu un pievienojiet B grupu pirmajai apakšmapei.</span><span class="sxs-lookup"><span data-stu-id="707a8-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="707a8-111">Faila vai mapes koplietošanas pārtraukšana</span><span class="sxs-lookup"><span data-stu-id="707a8-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

