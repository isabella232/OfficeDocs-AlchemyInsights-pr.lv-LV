---
title: BitLocker atkopšanas atslēgas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 4e06e0e43b63836b9e9cf923e554dd474b82c671
ms.sourcegitcommit: 123e9fe46e99719dd271e75a66555861e968f4a2
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/30/2019
ms.locfileid: "40908821"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Piekļūšana BitLocker atkopšanas atslēgām

Konfigurējot BitLocker iestatījumus InTune galapunkta aizsardzības politiku, ir iespējams noteikt, vai BitLocker atkopšanas informācija ir jāglabā Azure Active Directory.

Ja šis iestatījums ir konfigurēts, saglabātos atkopšanas dati ir jābūt redzamai InTune admin kā daļa no ierīces ieraksta datu InTune ierīces asmens divos veidos:

Ierīces-Azure AD ierīces-> "ierīces" vai ierīces-> visas ierīces-> "ierīce"-> atkopšanas atslēgas

Alternatīvi, ja ir administratīva piekļuve pašai ierīcei, atkopšanas atslēgu (paroli) var redzēt, izpildot šādu komandu priviliģētā komandu uzvednē:

```
manage-bde -protectors c: -get
Example
Volume C: []
All Key Protectors
    TPM:
      ID: {8A5D13D6-7ED9-46C8-A74F-AC3ADF016EC8}
      PCR Validation Profile:
        0, 2, 4, 8, 9, 10, 11
    Numerical Password:
      ID: {DFA26333-XXXX-402C-YYYY-A8C40AF3ZZZZ}
      Password:
        393943-22222-281721-555554-577984-77777-194700-99999
```
Ja ierīce ir šifrēta pirms reģistrācijas InTune, atkopšanas atslēga var būt saistīta ar "Microsoft konts" (PPL) izmanto, lai pierakstītos ierīces OOBE procesa laikā. Ja tas tā ir, piekļūstot https://onedrive.live.com/recoverykey un pierakstoties ar šo MSA, ir jāparāda ierīces, kurām ir saglabātas atkopšanas atslēgas.
 
Ja ierīce tika šifrēta konfigurācijas dēļ ar grupas politiku, izmantojot domēnu, atkopšanas informāciju var saglabāt lokālo Active Directory.
 

