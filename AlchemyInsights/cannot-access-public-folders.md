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
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="c7991-102">Outlook nevar izveidot savienojumu ar publiskajām mapēm</span><span class="sxs-lookup"><span data-stu-id="c7991-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="c7991-103">Ja dažiem lietotājiem nedarbojas piekļuve publiskajai mapei, izmēģiniet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="c7991-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="c7991-104">Izveidot savienojumu ar EXO PowerShell un konfigurēt DefaultPublicFolderMailbox parametru problēmu lietotāja kontā, lai tas atbilstu parametram darba lietotāja kontā.</span><span class="sxs-lookup"><span data-stu-id="c7991-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="c7991-105">Piemēram</span><span class="sxs-lookup"><span data-stu-id="c7991-105">Example:</span></span>

<span data-ttu-id="c7991-106">Get-Pastkaste WorkingUser | pēdu DefaultPublicFolderMailbox, EffectivePublicFolderMailbox</span><span class="sxs-lookup"><span data-stu-id="c7991-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="c7991-107">Iestatīt-pastkastes ProblemUser-DefaultPublicFolderMailbox \<value from previous command></span><span class="sxs-lookup"><span data-stu-id="c7991-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="c7991-108">Lai izmaiņas stātos spēkā, uzgaidiet vismaz vienu stundu.</span><span class="sxs-lookup"><span data-stu-id="c7991-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="c7991-109">Ja problēma joprojām pastāv, lūdzu, veiciet [šīs darbības](https://aka.ms/pfcte) , lai novērstu publisko mapju piekļuves problēmas, izmantojot programmu Outlook.</span><span class="sxs-lookup"><span data-stu-id="c7991-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>
 
<span data-ttu-id="c7991-110">**Lai kontrolētu, kuri lietotāji var piekļūt publiskajām mapēm, izmantojot programmu Outlook**:</span><span class="sxs-lookup"><span data-stu-id="c7991-110">**To control which users can access public folders using Outlook**:</span></span>

1.  <span data-ttu-id="c7991-111">Izmantojiet Set-CASMailbox <mailboxname> -PublicFolderClientAccess $TRUE vai $FALSE</span><span class="sxs-lookup"><span data-stu-id="c7991-111">Use Set-CASMailbox <mailboxname> -PublicFolderClientAccess $true or $false</span></span>  
      
    <span data-ttu-id="c7991-112">$true: atļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="c7991-112">$true: Allow users access public folders in Outlook</span></span>  
      
    <span data-ttu-id="c7991-113">$false: neļaut lietotājiem piekļūt publiskajām mapēm programmā Outlook.</span><span class="sxs-lookup"><span data-stu-id="c7991-113">$false: Prevent user access to public folders in Outlook.</span></span> <span data-ttu-id="c7991-114">Šī ir noklusējuma vērtība.</span><span class="sxs-lookup"><span data-stu-id="c7991-114">This is the default value.</span></span>  
        
2.  <span data-ttu-id="c7991-115">Set-OrganizationConfig-PublicFolderShowClientControl $true</span><span class="sxs-lookup"><span data-stu-id="c7991-115">Set-OrganizationConfig -PublicFolderShowClientControl $true</span></span>   
      
<span data-ttu-id="c7991-116">**Piezīmes** Šī procedūra var vadīt savienojumus tikai ar Outlook datora Windows klientiem.</span><span class="sxs-lookup"><span data-stu-id="c7991-116">**Note** This procedure can control connections only with Outlook desktop for Windows clients.</span></span> <span data-ttu-id="c7991-117">Lietotājs var turpināt piekļūt publiskajām mapēm, izmantojot OWA vai Outlook darbam ar Mac.</span><span class="sxs-lookup"><span data-stu-id="c7991-117">A user can continue accessing public folders using OWA or Outlook for Mac.</span></span>
 
<span data-ttu-id="c7991-118">Lai iegūtu papildinformāciju, skatiet rakstu kā paziņot [par atbalstu kontrolētajiem savienojumiem ar publiskajām mapēm programmā Outlook](https://aka.ms/controlpf).</span><span class="sxs-lookup"><span data-stu-id="c7991-118">For more info, see [Announcing Support for Controlled Connections to Public Folders in Outlook](https://aka.ms/controlpf).</span></span>