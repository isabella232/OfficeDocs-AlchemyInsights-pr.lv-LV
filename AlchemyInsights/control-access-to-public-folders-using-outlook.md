---
title: Kontrolējiet piekļuvi publiskajām mapēm, izmantojot programmu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "3500007"
- "3462"
ms.openlocfilehash: f528044ca7f6f2ee2812f9f831093c44eca26fe1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816747"
---
# <a name="control-access-to-public-folders-using-outlook"></a>Kontrolējiet piekļuvi publiskajām mapēm, izmantojot programmu Outlook

Lai kontrolētu, kuri lietotāji var piekļūt publiskajām mapēm, izmantojot programmu Outlook:

1. izmantojiet `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`

$true: atļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook  
$false: neļaut lietotājam piekļūt publiskajām mapēm programmā Outlook. Šī ir noklusējuma vērtība.  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

Piezīme. Šī procedūra var kontrolēt tikai savienojumus ar programmas Outlook datora versiju Windows klientiem. Lietotāji var turpināt piekļūt publiskām mapēm, izmantojot OWA vai programmai Outlook darbam Mac.

Papildinformāciju skatiet sadaļā [Kontrolēti savienojumi ar Outlook publiskajām mapēm](https://aka.ms/controlpf), lai iegūtu papildinformāciju.
