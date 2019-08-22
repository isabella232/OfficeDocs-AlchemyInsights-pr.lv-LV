---
title: Kļūda, nosūtot e-pastu bloķē SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 39213f6f1b96c2bef9ea071f43c38766debf64d1
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36527144"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="39710-102">Kļūda, nosūtot e-pastu: klientu uzņēmēja bloķēta, izmantojot Spamhaus</span><span class="sxs-lookup"><span data-stu-id="39710-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="39710-103">IP adresi, kas nosūtījis ziņojumu ir bloķēto sarakstam pieder [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="39710-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="39710-104">Bloķējis Spamhaus iemesli ietver apdraudēta kontu apdraudēta mašīnu koplietošanas publiska IP adrese un interneta pakalpojumu sniedzēja (ISP) politiku.</span><span class="sxs-lookup"><span data-stu-id="39710-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="39710-105">Ir iespējami labojumi:</span><span class="sxs-lookup"><span data-stu-id="39710-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="39710-106">Bloķēto ienākošajiem ziņojumiem uz Office 365, kur jūs kontrolēt avots e-pasta serverī, jums vajadzēs noteikt cēloni un bloka noņemšana no Spamhaus mājas lapā.</span><span class="sxs-lookup"><span data-stu-id="39710-106">For blocked inbound messages to Office 365 where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="39710-107">Bloķētie ienākošajiem ziņojumiem uz Office 365 kur avota IP adresi pieder kādam citam, adrese īpašniekam ir bloka noņemšana no Spamhaus mājas lapā.</span><span class="sxs-lookup"><span data-stu-id="39710-107">For blocked inbound messages to Office 365 where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="39710-108">Ja IP adrese ir politikas bloku saraksts (PBL), īpašnieks var piešķirt citu statisko IP adresi vai adresi izņemtu no PBL.</span><span class="sxs-lookup"><span data-stu-id="39710-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="39710-109">Bloķēts izejošajiem ziņojumiem no jūsu biroja 365 domēnu, jūs varat saņemt šo kļūdu, ja ziņojumi tiek novirzīti caur 3rd puses pakalpojums.</span><span class="sxs-lookup"><span data-stu-id="39710-109">For blocked outbound messages from your Office 365 domain, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="39710-110">WHOIS pārlūkošanas rīku varat izmantot, lai atrastu bloķēto IP adreses īpašnieks.</span><span class="sxs-lookup"><span data-stu-id="39710-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
