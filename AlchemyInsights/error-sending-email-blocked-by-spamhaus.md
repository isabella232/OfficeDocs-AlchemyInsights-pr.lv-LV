---
title: Kļūda, nosūtot e-pasta ziņojumu ar SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: a0c2f4be0b2d8ba6fd3dadbdf306e6ce623ad380
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47783810"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="84c6b-102">Kļūda, nosūtot e-pastu: klienta resursdators bloķēts, izmantojot spamhaus</span><span class="sxs-lookup"><span data-stu-id="84c6b-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="84c6b-103">Ziņojuma nosūtīšanas IP adrese ir bloķēto sarakstā, kas pieder [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="84c6b-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="84c6b-104">Spamhaus bloķēšanas iemesli ir kompromitēti konti, apdraudēti datori, kuros tiek kopīgota publiskā IP adrese un interneta pakalpojumu sniedzēja (ISP) politikas.</span><span class="sxs-lookup"><span data-stu-id="84c6b-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="84c6b-105">Iespējamie labojumi ir šādi:</span><span class="sxs-lookup"><span data-stu-id="84c6b-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="84c6b-106">Bloķēto ienākošo ziņojumu vietā, kur jūs kontrolējat avota e-pasta serveri, ir jānosaka iemesls un jānoņem bloks spamhaus tīmekļa vietnē.</span><span class="sxs-lookup"><span data-stu-id="84c6b-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="84c6b-107">Bloķēto ienākošo ziņojumu gadījumā, kad avota IP adrese pieder kādai citai personai, adreses īpašniekam ir jānoņem bloks spamhaus tīmekļa vietnē.</span><span class="sxs-lookup"><span data-stu-id="84c6b-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="84c6b-108">Ja IP adrese ir sarakstā politikas bloķēšana (PBL), īpašnieks var piešķirt citu statisko IP adresi vai noņemt adresi no PBL.</span><span class="sxs-lookup"><span data-stu-id="84c6b-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="84c6b-109">Lai bloķētu izejošos ziņojumus no domēna, kas savienots ar Microsoft, varat saņemt šo kļūdu, ja ziņojumi tiek maršrutēti caur trešo personu pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="84c6b-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="84c6b-110">Varat izmantot WHOIS uzmeklēšanas rīku, lai atrastu bloķēto IP adrešu īpašnieku.</span><span class="sxs-lookup"><span data-stu-id="84c6b-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
