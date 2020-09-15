---
title: BitLocker atkopšanas atslēgas
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "1922"
- "9000220"
ms.openlocfilehash: 7c56e68cf303939d8e7d4ee0a7301e367ecfe9f9
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47685893"
---
# <a name="accessing-bitlocker-recovery-keys"></a>Piekļuve BitLocker atkopšanas taustiņiem

Konfigurējot BitLocker iestatījumu Intune galapunktu aizsardzības politiku, ir iespējams definēt, vai BitLocker atkopšanas informācija ir jāglabā Azure Active Directory.

Ja šis iestatījums ir konfigurēts, saglabātajiem atkopšanas datiem ir jābūt redzamiem Intune administrators kā daļa no ierīces ieraksta datiem Intune ierīces diskam divējādi:

Ierīces — Azure AD ierīces — > "ierīce" vai ierīces-> visas ierīces-> "ierīce" — > atkopšanas atslēgas

Vai arī, ja pastāv administratora piekļuve pašai ierīcei, atkopšanas atslēgu (paroli) var redzēt, izpildot šādu komandu no privileģētas komandu uzvednes:

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
Ja ierīce tika šifrēta pirms reģistrācijas Intune, atkopšanas atslēga var būt saistīta ar Microsoft kontu (PPL), kas tiek izmantots, lai pierakstītos ierīcē OOBE procesa laikā. Ja tas tā bija, piekļūstot  https://onedrive.live.com/recoverykey un pierakstoties ar šo ppl, ir jāparāda ierīces, kurām ir saglabātas atkopšanas atslēgas.
 
Ja ierīce ir šifrēta kā konfigurācija, kas balstīta uz domēnu grupas politiku, atkopšanas informācija var būt saglabāta lokālajā Active Directory.
 

