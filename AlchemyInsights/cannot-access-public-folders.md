---
title: Nevar piekļūt publiskajām mapēm
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
- "3462"
ms.openlocfilehash: f129da8731877aa00fd9b1dcf20905d353a4895303390ce7ff5642a8ff3ccbc2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53996637"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook nevar izveidot savienojumu ar publiskajām mapēm

Ja piekļuve publiskajām mapēm dažiem lietotājiem nedarbojas, izmēģiniet tālāk norādītās darbības.

Savienošana uz EXO PowerShell un problēmas lietotāja kontā konfigurējiet parametru DefaultPublicFolderMailbox, lai tas atbilstu parametram lietotāja kontā, kas darbojas.

Piemērs:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Uzgaidiet vismaz vienu stundu, līdz izmaiņas stājas spēkā.

Ja problēma joprojām pastāv, izpildiet šo [procedūru,](https://aka.ms/pfcte) lai novērstu problēmas saistībā ar piekļuvi publiskajām mapēm, Outlook.
 
**Lai noteiktu, kuri lietotāji var piekļūt publiskajām mapēm, izmantojot Outlook:**

1.  Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true vai $false  
      
    $true: atļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook  
      
    $false: neļaut lietotājam piekļūt publiskajām mapēm programmā Outlook. Šī ir noklusējuma vērtība.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Piezīme** Šī procedūra var kontrolēt savienojumus tikai ar Outlook datoru Windows klientiem. Lietotājs var turpināt piekļūt publiskajām mapēm, izmantojot OWA vai Outlook for Mac.
 
Papildinformāciju skatiet rakstā [Atbalsts kontrolētiem savienojumiem ar publiskajām mapēm Outlook.](https://aka.ms/controlpf)