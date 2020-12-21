---
title: AggregateGroupMailbox pilns NDR saņemts e-pastam, kas nosūtīts uz Microsoft 365 grupu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/18/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004286"
- "7656"
ms.openlocfilehash: 9de09ab4cbd2f09648305b11da6273ed990907cf
ms.sourcegitcommit: 2ffdf6096de5608b117c6677d3cd7dd4c23ea024
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/18/2020
ms.locfileid: "49721916"
---
# <a name="aggregategroupmailbox-full-ndr-received-for-email-sent-to-microsoft-365-group"></a>AggregateGroupMailbox pilns NDR saņemts e-pastam, kas nosūtīts uz Microsoft 365 grupu

Izmantojiet šo EXO čaulas komandu, lai izveidotu Exchange transporta kārtulu, lai klusi nolaistu e-pasta ziņojumus, kas nosūtīti uz grupas pastkasti.

`New-TransportRule -SentTo @("AggregateGroupMailbox.A.201708181918@contoso.onmicrosoft.com") -DeleteMessage:$true -Name 'Agg1' -StopRuleProcessing:$false -Mode 'Enforce' -Comments '' -RuleErrorAction 'Ignore' -SenderAddressLocation 'Header'`

> [!NOTE]
> Savā nomniekā aizstājiet SMTP adresi programmā **SentTo** ar grupas pastkastes SMTP adresi. Jūs varat iegūt grupas pastkastes SMTP adresi no NDR saņemšanas.



