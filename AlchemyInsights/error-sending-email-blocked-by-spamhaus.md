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
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Kļūda, nosūtot e-pastu: klienta resursdatora bloķēts, izmantojot Spamhaus

Ziņojuma nosūtītā IP adrese ir bloķēto sarakstā, kas pieder [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Spamhaus Bloķētie iemesli ir kompromitēti konti, kompromitēti mehānismi, kas koplieto publisku IP adresi un interneta pakalpojumu sniedzēja (ISP) politikas. Iespējamie labojumi ir:
  
- Bloķētajiem ienākošajiem ziņojumiem, kur jūs kontrolējat avota e-pasta serveri, jums ir jānosaka cēlonis un jānoņem bloks no vietnes Spamhaus.

- Bloķētajiem ienākošajiem ziņojumiem, ja avota IP adrese pieder kādam citam, adreses īpašniekam ir jānoņem bloks no vietnes Spamhaus. Ja IP adrese ir politikas bloka sarakstā (PBL), īpašnieks var piešķirt citu statisko IP adresi vai noņemt adresi no PBL.

- Bloķēto izejošo ziņojumu no jūsu domēna savienots ar Microsoft, varat saņemt šo kļūdu, ja ziņojumi tiek maršrutēti caur 3rd Party pakalpojumu. Lai atrastu bloķēto IP adreses īpašnieku, varat izmantot WHOIS uzmeklēšanas rīku.
