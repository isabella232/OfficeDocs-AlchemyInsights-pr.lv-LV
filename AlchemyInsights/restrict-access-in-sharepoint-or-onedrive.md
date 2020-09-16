---
title: Piekļuves ierobežošana koplietošanas vidē SharePoint vai pakalpojumā OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: d8be1eb5bdcd0b5b08ddad32a45b6282c788c26a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47720689"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="710de-102">Piekļuves ierobežošana koplietošanas vidē SharePoint vai pakalpojumā OneDrive</span><span class="sxs-lookup"><span data-stu-id="710de-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="710de-103">Koplietošanas vidē SharePoint un OneDrive varat ierobežot piekļuvi tādiem vienumiem kā faili, mapes un saraksti, piešķirot piekļuvi tikai grupām vai personām, kurām vēlaties piešķirt piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="710de-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="710de-104">Pēc noklusējuma hierarhiskā vidē SharePoint atļaujas tiek pārmantotas augstāk.</span><span class="sxs-lookup"><span data-stu-id="710de-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="710de-105">Tādējādi fails pārmanto atļaujas no mapes, kas pārmanto atļaujas no bibliotēkas, kas pārmanto atļaujas no vietnes.</span><span class="sxs-lookup"><span data-stu-id="710de-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="710de-106">Varat kopīgot augstākos līmeņos (piemēram, kopīgojot visu vietni) un pēc tam pārtraukt pārmantošanu, ja nevēlaties kopīgot visus vienumus vietnē.</span><span class="sxs-lookup"><span data-stu-id="710de-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="710de-107">Tomēr mēs to neiesakām, jo tā nodrošina atļauju sarežģītāku un mulsinošu nākotnē.</span><span class="sxs-lookup"><span data-stu-id="710de-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="710de-108">Tā vietā varat rīkoties šādi:</span><span class="sxs-lookup"><span data-stu-id="710de-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="710de-109">Ja, piemēram, vēlaties kopīgot visu mapes saturu, izņemot vienu failu, pārvietojiet šo failu uz citu atrašanās vietu, kas netiek koplietota.</span><span class="sxs-lookup"><span data-stu-id="710de-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="710de-110">Ja mapē ir divas apakšmapes un vēlaties koplietot vienu apakšmapi ar A un B grupām un atļaut tikai grupēt piekļuvi otrai apakšmapei, kopīgojiet vecākmapi ar grupu A un pēc tam pievienojiet grupu B pirmajai apakšmapei.</span><span class="sxs-lookup"><span data-stu-id="710de-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="710de-111">Faila vai mapes kopīgošanas pārtraukšana </span><span class="sxs-lookup"><span data-stu-id="710de-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

