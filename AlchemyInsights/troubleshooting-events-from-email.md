---
title: Problēmu novēršanas notikumi no e-pasta
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 9efd969e3e639c2679b0768c4a0fd045916b00d1
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658741"
---
# <a name="troubleshooting-events-from-email"></a>Problēmu novēršanas notikumi no e-pasta

1. Pārbaudiet, vai pastkastei ir iespējots līdzeklis: **Get-EventsFromEmailConfiguration-Identity <mailbox> **

2. Pēc tam aplūkojiet notikumus no e-pasta žurnāliem **, eksportējot-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Žurnālos "notikumi no e-pasta" atrodiet InternetMessageId, kas atbilst pastkastes elementam.  

4. TrustScore nosaka, vai vienums ir pievienots. Notikumi tiks pievienoti tikai tad, ja TrustScore = "uzticams".

TrustScore nosaka SPF, DKIM vai Dmarc rekvizīti, kas atrodas ziņojuma iesākumā.

Lai skatītu šos rekvizītus:

**Darbvirsmas Outlook**

- Atvērt vienumu
- Failu-> rekvizīti — > interneta galvenes

vai

**MFCMapi**

- Pārvietošanās uz vienumu iesūtnē
- PR_TRANSPORT_MESSAGE_HEADERS_W meklēšana

Šos rekvizītus nosaka un reģistrē transportēšanas un maršrutēšanas laikā. Lai veiktu citas darbības problēmu novēršanai, iespējams, jums būs jāseko transporta atbalstam attiecībā uz SPF, DKIM un DMARC.