---
title: 2681 uzbrukums simulators Office 365
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "2681"
ms.assetid: ''
ms.openlocfilehash: 07d7622c00074f7bd0d567185824db448f1eeef3
ms.sourcegitcommit: 7232b48bcd8bb9867d52a2f055a46ce76a58b8da
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/27/2019
ms.locfileid: "37305338"
---
# <a name="attack-simulator-in-office-365"></a>Attack Simulator Office 365

- Vai jums trūkst uzbrukums simulators? Attack Simulator nepieciešama **office 365 uzlabotā Pretdraudu aizsardzības plāns 2 (ATP plāns 2)** vai **Office 365 Enterprise E5**. Uzbrukuma simulators nav **iekļauts office** 365 uzlabotā Pretdraudu aizsardzības plānā 1 (ATP Plan 1), Office 365 Enterprise E3 vai jebkurš Office 365 Business abonementi.

- Kontu, ko izmanto, lai palaistu simulēta uzbrukumiem nepieciešama globālā administratora vai drošības administratora atļaujas un vairāku faktoru autentifikācija (MFA). Lai iegūtu papildinformāciju par uzbrukuma simulatora prasībām, skatiet [šo tēmu](https://docs.microsoft.com/office365/securitycompliance/attack-simulator#before-you-begin).

- Svarīgas lietas, kas jāzina par **brutālu spēku parole** uzbrukums simulācijas:

  - Ja mērķa konts ir iespējots MFA un parole ir uzminējis pareizi, konts netiks rādīta kā apdraudēta (otrais autentifikācijas koeficients būs nepilnīga).

  - Paroles fails nevar būt lielāks par 10 MB. Katrā rindiņā izmantojiet vienu paroli un iekļaujiet tukšu rindiņu (rakstatgrieze) pēc pēdējās paroles sarakstā.

- Svarīgas lietas, kas jāzina par **šķēpu pikšķerēšana** pievienot simulācijas:

  - Pēc noformējuma nevar nodrošināt pielāgotu vērtību **pikšķerēšanas pieteikšanās servera URL**.

  - Ja adresāts izmanto atskaišu [ziņojumu pievienojumprogrammu iespējot](https://docs.microsoft.com/microsoft-365/security/office-365-security/enable-the-report-message-add-in) , lai ziņotu par ziņojumu kā pikšķerēšanu, iespējams, nesaņemsit ziņojuma brīdinājumus (jo tas ir simulēts uzbrukums).

- Ziņojumi: pēc simulēta uzbrukums ir pabeigta, jūs varat noklikšķināt **uzbrukums detaļas** redzēt ziņojumu.

- Detalizētus norādījumus un jaunas funkcijas uzbrukums simulators, skatiet [Attack Simulator Office 365](https://docs.microsoft.com/microsoft-365/security/office-365-security/attack-simulator).
