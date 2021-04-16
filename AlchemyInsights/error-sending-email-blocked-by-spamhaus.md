---
title: Kļūda, nosūtot SpamHaus bloķētu e-pasta ziņojumu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 8b5ac1df0b6a07a475345235a8b4b555d6881147
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813731"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="91a21-102">Kļūda, nosūtot e-pasta ziņojumu. Klienta resursdators ir bloķēts, izmantojot Spamhaus</span><span class="sxs-lookup"><span data-stu-id="91a21-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="91a21-103">IP adrese, kas nosūtīja ziņojumu, ir bloķēto sūtītāju sarakstā, kas pieder [organizācijai Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="91a21-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="91a21-104">Spamhaus bloķēšanas iemesli ir šādi: uz apdraudējumoti konti, uz apdraudēti datori, kuros ir kopīga IP adrese, un interneta pakalpojumu sniedzēja (Internet Service Provider – ISP) politikas.</span><span class="sxs-lookup"><span data-stu-id="91a21-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="91a21-105">Iespējamie labojumi ir šādi:</span><span class="sxs-lookup"><span data-stu-id="91a21-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="91a21-106">Ja tiek bloķēti ienākošie ziņojumi, kur jūs kontrolēat avota e-pasta serveri, ir jānosaka iemesls un jānoņem bloks Spamhaus tīmekļa vietnē.</span><span class="sxs-lookup"><span data-stu-id="91a21-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="91a21-107">Ja tiek bloķēti ienākošie ziņojumi, kuru avota IP adrese pieder kādam citam: adreses īpašniekam jānoņem bloks Spamhaus tīmekļa vietnē.</span><span class="sxs-lookup"><span data-stu-id="91a21-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="91a21-108">Ja IP adrese ir politiku bloķēšanas sarakstā (Policy Block List - PBL), īpašnieks var piešķirt citu statisko IP adresi vai noņemt adresi no PBL.</span><span class="sxs-lookup"><span data-stu-id="91a21-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="91a21-109">Ja tiek bloķēti izejošie ziņojumi no jūsu domēna, kas savienots ar Microsoft, šo kļūdu varat saņemt, ja ziņojumi tiek maršrutīti, izmantojot trešās puses pakalpojumus.</span><span class="sxs-lookup"><span data-stu-id="91a21-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="91a21-110">Lai atrastu bloķētās IP adreses īpašnieku, varat izmantot WHOIS uzmeklēšanas rīku.</span><span class="sxs-lookup"><span data-stu-id="91a21-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
