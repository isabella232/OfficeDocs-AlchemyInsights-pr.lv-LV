---
title: 2681 attack simulator in Microsoft 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: b173c6eb3bbbd1beba3b59878ae12bbe7684d0447a16fef746e5b97b82349e53
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54065291"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator in Microsoft 365

- Vai trūkst uzbrukuma simulatora? Uzbrukuma simulatoram ir **nepieciešama programmatūra Microsoft Defender Office 365 2.** vai Office 365 Enterprise **E5.** Attack Simulator nav **iekļauts** programmatūrā Microsoft Defender Office 365 1. plānam, Office 365 Enterprise E3 un citiem Microsoft 365 programmas darbam abonementiem.

- Kontam, kuru izmantojat simulētu uzbrukumu palaišanai, ir nepieciešamas globālā administratora vai drošības administratora atļaujas un daudzpakāpju autentifikācija (multi-factor authentication — MFA). Papildinformāciju par uzbrukumu simulatora prasībām skatiet [šajā tēmā.](/microsoft-365/security/office-365-security/attack-simulator)

- Svarīgas lietas, kas jāzina **par Brute Force Password uzbrukumu** simulācijām:

  - Ja mērķa kontā ir iespējota MFA un parole tika uzminēta pareizi, konts netiks rādīts kā uz apdraudējuma (otrais autentifikācijas faktors būs nepilnīgs).

  - Paroles fails nedrīkst būt lielāks par 10 MB. Izmantojiet vienu paroli katrā rindiņā un pēc pēdējās paroles sarakstā iekļaujiet tukšu rindiņu (rakstatgriezi).

- Svarīgas lietas, kas jāzina par **Pikšķerēšanas attach** simulācijām:

  - Pikšķerēšanas pieteikšanās servera URL nevar norādīt pielāgotu **vērtību.**

  - Ja adresāts izmanto pievienojumprogrammu Iespējot atskaišu ziņojumu, lai ziņotu par [ziņojumu](/microsoft-365/security/office-365-security/enable-the-report-message-add-in) kā pikšķerēšanas ziņojumu, iespējams, nesaņemsit brīdinājumus par ziņojumu (jo tas ir simulēts uzbrukums).

- Atskaites. Kad simulētais uzbrukums ir pabeigts, varat noklikšķināt uz Detalizēta informācija par **uzbrukumu,** lai skatītu atskaiti.

- Detalizētus norādījumus un jaunos līdzekļus attack simulatorā skatiet rakstā [Attack Simulator in Microsoft 365](/microsoft-365/security/office-365-security/attack-simulator).
