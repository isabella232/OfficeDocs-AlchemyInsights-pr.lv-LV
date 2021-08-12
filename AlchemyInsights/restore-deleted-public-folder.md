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
ms.openlocfilehash: 6df196fc0bde37c962e3aa84dd602ee414dad3d329addfd16cb6e3dcc40fc2ae
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53943382"
---
# <a name="restore-a-deleted-public-folder"></a>Izdzēstas publiskās mapes atjaunošana

**Lai atjaunotu izdzēstos vienumus no publiskas mapes:**

- Skatiet [rakstu Jūs nevarat atkopt izdzēstos vienumus no mapes, kas nav pasts, šajā Outlook 2016.](https://aka.ms/pfrec)
 
**Lai atjaunotu izdzēstu publisko mapi (jebkura tipa):** 

- Lūdzu, izmantojiet šādu EXO PowerShell komandu:

    Sintakse:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Piemērs: Izmantojot šo komandu, tiks atjaunota apakšmape1 un novietota apakšmapē \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

[Papildinformāciju skatiet rakstā Izdzēstas](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) publiskās mapes atjaunošana.
