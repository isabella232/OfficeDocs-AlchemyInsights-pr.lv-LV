---
title: TeamViewer izmantošana, lai attāli administrētu Intune ierīces
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555241"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a>TeamViewer izmantošana, lai attāli administrētu Intune ierīces

Intune pārvaldītās ierīces var lietot attāli, izmantojot [TeamViewer](https://www.teamviewer.com/).

Lai administrētu Intune, izmantojot TeamViewer, veiciet tālāk norādītās darbības. 

Sāciet ar akreditācijas datu saņemšanu no TeamViewer, lai iestatītu TeamViewer savienotāju pakalpojumā Intune. Tādējādi administrators var ievadīt akreditācijas datus TeamViewer Connector UI sadaļā ierīces — vienreizēja darbība, lai izveidotu saiti starp Intune un TeamViewer pakalpojumu.

**1. daļa: sesijas sākšana ar attālo ierīci**

1. Sadaļā **visas ierīces**atlasiet ierīci, ar kuru vēlaties sākt attālo sesiju.
2. No **... Papildu**atlasiet **Jauna attālās palīdzības sesija**.
3. Atlasiet **Jā** , lai apstiprinātu, ka vēlaties izveidot attālo sesiju.
    Pēc tam, kad TeamViewer pakalpojums ir atzinis pieprasījumu "jauna Attālā sesija", tiks parādīta opcija **palaist attālo palīdzību** atbilstoši ierīces pārskata (vai Essentials) rūtij. Atlasiet **Skatīt vairāk** , lai izvērstu rūti un rādītu attālās palīdzības statusu.
4. Atlasiet **Sākt attālo sesiju** , lai sāktu sesiju administratora pusē.
5. Izvēlieties lejupielādēt TeamViewer bināro failu (Windows) un pēc tam atlasiet **palaist**.<br/>
    **Piezīmes** Varat ignorēt jebkuru tīmekļa pārlūkprogrammas lapu, kas atvērta TeamViewer tīmekļa vietnē.

6. Apstipriniet TeamViewer lietojumprogrammas pieprasījumu veikt izmaiņas ierīcē (tikai sistēmā Windows).
7. Tiek palaista programma TeamViewer, kurā ir iekļauts sesijas kods, lai autentificētu savienojumu ar attālo ierīci.

**2. daļa: ierīcē, kas paredzēta attālai sesijai**

1. Atveriet Intune uzņēmuma portālu.
2. Meklējiet paziņojuma karodziņu: "jūsu IT administrators pieprasa šīs ierīces vadību attālās palīdzības sesijai" un pēc tam atlasiet paziņojumu.
3. Izvēlieties lejupielādēt lietojumprogrammu TeamViewer vai apstiprināt programmas TeamViewer lejupielādi no lietojumprogrammu veikala un atlasiet **palaist**.
    **Piezīmes** Varat ignorēt jebkuru tīmekļa pārlūkprogrammas lapu, kas atvērta TeamViewer tīmekļa vietnē.

4. Apstipriniet TeamViewer lietojumprogrammas pieprasījumu veikt izmaiņas ierīcē (tikai sistēmā Windows).
5. Tiek palaista programma TeamViewer, kurā ir iekļauts sesijas kods, lai autentificētu savienojumu ar attālo ierīci.
6. Uznirstošais jautājums, vai vēlaties atļaut sesijas sākšanu.

**Piezīmes** TeamViewer pakalpojuma ģenerētie sesijas kodi ir tikai vienreizēja izmantošana. Ja pazaudējat savienojumu, veiciet tālāk norādītās darbības.

1. Attālajā ierīcē un administrēšanas darbstacijā izvērsiet lietojumprogrammas TeamViewer instanci.
2. Attālajā ierīcē izvērsiet uzņēmuma portālu.
3. Administrēšanas portālā sāciet jaunu attālās palīdzības sesiju.
4. Atkārtoti atveriet uzņēmuma portālu attālajā ierīcē, lai saņemtu jauno paziņojumu.
5. Lejupielādējiet un atveriet programmu TeamViewer gan attālajā ierīcē, gan administratora darbstacijā, kā iepriekš.