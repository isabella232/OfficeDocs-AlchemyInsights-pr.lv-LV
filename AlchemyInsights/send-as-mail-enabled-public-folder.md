---
title: Publiskas mapes nosūtīšana programmā EXO
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1956"
- "3500007"
ms.openlocfilehash: ed62c6d7db0ae532f806ce4fdc48f42623bcd545
ms.sourcegitcommit: 1fb324fd156008e77b7e2008af4b3dc1c0d0ea3e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/13/2020
ms.locfileid: "48461962"
---
# <a name="sendas-mail-enabled-public-folder"></a><span data-ttu-id="b70e8-102">SendAs pasta iespējota publiskā mape</span><span class="sxs-lookup"><span data-stu-id="b70e8-102">SendAs Mail Enabled Public Folder</span></span>

<span data-ttu-id="b70e8-103">Tālāk sniegtajā piemērā tiek piešķirti "nosūtīt kā" atļaujas pasta publiskajai mapei NewPF1 lietotājam.</span><span class="sxs-lookup"><span data-stu-id="b70e8-103">The following example assigns "Send As" permissions for the mail-enabled public folder NewPF1 to the user Jason.</span></span>

<span data-ttu-id="b70e8-104">Add-RecipientPermission-Identity "NewPF1"-pilnvarnieks "Jason"-AccessRights "SendAs"</span><span class="sxs-lookup"><span data-stu-id="b70e8-104">Add-RecipientPermission -Identity 'NewPF1' -Trustee "Jason" -AccessRights 'SendAs'</span></span>

<span data-ttu-id="b70e8-105">Detalizētu informāciju par sintaksi un parametriem skatiet rakstā [piešķirt "Sūtīt kā" vai "Sūtīt vārdā" atļaujas pasta publiskajām mapēm](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span><span class="sxs-lookup"><span data-stu-id="b70e8-105">For detailed syntax and parameter information see [Assign "Send As" or "Send on Behalf" permissions for mail-enabled public folders](https://docs.microsoft.com/exchange/collaboration-exo/public-folders/assign-permissions-mail-enabled-pfs).</span></span>

