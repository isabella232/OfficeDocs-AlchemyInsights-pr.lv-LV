---
title: Pastkastes saņemšanas ierobežošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/31/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "13711"
- "9008580"
ms.openlocfilehash: c1ba5ab10b102680cec52f4e0740c3dd2ceaccbd
ms.sourcegitcommit: a36ec7eda49536933dc8c6f9319cf7320e8aa04d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/31/2021
ms.locfileid: "59316042"
---
# <a name="mailbox-receiving-limit-enforcement"></a>Pastkastes saņemšanas ierobežošana

Microsoft nesen sāka izmantot pastkastes slieksni 3600 ziņojumu stundā. Papildinformāciju skatiet rakstā [Exchange Online ierobežojumi.](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-limits) Microsoft 365 par 3600 ziņojumiem stundas laikā saņemtās pastkastes tiek migrētas uz nākamajām 60 minūtēm. 

Turklāt tiek lietoti sūtītāja-adresātu pāri (SRP) ierobežojums, kas bloķē no konkrēta Microsoft 365 saņemtos ziņojumus. Ja viens sūtītājs konkrētam adresātam sūta vairāk nekā 33% no kopējā sliekšņa vai 1200 ziņojumu vienā slīdošot stundā, TIEK sākts RPC ierobežojums un pastkaste vairs pieņem ziņojumus no šī sūtītāja. Ņemiet vērā:

- Šis ierobežojums ir lietojumprogramma e-pasta ziņojumiem, kas saņemti no citiem nomniekiem, lokāliem vai interneta sūtītājiem.
- E-pasta piegāde pastkastē tiek bloķēta tuvāko 60 minūšu laikā. 
- Šo pastkastu sūtītāji saņem atskaiti par nesniegšanas piegādi (5.2.121 vai 5.2.122), kurā norādīts, ka pastkaste ir pārsniedzusi maksimālo piegādes slieksni. Intra-tenant (mail within the same tenant) joprojām tiek piegādāts.
- Kad tiek lietots ADRESĀTU SKAITS ierobežojums, adresāta pastkaste turpina pieņemt ziņojumus no citiem sūtītājiem.

Administratori var pārraudzīt pašreizējās pastkastes darbības, piekļūstot jaunai atskaitei un ieskatam Exchange administrēšanas centrā "Pastkastes, kas pārsniedz saņemšanas ierobežojumus". Informācija tiek rādīta tikai tad, ja nomniekam ir aizskartas pastkastes, bet atskaite vienmēr tiek rādīta informācijas panelī, bet ir tukša, ja vien nomniekam nav pastkastu aizstās.

Papildinformāciju par informācijas saņemšanas ierobežojumiem skatiet rakstā Pastkastes, kas pārsniedz ierobežojumu [ieskatus jaunajā EAC](https://docs.microsoft.com/exchange/monitoring/mail-flow-insights/mailboxes-exceeding-receiving-limits-insights).

Papildinformāciju par ziņojumu par to, ka tiek pārsniegti saņemšanas ierobežojumi, skatiet rakstā Pastkastes, kas pārsniedz ierobežojumu atskaiti [jaunajā EAC.](https://docs.microsoft.com/exchange/monitoring/mail-flow-reports/mailboxes-exceeding-receiving-limits-report)