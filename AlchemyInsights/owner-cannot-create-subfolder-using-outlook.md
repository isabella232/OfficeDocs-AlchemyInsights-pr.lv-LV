---
title: Īpašnieks nevar izveidot apakšmapi, izmantojot Outlook
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: 9590f780cffeaf644733752c763e04d748b1b39e
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47665725"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a><span data-ttu-id="9558f-102">Īpašnieks nevar izveidot apakšmapi, izmantojot Outlook</span><span class="sxs-lookup"><span data-stu-id="9558f-102">Owner cannot create sub-folder using Outlook</span></span>

<span data-ttu-id="9558f-103">**Ir neatrisināta problēma ar publisko mapju īpašniekiem, kas izveido apakšmapes, izmantojot programmu Outlook. Šī problēma tiks novērsta drīzumā.**</span><span class="sxs-lookup"><span data-stu-id="9558f-103">**There's an ongoing issue with public folder owners creating subfolders using Outlook. The issue will be fixed soon.**</span></span>

<span data-ttu-id="9558f-104">Vienlaikus izmantojiet kādu no tālāk norādītajiem risinājumiem.</span><span class="sxs-lookup"><span data-stu-id="9558f-104">Meanwhile, use one of the following workarounds:</span></span>

1. <span data-ttu-id="9558f-105">Izmantojiet Outlook darbam ar MAC, lai izveidotu apakšmapi, jo problēma ietekmē tikai Outlook datora Windows (visas versijas)</span><span class="sxs-lookup"><span data-stu-id="9558f-105">Use Outlook for MAC to create the subfolder as the issue impacts only Outlook for desktop windows (all versions)</span></span>
2. <span data-ttu-id="9558f-106">Vai administrators izveido apakšmapi, izmantojot EXO Shell vai EAC</span><span class="sxs-lookup"><span data-stu-id="9558f-106">Have admin create the subfolder using EXO Shell or EAC</span></span>
3. <span data-ttu-id="9558f-107">Mainiet lietotāja DefaultPublicFolderMailbox/EffectivePublicFolderMailbox uz citu pastkasti, nevis mapes satura pastkasti, kas izraisa problēmas</span><span class="sxs-lookup"><span data-stu-id="9558f-107">Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue</span></span>  
    - <span data-ttu-id="9558f-108">*Iestatīt-pastkastes Lietotājs1 DefaultPublicFolderMailbox PubMBX3*</span><span class="sxs-lookup"><span data-stu-id="9558f-108">*Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*</span></span>
4. <span data-ttu-id="9558f-109">Uzgaidiet stundu un pēc tam restartējiet Outlook klientu</span><span class="sxs-lookup"><span data-stu-id="9558f-109">Wait for an hour, restart outlook client</span></span>