---
title: Izdzēstas publiskās mapes atjaunošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: d5480389c3bf50cee9fe30f7ec8d8ff28ef694ca
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51809446"
---
# <a name="restore-a-deleted-public-folder"></a><span data-ttu-id="a0cda-102">Izdzēstas publiskās mapes atjaunošana</span><span class="sxs-lookup"><span data-stu-id="a0cda-102">Restore a deleted public folder</span></span>

<span data-ttu-id="a0cda-103">**Lai atjaunotu izdzēstos vienumus no publiskas mapes:**</span><span class="sxs-lookup"><span data-stu-id="a0cda-103">**To restore deleted items from a public folder**:</span></span>

- <span data-ttu-id="a0cda-104">Skatiet [rakstu Programmā Outlook 2016](https://aka.ms/pfrec)nevar atkopt izdzēstos vienumus no publiskas mapes, kas nav pasts.</span><span class="sxs-lookup"><span data-stu-id="a0cda-104">See [You can't recover deleted items from a non-mail public folder in Outlook 2016](https://aka.ms/pfrec).</span></span>
 
<span data-ttu-id="a0cda-105">**Lai atjaunotu izdzēstu publisko mapi (jebkura tipa):**</span><span class="sxs-lookup"><span data-stu-id="a0cda-105">**To restore a deleted public folder (of any type)**:</span></span> 

- <span data-ttu-id="a0cda-106">Lūdzu, izmantojiet šādu EXO PowerShell komandu:</span><span class="sxs-lookup"><span data-stu-id="a0cda-106">Please use following EXO PowerShell command:</span></span>

    <span data-ttu-id="a0cda-107">Sintakse:</span><span class="sxs-lookup"><span data-stu-id="a0cda-107">Syntax:</span></span>

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    <span data-ttu-id="a0cda-108">Piemērs: Izmantojot šo komandu, tiks atjaunota apakšmape1 un novietota apakšmapē \Parent1:</span><span class="sxs-lookup"><span data-stu-id="a0cda-108">Example: The following command will restore Subfolder1 and place it under \Parent1:</span></span>

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

<span data-ttu-id="a0cda-109">[Papildinformāciju skatiet rakstā Izdzēstas](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) publiskās mapes atjaunošana.</span><span class="sxs-lookup"><span data-stu-id="a0cda-109">See [Restore a deleted public folder](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) for more details.</span></span>
