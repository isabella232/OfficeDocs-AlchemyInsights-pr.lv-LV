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
ms.openlocfilehash: b6a8b2a1174f04a1e0ed0fdee9a954bb3bf108038f0804353d84755e490f5f47
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105359"
---
# <a name="troubleshooting-events-from-email"></a>Problēmu novēršana saistībā ar notikumiem no e-pasta

1. Pārbaude, vai pastkastei šis līdzeklis ir iespējots: **Get-EventsFromEmailConfiguration -Identity <mailbox>**

2. Pēc tam skatiet žurnālus "Notikumi no **e-pasta" Export-MailboxDiagnosticLogs <mailbox> -Component TimeProfile**

3. Žurnālos "Notikumi no e-pasta" atrodiet InternetMessageId, kas atbilst vienumam pastkastē.  

4. TrustScore nosaka, vai vienums ir pievienots vai nē. Notikumi tiks pievienoti tikai tad, ja TrustScore = "Trusted".

TrustScore nosaka rekvizīti SPF, Dkim vai Dmarc, kuri ir ziņojuma iesākumā.

Lai skatītu šos rekvizītus:

**Darbvirsmas Outlook**

- Atvērt vienumu
- File -> Properties -> Internet Headers

vai

**MFCMapi**

- Naviģēt uz vienumu iesūtnē
- Meklējiet PR_TRANSPORT_MESSAGE_HEADERS_W

Šie rekvizīti tiek noteikti un ierakstīti transporta un maršrutēšanas laikā. Lai novērstu citas problēmas, iespējams, būs jāseko transporta atbalsta dienestam par kļūmēm SPF, DKIM un.vai DMARC.