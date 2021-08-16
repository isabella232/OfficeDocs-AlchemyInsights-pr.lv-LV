---
title: Lietotāja politikas/pastkastes iestatījumu labošana
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: fecc52bea66e0aed709a8995d2509f4432c09482459aa575d29e4c7551375211
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54034725"
---
# <a name="fix-user-policymailbox-settings"></a>Lietotāja politikas/pastkastes iestatījumu labošana

Nevēlamā e-pasta iestatījumi pastkastē, kurā tika ietekmēts šis ziņojums. Lai pārskatītu iestatījumus, rīkojieties šādi:

1. Palaidiet Exchange pārvaldības čaulu. Papildinformāciju skatiet rakstā [Pārvaldības čaulas Exchange atvēršana.](https://go.microsoft.com/fwlink/?linkid=2101432)
2. Izpildiet šo komandu (izmantojot lietotāja e-pasta adresi):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**
3. Pārbaudiet, vai sūtītāja e-pasta adrese ir daļa no **TrustedSendersAndDomains** vai **BlockedSendersAndDomains**. Ja e-pasta adrese ir kādā no sarakstiem, iespējams, tā ir jānoņem. Papildinformāciju skatiet [rakstā Set-MailboxJunkEmailConfiguration.](https://go.microsoft.com/fwlink/?linkid=2101047)
