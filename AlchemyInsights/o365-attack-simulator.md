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
ms.openlocfilehash: 7b48abea3400e3565f2ba33c97e24e5b9923eb3b
ms.sourcegitcommit: 4caf5e6c2fee2903ccaf92cfc9006eb580faa7ba
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/29/2020
ms.locfileid: "48801558"
---
# <a name="attack-simulator-in-microsoft-365"></a>Uzbrukuma simulators programmā Microsoft 365

- Vai jums trūkst uzbrukuma simulators? Uzbrukuma simulatoram ir nepieciešama **programma Microsoft Defender darbam ar office 365 2. plāns (ATP 2. plāns)** vai **Office 365 Enterprise E5** . Uzbrukuma simulators **nav** iekļauts produktā Microsoft Defender for Office 365 1. plāns (ATP 1. plāns), Office 365 Enterprise E3 vai jebkuras Microsoft 365 lietojumprogrammas darbam abonementiem.

- Kontam, ko izmantojat, lai palaistu simulētos uzbrukumus, nepieciešama globālā administratora vai drošības administratora atļaujas un daudzfaktoru autentifikācija (MFA). Papildinformāciju par uzbrukuma simulatora prasībām skatiet [šajā tēmā](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).

- Svarīgas lietas, kas jāzina par **brutālas spēku paroļu** uzbrukuma simulācijām:

  - Ja adresāta kontam ir iespējota MFA un parole ir uzrakstīta pareizi, konts netiks rādīts kā kompromitēts (otrais autentifikācijas faktors nebūs pilnīgs).

  - Paroles fails nedrīkst būt lielāks par 10 MB. Izmantojiet vienu paroli katrai rindiņai un pēc pēdējās saraksta paroles iekļaujiet tukšu rindiņu (rakstatgriezes).

- Svarīgas lietas, kas jāzina par **šķēpa pikšķerēšanas** pievienošanu simulācijām:

  - Pēc noformējuma nevar nodrošināt pielāgotu vērtību **pikšķerēšanas pieteikšanās servera URL** .

  - Ja adresāts izmanto [Iespējot atskaites ziņojuma pievienojumprogrammu](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , lai ziņotu par ziņojumu kā pikšķerēšanu, iespējams, nesaņemsit brīdinājumus par ziņojumu (jo tas ir simulēts uzbrukums).

- Atskaites: kad Simulētais uzbrukums ir pabeigts, varat noklikšķināt uz **uzbrukt detalizēti** , lai skatītu atskaiti.

- Detalizētus norādījumus un jaunus līdzekļus Attack simulatorā skatiet rakstā [Microsoft 365 uzbrukuma simulators](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
