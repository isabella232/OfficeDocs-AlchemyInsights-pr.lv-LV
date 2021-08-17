---
title: Nevar nosūtīt/saņemt e-pastu uz/no Office 365 TLS 1.0 un TLS 1.1 atspējošanas dēļ
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
ms.openlocfilehash: 508e48fd0e46557de075f4752da017ab8cc326923a965350140e598f7f7cf557
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54054913"
---
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a>Nevar nosūtīt/saņemt e-pastu uz/no Office 365 TLS 1.0 un TLS 1.1 atspējošanas dēļ

Kā to apstiprina ziņojumu centra ziņa MC229914, TLS 1.0 un TLS 1.1 tika sākta pasta plūsmas galapunktu Exchange Online iesūtīšana. Drīzumā Office 365 neakceptēs TLS 1.0 un TLS 1.1 e-pasta savienojumus no ārējiem avotiem. Turklāt Exchange Online TLS 1.0 vai 1.1, lai nosūtītu izejošo e-pastu. Ja rodas problēmas TLS 1.0 vai 1.1 atspējošanas dēļ, iespējams, rodas kāda no tālāk redzamaajām kļūdām.

- Sūtītājs saņem NDR atlēcienu atpakaļ — '421 4.4.2 Savienojums tiek atmests SocketError dēļ
- Kļūda lokālā servera rindas skatītājā, kas sūta e-pasta ziņojumu palīgam 365 — "421 4.4.2 Connection dropped due to SocketError"
- Kļūda sūtītāja savienotāja [protokola žurnālā serverī,](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) kas nosūta e-pastu Office 365- TLS sarunas kļūme ar error SocketError
- Kļūda sūtīšanas vai saņemšanas savienotāja protokola žurnālā — "451 5.7.3 Vispirms ir jāiz izsniedz komandu STARTTLS"

Ja rodas kāda no iepriekš minētajām kļūdām, lūdzu, pārliecinieties, vai serverī, kas sūta vai saņem e-pasta ziņojumus, ir iespējots TLS 1.2, pārbaudot tālāk norādītās reģistra atslēgas.

[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**

Ja veicat izmaiņas iepriekš minētajās reģistra atslēgās, lai iespējotu TLS 1.2, restartējiet serveri, lai izmaiņas stātos spēkā. Pārliecinieties arī par to, vai jums ir Windows un Exchange atjauninājumi.

Papildinformāciju skatiet rakstā:

- [Exchange Server TLS norādījumi, 1. daļa. Gatavojieties darbam ar TLS 1.2 — Microsoft Tech community](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [Exchange Server TLS norādījumu 2. daļa. TLS 1.2 iespējošana un to klientu identificēšana, kuri tos nelieto — Microsoft tehnoloģiju kopiena](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [Informācija par e-pasta scenārijiem, ja par TLS versijām nevar vienojas ar Exchange Online Microsoft tehnoloģiju kopienu](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
