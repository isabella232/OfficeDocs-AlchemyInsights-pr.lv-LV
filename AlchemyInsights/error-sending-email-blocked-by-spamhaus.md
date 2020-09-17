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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Kļūda, nosūtot e-pastu: klienta resursdators bloķēts, izmantojot spamhaus

Ziņojuma nosūtīšanas IP adrese ir bloķēto sarakstā, kas pieder [spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Spamhaus bloķēšanas iemesli ir kompromitēti konti, apdraudēti datori, kuros tiek kopīgota publiskā IP adrese un interneta pakalpojumu sniedzēja (ISP) politikas. Iespējamie labojumi ir šādi:
  
- Bloķēto ienākošo ziņojumu vietā, kur jūs kontrolējat avota e-pasta serveri, ir jānosaka iemesls un jānoņem bloks spamhaus tīmekļa vietnē.

- Bloķēto ienākošo ziņojumu gadījumā, kad avota IP adrese pieder kādai citai personai, adreses īpašniekam ir jānoņem bloks spamhaus tīmekļa vietnē. Ja IP adrese ir sarakstā politikas bloķēšana (PBL), īpašnieks var piešķirt citu statisko IP adresi vai noņemt adresi no PBL.

- Lai bloķētu izejošos ziņojumus no domēna, kas savienots ar Microsoft, varat saņemt šo kļūdu, ja ziņojumi tiek maršrutēti caur trešo personu pakalpojumu. Varat izmantot WHOIS uzmeklēšanas rīku, lai atrastu bloķēto IP adrešu īpašnieku.
