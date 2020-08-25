---
title: Sūtītājs nesaņem e-pasta ziņojumus, kas nosūtīti uz Microsoft 365 grupu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/20/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: b3b438e17c35f18289d3e9c3ca89d16a6f2a065f
ms.sourcegitcommit: dcca0df53f9194f406cf3a5f6b046cb33a0a5b03
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871938"
---
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a><span data-ttu-id="cbd92-102">Sūtītājs nesaņem e-pasta ziņojumus, kas nosūtīti uz Microsoft 365 grupu</span><span class="sxs-lookup"><span data-stu-id="cbd92-102">Sender does not receive email sent to Microsoft 365 group</span></span>

<span data-ttu-id="cbd92-103">Pēc noklusējuma e-pasta ziņojuma sūtītājs Microsoft 365 grupai nesaņem ziņojuma kopiju savā iesūtnē pat tad, ja sūtītājs ir grupas dalībnieks.</span><span class="sxs-lookup"><span data-stu-id="cbd92-103">By default, the sender of an email message to a Microsoft 365 group doesn't receive a copy of the message in their Inbox, even if the sender is a member of the group.</span></span>

<span data-ttu-id="cbd92-104">Izmantojiet šo EXO PowerShell komandu, lai ļautu sūtītājam saņemt katra e-pasta ziņojuma kopiju, ko tie nosūta uz Microsoft 365 grupu:</span><span class="sxs-lookup"><span data-stu-id="cbd92-104">Use this EXO PowerShell command to allow the sender to receive a copy of each email they send to the Microsoft 365 group:</span></span>  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

<span data-ttu-id="cbd92-105">Lai iespējotu visu pastkastu iestatījumu vienlaikus:</span><span class="sxs-lookup"><span data-stu-id="cbd92-105">To enable the setting for all mailboxes at once:</span></span>

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

<span data-ttu-id="cbd92-106">**Piezīmes** Izmaiņas šajā iestatījumā ir nepieciešamas līdz pat stundai, lai tās stātos spēkā.</span><span class="sxs-lookup"><span data-stu-id="cbd92-106">**Note** Changes to this setting take up to an hour to take effect.</span></span>