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
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Īpašnieks nevar izveidot apakšmapi, izmantojot programmu Outlook

**Pastāv problēma, kur publisko mapju īpašnieki izveido apakšmapes, izmantojot programmu Outlook. Problēma drīzumā tiks novērsta.**

Pagaidām izmantojiet kādu no šiem labojumiem:

1. Izmantojiet Outlook darbam ar MAC, lai izveidotu apakšmapi, jo problēma ietekmē tikai Outlook datora logus (visas versijas)
2. Vai administratoram ir jāizveido apakšmape, izmantojot EXO Shell vai EAC
3. Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue  
    - *Set-Mailbox Lietotājs1 DefaultPublicFolderMailbox PubMBX3*
4. Uzgaidiet stundu, restartējiet Outlook klientu