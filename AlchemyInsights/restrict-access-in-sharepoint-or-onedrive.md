---
title: Ierobežot piekļuvi SharePoint vai OneDrive
ms.author: mikeplum
author: MikePlumleyMSFT
ms.date: 8/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: af1b936b-0475-497b-a6d3-e671aef7b717
ms.openlocfilehash: e5458226fe33bd5cb3da1f608fb113b888fbfd16
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36551458"
---
# <a name="restrict-access-in-sharepoint-or-onedrive"></a><span data-ttu-id="af7e2-102">Ierobežot piekļuvi SharePoint vai OneDrive</span><span class="sxs-lookup"><span data-stu-id="af7e2-102">Restrict access in SharePoint or OneDrive</span></span>

<span data-ttu-id="af7e2-103">SharePoint un OneDrive, jūs ierobežojat piekļuvi precēm, piemēram, failus, mapes un sarakstus, piešķirot piekļuvi tikai uz grupām vai personām, kas vēlas piekļūt.</span><span class="sxs-lookup"><span data-stu-id="af7e2-103">In SharePoint and OneDrive, you restrict access to items like files, folders, and lists by granting access only to groups or individuals you want to have access.</span></span> <span data-ttu-id="af7e2-104">Pēc noklusējuma SharePoint atļaujas tiek pārmantotas no hierarhijā augstāk.</span><span class="sxs-lookup"><span data-stu-id="af7e2-104">By default, permissions in SharePoint are inherited from higher up in the hierarchy.</span></span> <span data-ttu-id="af7e2-105">Tātad failu manto atļaujas no mapes, kas manto atļaujas no bibliotēkas, kas manto atļaujas no vietnes.</span><span class="sxs-lookup"><span data-stu-id="af7e2-105">So a file inherits its permissions from the folder, which inherits its permissions from the library, which inherits its permissions from the site.</span></span>
  
<span data-ttu-id="af7e2-106">Varat kopīgot augstākā līmenī (piemēram, daloties ar visu vietā) un pēc tam pārtraukt pārmantošanu, ja nevēlaties koplietot visus elementus lapā.</span><span class="sxs-lookup"><span data-stu-id="af7e2-106">You can share at a higher level (such as by sharing an entire site) and then break inheritance if you don't want to share all the items on the site.</span></span> <span data-ttu-id="af7e2-107">Tomēr nav ieteicams to, jo tas padara uzturēšanas atļaujas nākotnē sarežģītu un neskaidru.</span><span class="sxs-lookup"><span data-stu-id="af7e2-107">However, we don't recommend this because it makes maintaining the permissions more complex and confusing in the future.</span></span> <span data-ttu-id="af7e2-108">Lūk, ko tu varētu darīt:</span><span class="sxs-lookup"><span data-stu-id="af7e2-108">Here's what you could do instead:</span></span>
  
- <span data-ttu-id="af7e2-109">Ja, piemēram, vēlaties koplietot visu saturu, izņemot vienu failu, mapi pārvietot šo failu uz jaunu atrašanās vietu, kas nav koplietots.</span><span class="sxs-lookup"><span data-stu-id="af7e2-109">If, for example, you want to share all the contents of a folder except for one file in it, move that file to a new location that isn't shared.</span></span>
    
- <span data-ttu-id="af7e2-110">Ja jums ir divas apakšmapēm mapē un vēlaties koplietot vienu apakšmapi ar A un B grupas un atļaut tikai A grupa piekļuvi otrās apakšmapi, mātes mapi koplietot ar grupas A un B grupas pievienošana pirmo apakšmapi.</span><span class="sxs-lookup"><span data-stu-id="af7e2-110">If you have two subfolders in a folder, and you want to share one subfolder with groups A and B and allow only group A access to the second subfolder, share the parent folder with group A and add group B to the first subfolder.</span></span>
    
[<span data-ttu-id="af7e2-111">Lai beigtu sūtīt failu vai mapi</span><span class="sxs-lookup"><span data-stu-id="af7e2-111">Stop sharing a file or folder </span></span>](https://go.microsoft.com/fwlink/?linkid=2008861)
  

