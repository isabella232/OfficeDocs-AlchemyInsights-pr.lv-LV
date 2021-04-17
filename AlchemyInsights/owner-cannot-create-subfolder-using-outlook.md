---
title: Īpašnieks nevar izveidot apakšmapi, izmantojot programmu Outlook
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5884"
- "3500007"
ms.openlocfilehash: b2ab7b60bc521fd28d68333bb963528f7b9e05f2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836142"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="f6c5f-102">Īpašnieks nevar izveidot apakšmapi, izmantojot programmu Outlook</span><span class="sxs-lookup"><span data-stu-id="f6c5f-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="f6c5f-103">**Pastāv problēma, kur publisko mapju īpašnieki izveido apakšmapes, izmantojot programmu Outlook. Problēma drīzumā tiks novērsta.**</span><span class="sxs-lookup"><span data-stu-id="f6c5f-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="f6c5f-104">Pagaidām izmantojiet kādu no šiem labojumiem:</span><span class="sxs-lookup"><span data-stu-id="f6c5f-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="f6c5f-105">Izmantojiet Outlook darbam ar MAC, lai izveidotu apakšmapi, jo problēma ietekmē tikai Outlook datora logus (visas versijas)</span><span class="sxs-lookup"><span data-stu-id="f6c5f-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="f6c5f-106">Vai administratoram ir jāizveido apakšmape, izmantojot EXO Shell vai EAC</span><span class="sxs-lookup"><span data-stu-id="f6c5f-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="f6c5f-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span><span class="sxs-lookup"><span data-stu-id="f6c5f-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="f6c5f-108">*Set-Mailbox Lietotājs1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="f6c5f-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="f6c5f-109">Uzgaidiet stundu, restartējiet Outlook klientu</span><span class="sxs-lookup"><span data-stu-id="f6c5f-109">Wait for an hour, restart outlook client</span></span>