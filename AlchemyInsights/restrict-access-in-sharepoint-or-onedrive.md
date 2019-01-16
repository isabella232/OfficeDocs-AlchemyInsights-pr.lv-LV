---
title: Ierobežot piekļuvi SharePoint vai OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: b6be074ed5f7e83f8196ca3fe90252673896569f
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28300600"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="89920-102">Ierobežot piekļuvi SharePoint vai OneDrive</span><span class="sxs-lookup"><span data-stu-id="89920-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="89920-p101">SharePoint un OneDrive, jūs ierobežojat piekļuvi precēm, piemēram, failus, mapes un sarakstus, piešķirot piekļuvi tikai uz grupām vai personām, kas vēlas piekļūt. Pēc noklusējuma SharePoint atļaujas tiek pārmantotas no hierarhijā augstāk. Tātad failu manto atļaujas no mapes, kas manto atļaujas no bibliotēkas, kas manto atļaujas no vietnes.</span><span class="sxs-lookup"><span data-stu-id="89920-p101">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access. By default, permissions in SharePoint are inherited from higher up in the hierarchy. So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="89920-p102">Varat kopīgot augstākā līmenī (piemēram, daloties ar visu vietā) un pēc tam pārtraukt pārmantošanu, ja nevēlaties koplietot visus elementus lapā. Tomēr nav ieteicams to, jo tas padara uzturēšanas atļaujas nākotnē sarežģītu un neskaidru. Lūk, ko tu varētu darīt:</span><span class="sxs-lookup"><span data-stu-id="89920-p102">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site. However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future. Here's what you could do instead:</span></span>
  
- <span data-ttu-id="89920-109">Ja, piemēram, vēlaties koplietot visu saturu, izņemot vienu failu, mapi pārvietot šo failu uz jaunu atrašanās vietu, kas nav koplietots.</span><span class="sxs-lookup"><span data-stu-id="89920-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="89920-110">Ja jums ir divas apakšmapēm mapē un vēlaties koplietot vienu apakšmapi ar A un B grupas un atļaut tikai A grupa piekļuvi otrās apakšmapi, mātes mapi koplietot ar grupas A un B grupas pievienošana pirmo apakšmapi.</span><span class="sxs-lookup"><span data-stu-id="89920-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="89920-111">Lai beigtu sūtīt failu vai mapi</span><span class="sxs-lookup"><span data-stu-id="89920-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

