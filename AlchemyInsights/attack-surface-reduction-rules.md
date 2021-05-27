---
title: Uzbrukumu trūkšanas samazināšanas kārtulas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676435"
---
# <a name="attack-surface-reduction-rules"></a>Uzbrukumu trūkšanas samazināšanas kārtulas

Izslēdzot failus vai mapes, var ievērojami samazināt uzbrukumu virsmas samazināšanas kārtulu nodrošināto aizsardzību. Failus, kurus kārtula būtu bloķējusi, ir atļauts palaist, un atskaite vai notikums netiek ierakstīts. Izņēmumi attiecas uz visām kārtulām, kas atļauj izņēmumus.

ASR izņēmumiem ir jāizmanto tā pati sintakse, kas pretvīrusu programmatūra Microsoft Defender izslēgšanai. Detalizētu informāciju skatiet rakstā [Izņēmumu konfigurēšana un pārbaude, lai pretvīrusu programmatūra Microsoft Defender skenēšanu.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus) Lai izvairītos no problēmām, [pārskatiet biežāk sastopamās kļūdas, kas rodas, definējot izņēmumus.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)

Ne visas ASR kārtulas atbalsta izņēmumus. Lai pārbaudītu, vai jūsu kārtula atbalsta izņēmumus, skatiet tabulu [Uzbrukumu trūkšanas kārtulas.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

## <a name="attack-surface-reduction-rules"></a>Uzbrukumu trūkšanas samazināšanas kārtulas

Jūsu organizācijas uzbrukuma virsma ietver visas vietas, kur uzbrucējs var uz apdraudējumēt organizācijas ierīces vai tīklus. Samazinot uzbrukumu virsmu, tiek aizsargātas organizācijas ierīces un tīkls, kas uzbrukumiem atstāj mazāk veidu, kā veikt uzbrukumus. Varat konfigurēt uzbrukumu surface samazināšanas kārtulas programmatūrā Microsoft Defender galapunktam.

Papildinformāciju skatiet rakstā:

- [Kartēt ASR kārtulas GUID uz nosaukumu](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- ASR noteikumu prasības:
    - [Windows 10 Pro, versija 1709 vai jaunāka](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows 10 Enterprise, versija 1709 vai jaunāka](/windows/whats-new/whats-new-windows-10-version-1709)
    - [Windows Server, versija 1803 (pusgada kanāls) vai jaunāka versija](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a>Pareizas izslēgšanas identificēšana, ko vēlaties lietot

1. Meklējiet eventID 1121 vai 1122 Microsoft-Windows-Windows Defender/darbības žurnālā.

1. Novērtējiet bloka scenāriju un kontekstu un apstipriniet, ka šo scenāriju nepieciešams atbloķēt.

1. Notikuma detalizētās informācijas sadaļā izlasiet ceļa vērtību, kas ir vērtība, kas definē izņēmumu.
    - Pēc iespējas precīzāk noteikt izņēmumus.
    - Lietojiet aizstājējzīmi, ja nepieciešams (piemēram, aizstājiet mainīgo Lietotājs).

1. Lietojiet izņēmumus atbilstoši izvietošanas vajadzībām. Detalizētu informāciju skatiet rakstā [Uzbrukuma virsmas samazināšanas kārtulu pielāgošana.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)

## <a name="exclusion-is-not-honored"></a>Izņēmumi netiek paturēti

1. Nosakiet, vai kārtula atbalsta izņēmumus. Detalizētu informāciju skatiet rakstā [Uzbrukuma virsmas samazināšanas kārtulas.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)

1. Pārskatiet lietotos izņēmumus un pārbaudiet, vai ir ievadīti drukas kļūdu vai nepareizi interpretētu aizstājējzīmju dati. Papildinformāciju skatiet rakstā [Atbalstītie izņēmumu tipi.](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)

1. ja kārtulas ietekme ir pārāk augsta, apsveriet iespēju pārvietot kārtulu (atpakaļ) uz audita režīmu, lai veiktu papildu validāciju. Detalizētu informāciju skatiet rakstā [Pārbaudiet, kā Microsoft Defender galapunkta līdzekļiem darbojas audita režīmā.](/microsoft-365/security/defender-endpoint/audit-windows-defender)

1. Apkopojiet atbalsta datus, lai atvērtu atbalsta gadījumu, izmantojot šo komandu:
    
   ** MDEClientAnalyzer.cmd -v**

    Lai iegūtu papildinformāciju, skatiet rakstu Ar datoru [sēšanu saistītie jautājumi līdz programmatūrai Microsoft Defender galapunktiem.](issues-with-onboarding-machines.md)
