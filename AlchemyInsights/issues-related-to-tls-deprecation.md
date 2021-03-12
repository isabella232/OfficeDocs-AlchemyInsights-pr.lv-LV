---
title: Nevar nosūtīt/saņemt e-pastu uz/no Office 365, jo TLS 1,0 un TLS 1,1 deaktivizēšana
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9005383"
- "9275"
ms.openlocfilehash: 9927112608ae58751e43c1bf0592fbd4a7cf1a0e
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745014"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nevar nosūtīt/saņemt e-pastu uz/no Office 365, jo TLS 1,0 un TLS 1,1 deaktivizēšana

Kā apstiprinājis ziņojumu centra izlikšana MC229914, TLS 1,0 un TLS 1,1 novecošana sāka izpildīt Exchange Online pasta plūsmas galapunktus. Drīzumā Office 365 vairs nepieņems TLS 1,0 un TLS 1,1 e-pasta savienojumus no ārējiem avotiem. Turklāt Exchange Online nekad neizmantos TLS 1,0 vai 1,1, lai nosūtītu izejošo e-pastu. Ja saskaramies ar TLS 1,0 vai 1,1 atspējošanu, var rasties kāda no tālāk norādītajām kļūdām.

- Sūtītājs saņem NDR atlēciens-"421 4.4.2 savienojums tika pārtraukts SocketError dēļ"
- Kļūdas ziņojumu rindu skatītājā lokālajā serverī, kas sūta e-pastu virsniekam 365-' 421 4.4.2 savienojums ir pārtraukts SocketError dēļ '
- Nosūtot e-pasta [ziņojumu uz Office](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) 365-TLS sarunām neizdevās kļūdu SocketError.
- Kļūda nosūtīšanas vai saņemšanas savienotāja protokola žurnālfailā — 451 5.7.3 ir jāizdod STARTTLS komanda pirmais

Ja rodas kāda no iepriekš norādītajām kļūdām, lūdzu, pārliecinieties, vai serverim, kas sūta vai saņem e-pasta ziņojumu, ir iespējota TLS 1,2, pārbaudot šīs reģistra atslēgas:

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ klients] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ Server] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**

Ja veicat izmaiņas iepriekš minētajās reģistra atslēgās, lai iespējotu TLS 1,2, restartējiet serveri, lai izmaiņas stātos spēkā. Pārliecinieties arī, vai jums ir instalēti jaunākie Windows un Exchange atjauninājumi.

Papildinformāciju skatiet šeit:

- [Exchange Server TLS vadlīnijas, 1. daļa: sagatavošanās TLS 1,2 — Microsoft Tech Kopiena](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS vadlīniju 2. daļa: iespējojiet TLS 1,2 un identificējot klientus, kas to neizmanto — Microsoft Tech Kopiena](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Par e-pasta scenārijiem, ja nevar vienoties par TLS versijām, izmantojot Exchange Online-Microsoft Tech Community](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
