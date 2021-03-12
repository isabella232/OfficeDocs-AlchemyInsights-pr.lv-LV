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
# <a name="unable-to-sendreceive-email-tofrom-office-365-because-of-the-tls-10-and-tls-11-disablement"></a><span data-ttu-id="cd233-102">Nevar nosūtīt/saņemt e-pastu uz/no Office 365, jo TLS 1,0 un TLS 1,1 deaktivizēšana</span><span class="sxs-lookup"><span data-stu-id="cd233-102">Unable to send/receive email to/from Office 365 because of the TLS 1.0 and TLS 1.1 disablement</span></span>

<span data-ttu-id="cd233-103">Kā apstiprinājis ziņojumu centra izlikšana MC229914, TLS 1,0 un TLS 1,1 novecošana sāka izpildīt Exchange Online pasta plūsmas galapunktus.</span><span class="sxs-lookup"><span data-stu-id="cd233-103">As confirmed by the message center post MC229914, TLS 1.0 and TLS 1.1 deprecation started enforcing for Exchange Online mail flow endpoints.</span></span> <span data-ttu-id="cd233-104">Drīzumā Office 365 vairs nepieņems TLS 1,0 un TLS 1,1 e-pasta savienojumus no ārējiem avotiem.</span><span class="sxs-lookup"><span data-stu-id="cd233-104">Soon Office 365 will no longer accept TLS 1.0 and TLS 1.1 email connections from external sources.</span></span> <span data-ttu-id="cd233-105">Turklāt Exchange Online nekad neizmantos TLS 1,0 vai 1,1, lai nosūtītu izejošo e-pastu.</span><span class="sxs-lookup"><span data-stu-id="cd233-105">Also, Exchange Online will never use TLS 1.0 or 1.1 to send outbound email.</span></span> <span data-ttu-id="cd233-106">Ja saskaramies ar TLS 1,0 vai 1,1 atspējošanu, var rasties kāda no tālāk norādītajām kļūdām.</span><span class="sxs-lookup"><span data-stu-id="cd233-106">If you are facing issues because of TLS 1.0 or 1.1 disablement, you might experience one of the following errors-</span></span>

- <span data-ttu-id="cd233-107">Sūtītājs saņem NDR atlēciens-"421 4.4.2 savienojums tika pārtraukts SocketError dēļ"</span><span class="sxs-lookup"><span data-stu-id="cd233-107">Sender is getting NDR bounce back - '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="cd233-108">Kļūdas ziņojumu rindu skatītājā lokālajā serverī, kas sūta e-pastu virsniekam 365-' 421 4.4.2 savienojums ir pārtraukts SocketError dēļ '</span><span class="sxs-lookup"><span data-stu-id="cd233-108">Error in the Queue Viewer of On-Premises server that is sending email to Officer 365- '421 4.4.2 Connection dropped due to SocketError'</span></span>
- <span data-ttu-id="cd233-109">Nosūtot e-pasta [ziņojumu uz Office](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) 365-TLS sarunām neizdevās kļūdu SocketError.</span><span class="sxs-lookup"><span data-stu-id="cd233-109">Error in Send connector [Protocol log](https://docs.microsoft.com/exchange/mail-flow/connectors/protocol-logging) on the server sending email to Office 365- TLS negotiation failed with error SocketError</span></span>
- <span data-ttu-id="cd233-110">Kļūda nosūtīšanas vai saņemšanas savienotāja protokola žurnālfailā — 451 5.7.3 ir jāizdod STARTTLS komanda pirmais</span><span class="sxs-lookup"><span data-stu-id="cd233-110">Error in Send or receive connector protocol log - '451 5.7.3 Must issue a STARTTLS command first'</span></span>

<span data-ttu-id="cd233-111">Ja rodas kāda no iepriekš norādītajām kļūdām, lūdzu, pārliecinieties, vai serverim, kas sūta vai saņem e-pasta ziņojumu, ir iespējota TLS 1,2, pārbaudot šīs reģistra atslēgas:</span><span class="sxs-lookup"><span data-stu-id="cd233-111">If you experience any of the above errors, please make sure the server that is sending or receiving email has TLS 1.2 enabled by checking the following registry keys-</span></span>

<span data-ttu-id="cd233-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ klients] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1,2 \ Server] **"DisabledByDefault" = DWORD: 00000000 "Enabled" = DWORD: 00000001**</span><span class="sxs-lookup"><span data-stu-id="cd233-112">[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2] [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Client] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001** [HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\SecurityProviders\SCHANNEL\Protocols\TLS 1.2\Server] **"DisabledByDefault"=dword:00000000 "Enabled"=dword:00000001**</span></span>

<span data-ttu-id="cd233-113">Ja veicat izmaiņas iepriekš minētajās reģistra atslēgās, lai iespējotu TLS 1,2, restartējiet serveri, lai izmaiņas stātos spēkā.</span><span class="sxs-lookup"><span data-stu-id="cd233-113">If you make any change in the above registry keys to enable TLS 1.2, restart the server for the changes to take effect.</span></span> <span data-ttu-id="cd233-114">Pārliecinieties arī, vai jums ir instalēti jaunākie Windows un Exchange atjauninājumi.</span><span class="sxs-lookup"><span data-stu-id="cd233-114">Also make sure you have the latest Windows and Exchange updates installed.</span></span>

<span data-ttu-id="cd233-115">Papildinformāciju skatiet šeit:</span><span class="sxs-lookup"><span data-stu-id="cd233-115">For more information, see:</span></span>

- [<span data-ttu-id="cd233-116">Exchange Server TLS vadlīnijas, 1. daļa: sagatavošanās TLS 1,2 — Microsoft Tech Kopiena</span><span class="sxs-lookup"><span data-stu-id="cd233-116">Exchange Server TLS guidance, part 1: Getting Ready for TLS 1.2 - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-1-getting-ready-for-tls-1-2/ba-p/607649)
- [<span data-ttu-id="cd233-117">Exchange Server TLS vadlīniju 2. daļa: iespējojiet TLS 1,2 un identificējot klientus, kas to neizmanto — Microsoft Tech Kopiena</span><span class="sxs-lookup"><span data-stu-id="cd233-117">Exchange Server TLS guidance Part 2: Enabling TLS 1.2 and Identifying Clients Not Using It - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/exchange-server-tls-guidance-part-2-enabling-tls-1-2-and/ba-p/607761)
- [<span data-ttu-id="cd233-118">Par e-pasta scenārijiem, ja nevar vienoties par TLS versijām, izmantojot Exchange Online-Microsoft Tech Community</span><span class="sxs-lookup"><span data-stu-id="cd233-118">Understanding email scenarios if TLS versions cannot be agreed on with Exchange Online - Microsoft Tech Community</span></span>](https://techcommunity.microsoft.com/t5/exchange-team-blog/understanding-email-scenarios-if-tls-versions-cannot-be-agreed/ba-p/2065089)
