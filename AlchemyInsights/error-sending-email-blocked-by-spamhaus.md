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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Kļūda, nosūtot e-pasta ziņojumu. Klienta resursdators ir bloķēts, izmantojot Spamhaus

IP adrese, kas nosūtīja ziņojumu, ir bloķēto sūtītāju sarakstā, kas pieder [organizācijai Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Spamhaus bloķēšanas iemesli ir šādi: uz apdraudējumoti konti, uz apdraudēti datori, kuros ir kopīga IP adrese, un interneta pakalpojumu sniedzēja (Internet Service Provider – ISP) politikas. Iespējamie labojumi ir šādi:
  
- Ja tiek bloķēti ienākošie ziņojumi, kur jūs kontrolēat avota e-pasta serveri, ir jānosaka iemesls un jānoņem bloks Spamhaus tīmekļa vietnē.

- Ja tiek bloķēti ienākošie ziņojumi, kuru avota IP adrese pieder kādam citam: adreses īpašniekam jānoņem bloks Spamhaus tīmekļa vietnē. Ja IP adrese ir politiku bloķēšanas sarakstā (Policy Block List - PBL), īpašnieks var piešķirt citu statisko IP adresi vai noņemt adresi no PBL.

- Ja tiek bloķēti izejošie ziņojumi no jūsu domēna, kas savienots ar Microsoft, šo kļūdu varat saņemt, ja ziņojumi tiek maršrutīti, izmantojot trešās puses pakalpojumus. Lai atrastu bloķētās IP adreses īpašnieku, varat izmantot WHOIS uzmeklēšanas rīku.
