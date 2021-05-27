---
title: Defender galapunktu pārbaudes sensora statuss
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676344"
---
# <a name="defender-endpoint-check-sensor-status"></a>Defender galapunktu pārbaudes sensora statuss

Elements **Ierīces ar sensora** problēmām atrodas informācijas panelī Drošības operācijas. Šis elements sniedz informāciju par atsevišķas ierīces iespēju nodrošināt sensora datus un sazināties ar Defender galapunktu pakalpojumu. Tā ziņo, cik ierīcēm jāpievērš uzmanība un palīdz noteikt problemātiskās ierīces un rīkoties, lai novērstu zināmās problēmas.

Divi statusa indikatori elementā sniedz informāciju par to ierīču skaitu, par kuru nav pareizi ziņots pakalpojumam:

- **Nepareizi konfigurēts** Ierīces, kas var daļēji būt atskaišu sensora dati pakalpojumam Defender for Endpoint, un kurās var būt konfigurācijas kļūdas, kas ir jāizlabo.
- **Inactive** Ierīces, kuras pēdējā mēnesī ir pārtraukuši atskaišu rādīšanu pakalpojumam Defender for Endpoint vairāk nekā septiņas dienas.

Noklikšķinot uz jebkuras grupas, tiks iet novirzīts uz sarakstu Ierīces, kas filtrēts atbilstoši jūsu izvēlei. Sarakstā Ierīces varat filtrēt darbspējas stāvokļa sarakstu pēc šāda statusa:

- **Aktīvs** Ierīces, kas aktīvi ziņo Par pakalpojumu Defender for Endpoint.
- **Nepareizi konfigurēts** Ierīces, kas var daļēji būt atskaišu sensora dati Defender galapunktu pakalpojumam, bet kurās ir konfigurācijas kļūdas, kas ir jāizlabo. Nepareizi konfigurētām ierīcēm var būt viena vai vairākas tālāk minētās problēmas.

    - Bez sensora datiem — ierīces apturēs sensora datu sūtīšanu. No ierīces var tikt aktivizēti ierobežoti brīdinājumi.
    - Sakaru traucējumi — spējām sazināties ar ierīci ir traucējumi. Failu sūtīšana padziļinātai analīzei, failu bloķēšanai, ierīču izbrīvošana no tīkla un citas darbības, kam nepieciešama saziņa ar ierīci, var nedarboties.
- **Inactive** Ierīces, kuras pārtrauca atskaišu rādīšanu pakalpojumam Defender for Endpoint.

Varat lejupielādēt visu sarakstu CSV formātā, izmantojot eksportēšanas līdzekli.

Papildinformāciju skatiet rakstā [Sensora darbspējas stāvokļa pārbaude programmatūrā Microsoft Defender galapunktam](/microsoft-365/security/defender-endpoint/check-sensor-status).

Papildinformāciju par to, kas izraisīja ierīces neaktīvu vai nepareizi konfigurētu, skatiet rakstā Neaktīviem sensoriem labošana [programmatūrā Microsoft Defender galapunktam.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)
