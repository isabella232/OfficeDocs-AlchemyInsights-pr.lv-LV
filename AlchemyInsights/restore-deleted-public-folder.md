---
title: Izdzēstas publiskās mapes atjaunošana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3488"
ms.openlocfilehash: cd85dd3c0eb14f6e02ac4f912e733468403387aa
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158523"
---
# <a name="restore-a-deleted-public-folder"></a>Izdzēstas publiskās mapes atjaunošana

**Lai no publiskās mapes atjaunotu izdzēstos vienumus**:

- Skatiet [nevar atkopt izdzēstos vienumus no e-pasta publiskās mapes programmā Outlook 2016](https://aka.ms/pfrec).
 
**Lai atjaunotu dzēstu publisko mapi (jebkura veida)**: 

- Lūdzu, izmantojiet šādu komandu EXO PowerShell:

    Sintakse:

     `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse  | ?{$_.Name -eq "\<name_of_deleted_public_Folder"};Set-PublicFolder $pf.identity -Path \<path where the folder will be restored>`

    Piemērs: šī komanda atjaunos Subfolder1 un novietot to zem \Parent1:

    `$pf=Get-PublicFolder \NON_IPM_SUBTREE\DUMPSTER_ROOT -Recurse | ?{$_.Name -eq "Subfolder1"};Set-PublicFolder $pf.identity -Path \Parent1`

Plašāku informāciju skatiet sadaļā [izdzēstas publiskās mapes atjaunošana](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/restore-deleted-public-folder) .
