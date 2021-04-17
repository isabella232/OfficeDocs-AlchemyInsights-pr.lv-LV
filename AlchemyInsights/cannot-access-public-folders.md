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
ms.openlocfilehash: af5bd57512ee917d6e22d3838d55a2a1d62750d4
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51819519"
---
# <a name="outlook-cannot-connect-to-public-folders"></a>Outlook nevar izveidot savienojumu ar publiskajām mapēm

Ja piekļuve publiskajām mapēm dažiem lietotājiem nedarbojas, izmēģiniet tālāk norādītās darbības.

Izveidojiet savienojumu ar EXO PowerShell un konfigurējiet parametru DefaultPublicFolderMailbox problēmas lietotāja kontā, lai tas atbilstu parametram lietotāja kontā, kas darbojas.

Piemērs:

Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox

Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command>

Uzgaidiet vismaz vienu stundu, līdz izmaiņas stājas spēkā.

Ja problēma joprojām pastāv, izpildiet šo procedūru, lai [novērstu](https://aka.ms/pfcte) publisko mapju piekļuves problēmas, izmantojot Outlook.
 
**Lai noteiktu, kuri lietotāji var piekļūt publiskajām mapēm, izmantojot programmu Outlook:**

1.  Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true vai $false  
      
    $true. Atļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook  
      
    $false: neļaujiet lietotājiem piekļūt publiskajām mapēm programmā Outlook. Šī ir noklusējuma vērtība.  
        
2.  Set-OrganizationConfig -PublicFolderShowClientControl $true   
      
**Piezīme** Šī procedūra var kontrolēt savienojumus tikai ar Outlook datora versiju Windows klientiem. Lietotājs var turpināt piekļūt publiskajām mapēm, izmantojot OWA vai Outlook darbam ar Mac.
 
Papildinformāciju skatiet rakstā [Atbalsts kontrolētiem savienojumiem ar publiskajām mapēm programmā Outlook.](https://aka.ms/controlpf)