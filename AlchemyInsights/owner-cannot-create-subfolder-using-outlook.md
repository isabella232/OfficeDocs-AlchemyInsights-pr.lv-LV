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
# <a name="owner-cannot-create-sub-folder-using-outlook"></a>Īpašnieks nevar izveidot apakšmapi, izmantojot Outlook

**Ir neatrisināta problēma ar publisko mapju īpašniekiem, kas izveido apakšmapes, izmantojot programmu Outlook. Šī problēma tiks novērsta drīzumā.**

Vienlaikus izmantojiet kādu no tālāk norādītajiem risinājumiem.

1. Izmantojiet Outlook darbam ar MAC, lai izveidotu apakšmapi, jo problēma ietekmē tikai Outlook datora Windows (visas versijas)
2. Vai administrators izveido apakšmapi, izmantojot EXO Shell vai EAC
3. Mainiet lietotāja DefaultPublicFolderMailbox/EffectivePublicFolderMailbox uz citu pastkasti, nevis mapes satura pastkasti, kas izraisa problēmas  
    - *Iestatīt-pastkastes Lietotājs1 DefaultPublicFolderMailbox PubMBX3*
4. Uzgaidiet stundu un pēc tam restartējiet Outlook klientu