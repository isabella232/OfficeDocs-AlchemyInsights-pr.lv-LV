---
title: Sūtīt kā Microsoft 365 grupu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/19/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9003200"
ms.openlocfilehash: cfb4bd5ce59eeccdd0812d013b8a444aebeb1d4c
ms.sourcegitcommit: 9818d3c8e6b10f23244e51286e2463caf48fffd5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/21/2020
ms.locfileid: "46871940"
---
# <a name="send-as-microsoft-365-group"></a>Sūtīt kā Microsoft 365 grupu

Varat piešķirt sūtīšanas kā atļaujas, lai konkrētiem lietotājiem atļautu sūtīt ziņojumus kā Microsoft 365 grupu:  

1. Savienojuma izveide ar Exchange Online PowerShell.  

2. Palaidiet šādu komandu:  

    Pievienojumprogramma RecipientPermission `<GroupName>` - `<MailboxName>` AccessRights SendAs

Lai iegūtu papildinformāciju, skatiet rakstu [Atļaut dalībniekiem sūtīt vai sūtīt grupas vārdā](https://docs.microsoft.com/microsoft-365/admin/create-groups/allow-members-to-send-as-or-send-on-behalf-of-group?view=o365-worldwide).