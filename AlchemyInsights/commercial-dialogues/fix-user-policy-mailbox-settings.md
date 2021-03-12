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
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50746731"
---
# <a name="fix-user-policymailbox-settings"></a>Lietotāja politikas/pastkastes iestatījumu labošana

Nevēlamais e-pasta iestatījumi pastkastē ietekmēja šo ziņojumu. Lai pārskatītu iestatījumus, veiciet tālāk norādītās darbības.

1. Palaidiet Exchange pārvaldības čaulu. Papildinformāciju skatiet rakstā [Exchange pārvaldības čaulas atvēršana](https://go.microsoft.com/fwlink/?linkid=2101432).
2. Izpildīt šo komandu (izmantojot lietotāja e-pasta adresi):  **Get-mailboxjunkmailconfiguration-Identity "user@domain.com"**
3. Pārbaudiet, vai sūtītāja e-pasta adrese ir daļa no **TrustedSendersAndDomains** vai **BlockedSendersAndDomains**. Ja e-pasta adrese ir kādā no sarakstiem, iespējams, tas ir jānoņem. Papildinformāciju skatiet rakstā [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).
