---
title: Migrēšana no AIP uz MIP/vienotās etiķetes atbilstības centrā
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002278"
- "5114"
ms.openlocfilehash: 378c3f58f77db8b23682432c942cd4f9c3a392651ca6564528a635724ad66a25
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54000363"
---
# <a name="migration-from-aip-to-mipunified-labeling-in-the-compliance-center"></a>Migrēšana no AIP uz MIP/vienotās etiķetes atbilstības centrā

Lai migrētu no AIP etiķetēm uz vienoto uzlīmēšanu drošības un atbilstības centrā, rīkojieties šādi:

**Aizsardzības aktivizēšana no Azure portāla**

1. Ja vēl neesat to izdarījis, atveriet jaunu pārlūkprogrammas logu [un pierakstieties Azure portālā.](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#signing-in-to-the-azure-portal) Naviģējiet uz **Azure informācijas aizsardzības asmens stieņu.** Piemēram, centrmezgla izvēlnē noklikšķiniet uz **Visi pakalpojumi** un sāciet **rakstīt informācija** lodziņā Filtrs. Atlasiet **Azure informācijas aizsardzība**. Ja iepriekš neesat piekļuvis Azure informācijas aizsardzības asmenim, skatiet vienreizējās papildu darbības, lai šo asmeni pievienotu portālam. [](https://docs.microsoft.com/azure/information-protection/deploy-use/configure-policy#to-access-the-azure-information-protection-blade-for-the-first-time) Lai atvērtu Azure informācijas aizsardzības asmens stieņu, ir nepieciešams Azure informācijas aizsardzības [Premium vai](https://www.microsoft.com/cloud-platform/azure-information-protection-pricing) Office 365 plāns, kurā iekļauta tiesību pārvaldība. Ja jums ir kāds no šiem abonementiem, bet tiek parādīts ziņojums, ka nevar atrast derīgu abonementu, sazinieties ar [Microsoft](https://docs.microsoft.com/azure/information-protection/get-started/information-support#to-contact-microsoft-support) atbalsta dienestu vai izmantojiet standarta atbalsta kanālus.

2. Atrodiet **izvēlnes opciju** Pārvaldība un atlasiet Aizsardzība **aktivizācija**. Noklikšķiniet **uz** Aktivizēt un pēc tam apstipriniet savu darbību. Kad aktivizācija ir pabeigta, informācijas joslā ir redzams, ka **aktivizēšana ir sekmīgi pabeigta.**

**Azure informācijas aizsardzības etiķešu migrēšana Office 365 drošības & centrā**

1. Pārliecinieties, vai esat pieteicies kā lietotājs ar globālā administratora atļauju.

2. Naviģējiet uz **Azure informācijas aizsardzības asmens stieņu.**

3. Izvēlnes **opcijā** Pārvaldīt atlasiet **Vienotā etiķetēšana**.

4. Azure Informācijas **aizsardzības vietnē — vienotās uzlīmju asmensmens** nosaukums noklikšķiniet uz **Aktivizēt** un izpildiet tiešsaistes norādījumus.

**Piezīme.** Pārliecinieties, vai jums ir nepieciešamās atļaujas, pirms aktivizējot & atbilstības centra migrāciju. Papildinformāciju skatiet šajos rakstos:

1. [Vai jums ir jābūt globālajam administratoram, lai konfigurētu Azure informācijas aizsardzību, vai vai varu deleģēt citiem administratoriem?](https://docs.microsoft.com/azure/information-protection/faqs#do-you-need-to-be-a-global-admin-to-configure-azure-information-protection-or-can-i-delegate-to-other-administrators)

2. [Svarīga informācija par administratīvajām lomām pēc migrēšanas uz & atbilstības centru.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels#important-information-about-administrative-roles)

Papildinformāciju par AIP uz vienoto uzlīmju migrāciju uz drošības un atbilstības centru skatiet rakstā [Etiķešu migrēšana.](https://docs.microsoft.com/azure/information-protection/configure-policy-migrate-labels)
