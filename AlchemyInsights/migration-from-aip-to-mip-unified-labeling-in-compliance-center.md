---
title: Migrēšana no AIP uz MIP/vienotās marķēšanas atbilstības centrā
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 7157eada10db2443f64fb7925f408359275d75eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47674333"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrēšana no AIP uz MIP/vienotās marķēšanas atbilstības centrā

Lai migrētu no AIP etiķetēm uz vienotu marķējumu drošības un atbilstības centrā, rīkojieties šādi:

**Aizsardzības aktivizēšana no Azure portāla**

1. Ja vēl neesat to izdarījis, atveriet jaunu pārlūkprogrammas logu un [pierakstieties Azure portālā](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal). Pārejiet uz **Azure informācijas aizsardzības** asmeni. Piemēram, izvēlnē centrmezgls noklikšķiniet uz **Visi pakalpojumi** un sāciet rakstīt **informāciju** filtra lodziņā. Atlasiet **Azure informācijas aizsardzība**. Ja iepriekš neesat piekļuvis Azure informācijas aizsardzības diskam, skatiet vienreizējās [papildu darbības](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) , lai šo disku pievienotu portālam. Lai atvērtu Azure Information Protection asmeni, jums ir jābūt [Azure Information Protection Premium plānam](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) vai Office 365 plānam, kurā ir iekļauta tiesību pārvaldība. Ja jums ir kāds no šiem abonementiem, bet redzat ziņojumu, ka derīgu abonementu nevar atrast, [sazinieties ar Microsoft atbalsta dienestu](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) vai izmantojiet savus standarta atbalsta kanālus.

2. Atrodiet **pārvaldības** izvēlnes opcijas un atlasiet **aizsardzības aktivizēšana**. Noklikšķiniet uz **Aktivizēt**un pēc tam apstipriniet savu darbību. Kad aktivizēšana ir pabeigta, informācijas joslā aktivizācija ir **sekmīgi pabeigta**.

**Azure informācijas aizsardzības etiķešu migrēšana uz Office 365 drošības & atbilstības centrs**

1. Pārliecinieties, vai esat pieteicies kā lietotājs, kuram ir globālās administratora atļaujas.

2. Pārejiet uz **Azure informācijas aizsardzības** asmeni.

3. Izvēlnē **Manage (pārvaldīt** ) atlasiet **vienota marķēšana**.

4. **Azure Information Protection — vienotās marķēšanas** asmens, noklikšķiniet uz **Aktivizēt** un izpildiet tiešsaistes instrukcijas.

**Piezīme**. Pārbaudiet, vai jums ir atbilstošas atļaujas, pirms aktivizējat drošības & atbilstības centra migrāciju. Lai iegūtu papildinformāciju, skatiet šos rakstus:

1. [Vai jums ir jābūt globālajam administratoram, lai konfigurētu Azure informācijas aizsardzību vai varu deleģēt citiem administratoriem?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Svarīga informācija par administratīvajām lomām pēc migrēšanas uz drošības & atbilstības centru.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Lai iegūtu papildinformāciju par to, kā AIP ir vienots pārzīmju migrēšanas uz drošības un atbilstības centru, skatiet rakstu [etiķešu migrēšana](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels).
