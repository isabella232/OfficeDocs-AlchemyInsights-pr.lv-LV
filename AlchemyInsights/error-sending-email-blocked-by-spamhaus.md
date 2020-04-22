---
title: Kļūda, nosūtot e-pastu bloķēts SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "255"
- "3100003"
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: 3ff4f7a155fe74f5b42a1bd43e67ef0a751d7fbd
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43714265"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a><span data-ttu-id="0ae36-102">Kļūda, nosūtot e-pastu: klienta resursdatora bloķēts, izmantojot Spamhaus</span><span class="sxs-lookup"><span data-stu-id="0ae36-102">Error sending email: Client host blocked using Spamhaus</span></span>

<span data-ttu-id="0ae36-103">Ziņojuma nosūtītā IP adrese ir bloķēto sarakstā, kas pieder [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span><span class="sxs-lookup"><span data-stu-id="0ae36-103">The IP address that sent the message is on a block list owned by [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245).</span></span> <span data-ttu-id="0ae36-104">Spamhaus Bloķētie iemesli ir kompromitēti konti, kompromitēti mehānismi, kas koplieto publisku IP adresi un interneta pakalpojumu sniedzēja (ISP) politikas.</span><span class="sxs-lookup"><span data-stu-id="0ae36-104">Reasons for being blocked by Spamhaus include compromised accounts, compromised machines sharing a public IP address, and Internet Service Provider (ISP) policies.</span></span> <span data-ttu-id="0ae36-105">Iespējamie labojumi ir:</span><span class="sxs-lookup"><span data-stu-id="0ae36-105">Possible fixes are:</span></span>
  
- <span data-ttu-id="0ae36-106">Bloķētajiem ienākošajiem ziņojumiem, kur jūs kontrolējat avota e-pasta serveri, jums ir jānosaka cēlonis un jānoņem bloks no vietnes Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="0ae36-106">For blocked inbound messages where you control the source email server, you need to determine the cause and remove the block from the Spamhaus website.</span></span>

- <span data-ttu-id="0ae36-107">Bloķētajiem ienākošajiem ziņojumiem, ja avota IP adrese pieder kādam citam, adreses īpašniekam ir jānoņem bloks no vietnes Spamhaus.</span><span class="sxs-lookup"><span data-stu-id="0ae36-107">For blocked inbound messages where the source IP address belongs to someone else, the address owner needs to remove the block from the Spamhaus website.</span></span> <span data-ttu-id="0ae36-108">Ja IP adrese ir politikas bloka sarakstā (PBL), īpašnieks var piešķirt citu statisko IP adresi vai noņemt adresi no PBL.</span><span class="sxs-lookup"><span data-stu-id="0ae36-108">If the IP address is on the Policy Block List (PBL), the owner can assign a different static IP address or remove the address from the PBL.</span></span>

- <span data-ttu-id="0ae36-109">Bloķēto izejošo ziņojumu no jūsu domēna savienots ar Microsoft, varat saņemt šo kļūdu, ja ziņojumi tiek maršrutēti caur 3rd Party pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="0ae36-109">For blocked outbound messages from your domain connected to Microsoft, you can receive this error if the messages are routed through a 3rd party service.</span></span> <span data-ttu-id="0ae36-110">Lai atrastu bloķēto IP adreses īpašnieku, varat izmantot WHOIS uzmeklēšanas rīku.</span><span class="sxs-lookup"><span data-stu-id="0ae36-110">You can use a WHOIS lookup tool to find the blocked IP address owner.</span></span>
