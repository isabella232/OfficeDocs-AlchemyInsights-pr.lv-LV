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
# <a name="control-access-to-public-folders-using-outlook"></a><span data-ttu-id="f68dd-102">Kontrolējiet piekļuvi publiskajām mapēm, izmantojot programmu Outlook</span><span class="sxs-lookup"><span data-stu-id="f68dd-102">Control access to public folders using Outlook</span></span>

<span data-ttu-id="f68dd-103">Lai kontrolētu, kuri lietotāji var piekļūt publiskajām mapēm, izmantojot programmu Outlook:</span><span class="sxs-lookup"><span data-stu-id="f68dd-103">To control which users can access public folders using Outlook:</span></span>

1. <span data-ttu-id="f68dd-104">izmantojiet `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span><span class="sxs-lookup"><span data-stu-id="f68dd-104">Use `Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false`</span></span>

<span data-ttu-id="f68dd-105">$true: atļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="f68dd-105">$true: Allow users access public folders in Outlook</span></span>  
<span data-ttu-id="f68dd-106">$false: neļaut lietotājam piekļūt publiskajām mapēm programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="f68dd-106">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="f68dd-107">Šī ir noklusējuma vērtība.</span><span class="sxs-lookup"><span data-stu-id="f68dd-107">This is the default value.</span></span>  

2. `Set-OrganizationConfig -PublicFolderShowClientControl $true`

<span data-ttu-id="f68dd-108">Piezīme. Šī procedūra var kontrolēt tikai savienojumus ar programmas Outlook datora versiju Windows klientiem.</span><span class="sxs-lookup"><span data-stu-id="f68dd-108">Note: This procedure can only control connections with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="f68dd-109">Lietotāji var turpināt piekļūt publiskām mapēm, izmantojot OWA vai programmai Outlook darbam Mac.</span><span class="sxs-lookup"><span data-stu-id="f68dd-109">Users can continue accessing public folders using OWA or Outlook for Mac.</span></span>

<span data-ttu-id="f68dd-110">Papildinformāciju skatiet sadaļā [Kontrolēti savienojumi ar Outlook publiskajām mapēm](https://aka.ms/controlpf), lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="f68dd-110">For more information, see [Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf) for more information.</span></span>
