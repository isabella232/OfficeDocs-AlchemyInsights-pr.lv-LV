---
title: Kļūda, nosūtot e-pastu bloķē SpamHaus
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 2/23/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: fa98ab4a-92eb-45e9-8d57-ad10fb123042
ms.openlocfilehash: a16c998d2f289ea2da52454819f6677c405381a1
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28300648"
---
# <a name="error-sending-email-client-host-blocked-using-spamhaus"></a>Kļūda, nosūtot e-pastu: klientu uzņēmēja bloķēta, izmantojot Spamhaus

IP adresi, kas nosūtījis ziņojumu ir bloķēto sarakstam pieder [Spamhaus](https://go.microsoft.com/fwlink/p/?linkid=123245). Bloķējis Spamhaus iemesli ietver apdraudēta kontu apdraudēta mašīnu koplietošanas publiska IP adrese un interneta pakalpojumu sniedzēja (ISP) politiku. Ir iespējami labojumi:
  
- Bloķēto ienākošajiem ziņojumiem uz Office 365, kur jūs kontrolēt avots e-pasta serverī, jums vajadzēs noteikt cēloni un bloka noņemšana no Spamhaus mājas lapā.
    
- Bloķētie ienākošajiem ziņojumiem uz Office 365 kur avota IP adresi pieder kādam citam, adrese īpašniekam ir bloka noņemšana no Spamhaus mājas lapā. Ja IP adrese ir politikas bloku saraksts (PBL), īpašnieks var piešķirt citu statisko IP adresi vai adresi izņemtu no PBL.
    
- Bloķēts izejošajiem ziņojumiem no jūsu biroja 365 domēnu, jūs varat saņemt šo kļūdu, ja ziņojumi tiek novirzīti caur 3rd puses pakalpojums. WHOIS pārlūkošanas rīku varat izmantot, lai atrastu bloķēto IP adreses īpašnieks.
    

