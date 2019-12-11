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
ms.openlocfilehash: a9305b175e1ca0b992c014a73705447d67e037bc
ms.sourcegitcommit: cbbd46fa9a32873c5446d9fd5a532cea0300b795
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/10/2019
ms.locfileid: "39959501"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="1b369-102">Programma Outlook nevar izveidot savienojumu ar publiskajām mapēm</span><span class="sxs-lookup"><span data-stu-id="1b369-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="1b369-103">Ja publiskās mapes piekļuve nedarbojas tikai dažiem lietotājiem, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="1b369-103">If public folder access isn't working for few users, try the following:</span></span>

<span data-ttu-id="1b369-104">Izveidot savienojumu ar EXO PowerShell un konfigurēt DefaultPublicFolderMailbox problēmu lietotāja kontu, lai saskaņotu vienu darba lietotāja kontu.</span><span class="sxs-lookup"><span data-stu-id="1b369-104">Connect to EXO PowerShell, and configure the DefaultPublicFolderMailbox on the problem user account to match one on a working user account.</span></span>

<span data-ttu-id="1b369-105">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="1b369-105">Example:</span></span>

<span data-ttu-id="1b369-106">Iegūt pastkasti WorkingUser | FT DefaultPublicFolderMailbox Efektivepublicfoldermailbox</span><span class="sxs-lookup"><span data-stu-id="1b369-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="1b369-107">Set-pastkaste ProblemUser-DefaultPublicFolderMailbox \<vērtību no iepriekšējās komandas></span><span class="sxs-lookup"><span data-stu-id="1b369-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="1b369-108">Uzgaidiet vismaz vienu stundu, lai izmaiņas stātos spēkā.</span><span class="sxs-lookup"><span data-stu-id="1b369-108">Wait at least one hour for the change to take effect.</span></span>