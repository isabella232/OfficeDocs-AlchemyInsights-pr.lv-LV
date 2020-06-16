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
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Īpašnieks nevar izveidot apakšmapi , izmantojot programmu Outlook

**Pastāv problēma ar publisko mapju īpašniekiem, kas veido apakšmapes, izmantojot programmu Outlook. Problēma tiks novērsta drīz.**

Tikmēr izmantojiet kādu no šiem veidiem:

1. Izmantojiet Outlook MAC izveidot apakšmapi, jo problēma ietekmē tikai Outlook darbvirsmas logiem (visas versijas)
2. Admin izveidot apakšmapi, izmantojot EXO Shell vai EAC
3. Mainīt DefaultPublicFolderMailbox/EffectivePublicFolderMailbox lietotājam uz citu pastkasti, nevis satura pastkasti mapei, kas izraisa problēmu  
    - *Set-Mailbox User1 DefaultPublicFolderMailbox PubMBX3*
4. Pagaidiet stundu, restartējiet outlook klientu