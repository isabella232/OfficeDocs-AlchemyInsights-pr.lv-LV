---
title: Izdzēstas publiskās mapes atjaunošana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: bb7fe248714e9a7e7f4c48913b159b5c23132192
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47774538"
---
# <a name="restore-a-deleted-public-folder"></a>Izdzēstas publiskās mapes atjaunošana

**Lai atjaunotu izdzēstos vienumus no publiskas mapes**:

- Skatiet rakstu [nevar atkopt izdzēstos vienumus no nepasta publiskas mapes programmā Outlook 2016](https://aka.ms/pfrec).
 
**Lai atjaunotu izdzēstu publisku mapi (no jebkura tipa)**: 

- Lūdzu, izmantojiet šādu EXO PowerShell komandu:

    Sintakse

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Piemērs: tālāk norādītā komanda atjaunos Subfolder1 un novietos to zem \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Detalizētu informāciju skatiet rakstā [izdzēstas publiskās mapes atjaunošana](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
