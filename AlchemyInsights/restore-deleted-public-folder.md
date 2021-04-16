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
# <a name="restore-a-deleted-public-folder"></a>Izdzēstas publiskās mapes atjaunošana

**Lai atjaunotu izdzēstos vienumus no publiskas mapes:**

- Skatiet [rakstu Programmā Outlook 2016](https://aka.ms/pfrec)nevar atkopt izdzēstos vienumus no publiskas mapes, kas nav pasts.
 
**Lai atjaunotu izdzēstu publisko mapi (jebkura tipa):** 

- Lūdzu, izmantojiet šādu EXO PowerShell komandu:

    Sintakse:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Piemērs: Izmantojot šo komandu, tiks atjaunota apakšmape1 un novietota apakšmapē \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

[Papildinformāciju skatiet rakstā Izdzēstas](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) publiskās mapes atjaunošana.
