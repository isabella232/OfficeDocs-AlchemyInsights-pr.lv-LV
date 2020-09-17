---
title: Nevar piekļūt publiskajām mapēm
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
- "3462"
ms.openlocfilehash: 272918b38f6019cb2bdcaa4013baebaa5f04fe85
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47812554"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook nevar izveidot savienojumu ar publiskajām mapēm

Ja dažiem lietotājiem nedarbojas piekļuve publiskajai mapei, izmēģiniet tālāk norādītās darbības.

Izveidot savienojumu ar EXO PowerShell un konfigurēt DefaultPublicFolderMailbox parametru problēmu lietotāja kontā, lai tas atbilstu parametram darba lietotāja kontā.

Piemēram

Get-Pastkaste WorkingUser | pēdu DefaultPublicFolderMailbox, EffectivePublicFolderMailbox

Iestatīt-pastkastes ProblemUser-DefaultPublicFolderMailbox \<value from previous command>

Lai izmaiņas stātos spēkā, uzgaidiet vismaz vienu stundu.

Ja problēma joprojām pastāv, lūdzu, veiciet [šīs darbības](https://aka.ms/pfcte) , lai novērstu publisko mapju piekļuves problēmas, izmantojot programmu Outlook.
 
**Lai kontrolētu, kuri lietotāji var piekļūt publiskajām mapēm, izmantojot programmu Outlook**:

1.  Izmantojiet Set-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE vai $FALSE  
      
    $true: atļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook  
      
    $false: neļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook. Šī ir noklusējuma vērtība.  
        
2.  Set-OrganizationConfig-PublicFolderShowClientControl $true   
      
**Piezīmes** Šī procedūra var vadīt savienojumus tikai ar Outlook datora Windows klientiem. Lietotājs var turpināt piekļūt publiskajām mapēm, izmantojot OWA vai Outlook darbam ar Mac.
 
Lai iegūtu papildinformāciju, skatiet rakstu kā paziņot [par atbalstu kontrolētajiem savienojumiem ar publiskajām mapēm programmā Outlook](https://aka.ms/controlpf).