---
title: 2681 uzbrukuma simulators programmā Microsoft 365
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
ms.openlocfilehash: dec96238c8438dcf9df176e3e3f20bd8a985b2cc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47759226"
---
# <a name="attack-simulator-in-microsoft-365"></a>Uzbrukuma simulators programmā Microsoft 365

- Vai jums trūkst uzbrukuma simulators? Uzbrukuma simulatoram ir nepieciešams **office 365 uzlabots draudu aizsardzības plāns 2 (ATP 2. plāns)** vai **Office 365 Enterprise E5**. Uzbrukuma simulators **nav iekļauts** produktā Office 365 Advanced Threat Protection Plan 1 (ATP 1. plāns), Office 365 Enterprise E3 vai Microsoft 365 lietojumprogrammas darbam ar abonementu.

- Kontam, ko izmantojat, lai palaistu simulētos uzbrukumus, nepieciešama globālā administratora vai drošības administratora atļaujas un daudzfaktoru autentifikācija (MFA). Papildinformāciju par uzbrukuma simulatora prasībām skatiet [šajā tēmā](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Svarīgas lietas, kas jāzina par **brutālas spēku paroļu** uzbrukuma simulācijām:

  - Ja adresāta kontam ir iespējota MFA un parole ir uzrakstīta pareizi, konts netiks rādīts kā kompromitēts (otrais autentifikācijas faktors nebūs pilnīgs).

  - Paroles fails nedrīkst būt lielāks par 10 MB. Izmantojiet vienu paroli katrai rindiņai un pēc pēdējās saraksta paroles iekļaujiet tukšu rindiņu (rakstatgriezes).

- Svarīgas lietas, kas jāzina par **šķēpa pikšķerēšanas** pievienošanu simulācijām:

  - Pēc noformējuma nevar nodrošināt pielāgotu vērtību **pikšķerēšanas pieteikšanās servera URL**.

  - Ja adresāts izmanto [Iespējot atskaites ziņojuma pievienojumprogrammu](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , lai ziņotu par ziņojumu kā pikšķerēšanu, iespējams, nesaņemsit brīdinājumus par ziņojumu (jo tas ir simulēts uzbrukums).

- Atskaites: kad Simulētais uzbrukums ir pabeigts, varat noklikšķināt uz **uzbrukt detalizēti** , lai skatītu atskaiti.

- Detalizētus norādījumus un jaunus līdzekļus Attack simulatorā skatiet rakstā [Microsoft 365 uzbrukuma simulators](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
