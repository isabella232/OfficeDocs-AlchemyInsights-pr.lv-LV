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
# <a name="sender-does-not-receive-email-sent-to-microsoft-365-group"></a>Sūtītājs nesaņem e-pasta ziņojumus, kas nosūtīti uz Microsoft 365 grupu

Pēc noklusējuma e-pasta ziņojuma sūtītājs Microsoft 365 grupai nesaņem ziņojuma kopiju savā iesūtnē pat tad, ja sūtītājs ir grupas dalībnieks.

Izmantojiet šo EXO PowerShell komandu, lai ļautu sūtītājam saņemt katra e-pasta ziņojuma kopiju, ko tie nosūta uz Microsoft 365 grupu:  

`Set-MailboxMessageConfiguration <MailboxName> -EchoGroupMessageBackToSubscribedSender $True`  

Lai iespējotu visu pastkastu iestatījumu vienlaikus:

`Get-Mailbox -ResultSize Unlimited | ForEach {Set-MailboxMessageConfiguration -Identity $_.UserPrincipalName -EchoGroupMessageBackToSubscribedSender $true}` 

**Piezīmes** Izmaiņas šajā iestatījumā ir nepieciešamas līdz pat stundai, lai tās stātos spēkā.