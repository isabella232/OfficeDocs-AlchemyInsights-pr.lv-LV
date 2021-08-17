---
title: Bitlocker atkopšanas atslēgas
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: f71fae0aabda3fc48f20d5ea1e6909475f0c17ff5cdf98b58b1403bd2e291c19
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54060071"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Piekļuve Bitlocker atkopšanas atslēgām

Konfigurējot Bitlocker iestatījumus Intune galapunktu aizsardzības politiku, var definēt, vai Bitlocker atkopšanas informācija jāglabā Azure Active Directory.

Ja šis iestatījums ir konfigurēts, saglabātajiem atkopšanas datiem jābūt redzamiem Intune administratoram kā daļa no ierīces ierakstu datiem Intune ierīču asmenī divos veidos:

Ierīces - Azure AD ierīces -> "Ierīce" OR ierīces -> Visas ierīces -> "Ierīce" -> atkopšanas atslēgas

Alternatīvi, ja pašai ierīcei ir administratīva piekļuve, atkopšanas atslēgu (paroli) var skatīt, priviliģētā komandu uzvednē izpildot šādu komandu:

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
Ja ierīce tika šifrēta, pirms iereģistrējat Intune, atkopšanas atslēga, iespējams, ir saistīta ar "Microsoft kontu" (MSA), kas izmantota, lai OOBE procesa laikā pierakstītos ierīcē. Šādā gadījumā, piekļūstot šai MSA un pierakstoties tajā, ir jābūt parādītām ierīcēm,  https://onedrive.live.com/recoverykey kurām tika glabātas atkopšanas atslēgas.
 
Ja ierīce tika šifrēta, veicot konfigurēšanu, izmantojot domēna grupas politiku, atkopšanas informācija var tikt glabāta lokālajā Active Directory.

Ja esat konfigurējis galapunkta aizsardzības politiku atkopšanas atslēgas glabāšanai pakalpojumā Azure Active Directory bet konkrētas ierīces atslēga nav augšupielādēta, varat izraisīt augšupielādi, pagriežot šīs ierīces atkopšanas atslēgu no MEM konsoles. Detalizētu informāciju skatiet rakstā [BitLocker atkopšanas atslēgu pagriešana.](https://docs.microsoft.com/mem/intune/protect/encrypt-devices#view-details-for-recovery-keys)

