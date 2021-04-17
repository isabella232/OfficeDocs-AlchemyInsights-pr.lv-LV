---
title: Problēmu novēršana saistībā ar notikumiem no e-pasta
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000301"
- "5765"
ms.openlocfilehash: 2cea347f248a3b04873428946f1817657af04773
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51834846"
---
# <a name="troubleshooting-events-from-email"></a>Problēmu novēršana saistībā ar notikumiem no e-pasta

1. Pārbaude, vai pastkastei šis līdzeklis ir iespējots: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Pēc tam skatiet žurnālus "Notikumi no **e-pasta" Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Žurnālos "Notikumi no e-pasta" atrodiet InternetMessageId, kas atbilst vienumam pastkastē.  

4. TrustScore nosaka, vai vienums ir pievienots vai nē. Notikumi tiks pievienoti tikai tad, ja TrustScore = "Trusted".

TrustScore nosaka rekvizīti SPF, Dkim vai Dmarc, kuri ir ziņojuma iesākumā.

Lai skatītu šos rekvizītus:

**Outlook datora versija**

- Atvērt vienumu
- File -> Properties -> Internet Headers

vai

**MFCMapi**

- Naviģēt uz vienumu iesūtnē
- Meklējiet PR_TRANSPORT_MESSAGE_HEADERS_W

Šie rekvizīti tiek noteikti un ierakstīti transporta un maršrutēšanas laikā. Lai novērstu citas problēmas, iespējams, būs jāseko transporta atbalsta dienestam par kļūmēm SPF, DKIM un.vai DMARC.