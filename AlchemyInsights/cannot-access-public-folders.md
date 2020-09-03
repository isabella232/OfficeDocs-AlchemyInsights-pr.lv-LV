---
title: Nevar piekļūt publiskajām mapēm
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
- "3462"
ms.openlocfilehash: d63a193585cb73c2ce8e160d413db4e837100d33
ms.sourcegitcommit: d3ace2376195d54229ee1e232daf8133ba4e58a9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/03/2020
ms.locfileid: "47341410"
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