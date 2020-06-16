---
title: Īpašnieks nevar izveidot apakšmapi , izmantojot programmu Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: 2116bb837e4378ea29d7882df1d3010b3a4e0b1c
ms.sourcegitcommit: 936330b11fec49f6174eadea6c765bdf9e6ba784
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/12/2020
ms.locfileid: "44749137"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="65dbd-102">Īpašnieks nevar izveidot apakšmapi , izmantojot programmu Outlook</span><span class="sxs-lookup"><span data-stu-id="65dbd-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="65dbd-103">**Pastāv problēma ar publisko mapju īpašniekiem, kas veido apakšmapes, izmantojot programmu Outlook. Problēma tiks novērsta drīz.**</span><span class="sxs-lookup"><span data-stu-id="65dbd-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="65dbd-104">Tikmēr izmantojiet kādu no šiem veidiem:</span><span class="sxs-lookup"><span data-stu-id="65dbd-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="65dbd-105">Izmantojiet Outlook MAC izveidot apakšmapi, jo problēma ietekmē tikai Outlook darbvirsmas logiem (visas versijas)</span><span class="sxs-lookup"><span data-stu-id="65dbd-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="65dbd-106">Admin izveidot apakšmapi, izmantojot EXO Shell vai EAC</span><span class="sxs-lookup"><span data-stu-id="65dbd-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="65dbd-107">Mainīt DefaultPublicFolderMailbox/EffectivePublicFolderMailbox lietotājam uz citu pastkasti, nevis satura pastkasti mapei, kas izraisa problēmu</span><span class="sxs-lookup"><span data-stu-id="65dbd-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="65dbd-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="65dbd-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="65dbd-109">Pagaidiet stundu, restartējiet outlook klientu</span><span class="sxs-lookup"><span data-stu-id="65dbd-109">Wait for an hour, restart outlook client</span></span>