---
title: Problēmu novēršanas notikumus no e-pasta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: e27589b7f6730036040b948b6275cef072fd8235
ms.sourcegitcommit: dc149ab45fbc2c974b54fb81156d2bc1b07017bb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44569138"
---
# <a name="troubleshooting-events-from-email"></a>Problēmu novēršanas notikumus no e-pasta

1. Pārbaudiet, vai ir iespējots līdzeklis pastkastes: **Get EventsFromEmailConfiguration-identitātes <mailbox> **

2. Pēc tam apskatiet "notikumus no e-pasta" žurnālus **Export-MailboxDiagnosticLogs <mailbox> -komponenta timeprofile**

3. Žurnālos "notikumi no e-pasta" atrodiet InternetMessageId, kas atbilst pastkastes vienumam.  

4. TrustScore nosaka, vai krājums ir pievienots vai nav. Notikumi tiks pievienoti tikai tad, ja TrustScore = "uzticams".

TrustScore nosaka ar SPF, DKIM vai Dmarc rekvizītiem, kas atrodas ziņojuma galvenē.

Lai skatītu šos rekvizītus:

**Desktop Outlook**

- Atveriet vienumu
- Fails-> rekvizīti-> interneta galvenes

Vai

**MFCMapi**

- Naviģējiet uz vienumu iesūtnē
- Meklēt PR_TRANSPORT_MESSAGE_HEADERS_W

Šie rekvizīti tiek noteikti un reģistrēti transportēšanas un maršrutēšanas laikā. Lai novērstu turpmāku problēmu novēršanu, var būt nepieciešams sekot līdzi transporta atbalstam par SPF, DKIM un. vai DMARC kļūmēm.