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
ms.openlocfilehash: 43f7ae0df98726e61bfe6f93f91909b0bb8a6d19129a99dc027e8b563bc35a6c
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57895798"
---
# <a name="attack-simulator-in-microsoft-365"></a>Attack Simulator in Microsoft 365

- Vai trūkst uzbrukuma simulatora? Attack Simulator nepieciešama **programmatūra Microsoft Defender Office 365 2.** vai Office 365 Enterprise **E5.** Attack Simulator nav **iekļauts** programmatūrā Microsoft Defender Office 365 1. plānam, Office 365 Enterprise E3 un citiem Microsoft 365 programmas darbam abonementiem.

- Kontam, kuru izmantojat simulētu uzbrukumu palaišanai, ir nepieciešamas globālā administratora vai drošības administratora atļaujas un daudzpakāpju autentifikācija (multi-factor authentication — MFA). Papildinformāciju par uzbrukumu simulatora prasībām skatiet [šajā tēmā.](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator)

- Svarīgas lietas, kas jāzina **par Brute Force Password uzbrukumu** simulācijām:

  - Ja mērķa kontā ir iespējota MFA un parole tika uzminēta pareizi, konts netiks rādīts kā uz apdraudējuma (otrais autentifikācijas faktors būs nepilnīgs).

  - Paroles fails nedrīkst būt lielāks par 10 MB. Izmantojiet vienu paroli katrā rindiņā un pēc pēdējās paroles sarakstā iekļaujiet tukšu rindiņu (rakstatgriezi).

- Svarīgas lietas, kas jāzina par **Pikšķerēšanas attach** simulācijām:

  - Pikšķerēšanas pieteikšanās servera URL nevar norādīt pielāgotu **vērtību.**

  - Ja adresāts izmanto pievienojumprogrammu Iespējot atskaišu ziņojumu, lai ziņotu par [ziņojumu](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) kā pikšķerēšanas ziņojumu, iespējams, nesaņemsit brīdinājumus par ziņojumu (jo tas ir simulēts uzbrukums).

- Atskaites. Kad simulētais uzbrukums ir pabeigts, varat noklikšķināt uz Detalizēta informācija par **uzbrukumu,** lai skatītu atskaiti.

- Detalizētus norādījumus un jaunos līdzekļus attack simulatorā skatiet rakstā [Attack Simulator in Microsoft 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
