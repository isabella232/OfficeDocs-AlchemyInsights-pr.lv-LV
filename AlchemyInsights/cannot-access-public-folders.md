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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="ec3af-102">Outlook nevar izveidot savienojumu ar publiskajām mapēm</span><span class="sxs-lookup"><span data-stu-id="ec3af-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="ec3af-103">Ja dažiem lietotājiem nedarbojas piekļuve publiskajai mapei, izmēģiniet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="ec3af-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="ec3af-104">Izveidot savienojumu ar EXO PowerShell un konfigurēt DefaultPublicFolderMailbox parametru problēmu lietotāja kontā, lai tas atbilstu parametram darba lietotāja kontā.</span><span class="sxs-lookup"><span data-stu-id="ec3af-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="ec3af-105">Piemēram</span><span class="sxs-lookup"><span data-stu-id="ec3af-105">Example:</span></span>

<span data-ttu-id="ec3af-106">Get-Pastkaste WorkingUser | pēdu DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="ec3af-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="ec3af-107">Iestatīt-pastkastes ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="ec3af-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="ec3af-108">Lai izmaiņas stātos spēkā, uzgaidiet vismaz vienu stundu.</span><span class="sxs-lookup"><span data-stu-id="ec3af-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="ec3af-109">Ja problēma joprojām pastāv, lūdzu, veiciet [šīs darbības](https://aka.ms/pfcte) , lai novērstu publisko mapju piekļuves problēmas, izmantojot programmu Outlook.</span><span class="sxs-lookup"><span data-stu-id="ec3af-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="ec3af-110">**Lai kontrolētu, kuri lietotāji var piekļūt publiskajām mapēm, izmantojot programmu Outlook**:</span><span class="sxs-lookup"><span data-stu-id="ec3af-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="ec3af-111">Izmantojiet Set-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE vai $FALSE</span><span class="sxs-lookup"><span data-stu-id="ec3af-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="ec3af-112">$true: atļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="ec3af-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="ec3af-113">$false: neļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="ec3af-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="ec3af-114">Šī ir noklusējuma vērtība.</span><span class="sxs-lookup"><span data-stu-id="ec3af-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="ec3af-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="ec3af-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="ec3af-116">**Piezīmes** Šī procedūra var vadīt savienojumus tikai ar Outlook datora Windows klientiem.</span><span class="sxs-lookup"><span data-stu-id="ec3af-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="ec3af-117">Lietotājs var turpināt piekļūt publiskajām mapēm, izmantojot OWA vai Outlook darbam ar Mac.</span><span class="sxs-lookup"><span data-stu-id="ec3af-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="ec3af-118">Lai iegūtu papildinformāciju, skatiet rakstu kā paziņot [par atbalstu kontrolētajiem savienojumiem ar publiskajām mapēm programmā Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="ec3af-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>