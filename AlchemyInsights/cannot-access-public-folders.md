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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="3d4a5-102">Outlook nevar izveidot savienojumu ar publiskajām mapēm</span><span class="sxs-lookup"><span data-stu-id="3d4a5-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="3d4a5-103">Ja piekļuve publiskajām mapēm dažiem lietotājiem nedarbojas, izmēģiniet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="3d4a5-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="3d4a5-104">Izveidojiet savienojumu ar EXO PowerShell un konfigurējiet parametru DefaultPublicFolderMailbox problēmas lietotāja kontā, lai tas atbilstu parametram lietotāja kontā, kas darbojas.</span><span class="sxs-lookup"><span data-stu-id="3d4a5-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="3d4a5-105">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="3d4a5-105">Example:</span></span>

<span data-ttu-id="3d4a5-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="3d4a5-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="3d4a5-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="3d4a5-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="3d4a5-108">Uzgaidiet vismaz vienu stundu, līdz izmaiņas stājas spēkā.</span><span class="sxs-lookup"><span data-stu-id="3d4a5-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="3d4a5-109">Ja problēma joprojām pastāv, izpildiet šo procedūru, lai [novērstu](https://aka.ms/pfcte) publisko mapju piekļuves problēmas, izmantojot Outlook.</span><span class="sxs-lookup"><span data-stu-id="3d4a5-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="3d4a5-110">**Lai noteiktu, kuri lietotāji var piekļūt publiskajām mapēm, izmantojot programmu Outlook:**</span><span class="sxs-lookup"><span data-stu-id="3d4a5-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="3d4a5-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true vai $false</span><span class="sxs-lookup"><span data-stu-id="3d4a5-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="3d4a5-112">$true. Atļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="3d4a5-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="3d4a5-113">$false: neļaujiet lietotājiem piekļūt publiskajām mapēm programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="3d4a5-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="3d4a5-114">Šī ir noklusējuma vērtība.</span><span class="sxs-lookup"><span data-stu-id="3d4a5-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="3d4a5-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="3d4a5-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="3d4a5-116">**Piezīme** Šī procedūra var kontrolēt savienojumus tikai ar Outlook datora versiju Windows klientiem.</span><span class="sxs-lookup"><span data-stu-id="3d4a5-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="3d4a5-117">Lietotājs var turpināt piekļūt publiskajām mapēm, izmantojot OWA vai Outlook darbam ar Mac.</span><span class="sxs-lookup"><span data-stu-id="3d4a5-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="3d4a5-118">Papildinformāciju skatiet rakstā [Atbalsts kontrolētiem savienojumiem ar publiskajām mapēm programmā Outlook.](https://aka.ms/controlpf)</span><span class="sxs-lookup"><span data-stu-id="3d4a5-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>