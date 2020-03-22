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
ms.openlocfilehash: a579b89b68bfb8432adfe64b155803eda2c3b086
ms.sourcegitcommit: a3b42ee05224846327d353b48a8c67dab724f6eb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/21/2020
ms.locfileid: "42891756"
---
# <a name="outlook-cannot-connect-to-public-folders"></a><span data-ttu-id="00e09-102">Programma Outlook nevar izveidot savienojumu ar publiskajām mapēm</span><span class="sxs-lookup"><span data-stu-id="00e09-102">Outlook cannot connect to public folders</span></span>

<span data-ttu-id="00e09-103">Ja piekļuve publiskajai mapei nedarbojas dažiem lietotājiem, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="00e09-103">If public folder access isn't working for some users, try the following:</span></span>

<span data-ttu-id="00e09-104">Izveidot savienojumu ar EXO PowerShell un konfigurēt parametru DefaultPublicFolderMailbox problēmu lietotāja kontu, lai atbilstu parametru darba lietotāja kontu.</span><span class="sxs-lookup"><span data-stu-id="00e09-104">Connect to EXO PowerShell and configure the DefaultPublicFolderMailbox parameter on the problem user account to match the parameter on a working user account.</span></span>

<span data-ttu-id="00e09-105">Piemērs:</span><span class="sxs-lookup"><span data-stu-id="00e09-105">Example:</span></span>

<span data-ttu-id="00e09-106">Iegūt pastkasti WorkingUser | FT DefaultPublicFolderMailbox Efektivepublicfoldermailbox</span><span class="sxs-lookup"><span data-stu-id="00e09-106">Get-Mailbox WorkingUser | ft DefaultPublicFolderMailbox,EffectivePublicFolderMailbox</span></span>

<span data-ttu-id="00e09-107">Set-pastkaste ProblemUser-DefaultPublicFolderMailbox \<vērtību no iepriekšējās komandas></span><span class="sxs-lookup"><span data-stu-id="00e09-107">Set-Mailbox ProblemUser -DefaultPublicFolderMailbox \<value from previous command></span></span>

<span data-ttu-id="00e09-108">Uzgaidiet vismaz vienu stundu, lai izmaiņas stātos spēkā.</span><span class="sxs-lookup"><span data-stu-id="00e09-108">Wait at least one hour for the change to take effect.</span></span>

<span data-ttu-id="00e09-109">Ja problēma joprojām pastāv, lūdzu, veiciet [šīs darbības](https://aka.ms/pfcte) , lai novērstu publiskās mapes piekļuves problēmas, izmantojot programmu Outlook.</span><span class="sxs-lookup"><span data-stu-id="00e09-109">If the issue remains, please follow [this procedure](https://aka.ms/pfcte) to troubleshoot public folder access issues using Outlook.</span></span>