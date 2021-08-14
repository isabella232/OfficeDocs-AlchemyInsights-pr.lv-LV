---
title: Īpašnieks nevar izveidot apakšmapi, izmantojot Outlook
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
ms.openlocfilehash: 60190727e75c120ad3915da8b563b7f6b1a3238b46bb6e14cbf956365e1a84e0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54063131"
---
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Īpašnieks nevar izveidot apakšmapi, izmantojot Outlook

**Pastāv problēma, kur publisko mapju īpašnieki izveido apakšmapes, izmantojot Outlook. Problēma drīzumā tiks novērsta.**

Pagaidām izmantojiet kādu no šiem labojumiem:

1. Izmantojiet Outlook for MAC, lai izveidotu apakšmapi, jo problēma ietekmē tikai Outlook darbvirsmas logiem (visas versijas)
2. Vai administratoram ir jāizveido apakšmape, izmantojot EXO Shell vai EAC
3. Change the DefaultPublicFolderMailbox/EffectivePublicFolderMailbox on the user to other mailbox than the Content Mailbox for the folder causing issue  
    - *Set-Mailbox Lietotājs1 DefaultPublicFolderMailbox PubMBX3*
4. Uzgaidiet stundu, restartējiet Outlook klientu