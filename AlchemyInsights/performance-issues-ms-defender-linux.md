---
title: Microsoft Defender galapunkta veiktspējas problēmas operētājsistēmā Linux
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/04/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11491"
- "9001464"
ms.openlocfilehash: 268f44640d3b2d8764133560d0cbf500eb4afd22
ms.sourcegitcommit: 8242a824491f64be48dfe81da09766920fbd7feb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/06/2021
ms.locfileid: "52794005"
---
# <a name="performance-issues-for-microsoft-defender-for-endpoint-on-linux"></a>Microsoft Defender galapunkta veiktspējas problēmas operētājsistēmā Linux

Šajā rakstā ir norādījumi, kā noteikt veiktspējas problēmas programmatūrai Microsoft Defender galapunktam operētājsistēmā Linux.

Vispirms pārbaudiet, vai problēma ir novērsta, izmantojot [jaunāko versiju.](/microsoft-365/security/defender-endpoint/linux-whatsnew) 

Lai sāktu izpēti, skatiet rakstu [Microsoft Defender galapunkta veiktspējas problēmu novēršana operētājsistēmā Linux.](/microsoft-365/security/defender-endpoint/linux-support-perf)

## <a name="exclusions"></a>Izņēmumi

Izņēmumi var palīdzēt mazināt veiktspējas problēmas. Pirms sākat darbu, pārskatiet izņēmumus, lai visi papildu riski būtu zināmi un dokumentēti.

Papildinformāciju skatiet rakstā [Microsoft Defender galapunkta izņēmumu konfigurēšana](/microsoft-365/security/defender-endpoint/linux-exclusions)un pārbaude operētājsistēmā Linux.

Ja ir vairāki faili& vai mapes izslēgt, un tie visi atrodas vienā vietā, iespējams, vieglāk ir izslēgt no kalnpunkta. Sākot ar februāra laidienu 101.22.80, varat izslēgt visu mountpoint.

Piemēram, ja /mnt/backup ir mountpoint, varat pievienot /mnt/backup izslēgšanas sarakstam, izpildot šo komandu:

`$ mdatp exclusion folder add –path /mnt/backup`

**Piezīme.** Pievienojot izņēmumus, tiek palielināts risks, ka ļaunprogrammatūra netiek noteikta, un tā ir jāapstrādā un ieviesīs rūpīgi.

## <a name="need-help"></a>Vai nepieciešama palīdzība?

Lai jums palīdzētu efektīvāk, apkopojiet diagnostikas datus pirms atbalsta pieteikuma atvēršanas.
