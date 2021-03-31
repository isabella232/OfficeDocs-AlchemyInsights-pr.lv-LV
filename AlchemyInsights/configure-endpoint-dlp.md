---
title: Galapunkta DLP konfigurēšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6108"
- "3200001"
ms.openlocfilehash: 36af769b67f8c9aa4b8d17e9f4f3f3b82c8a8534
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51402437"
---
# <a name="configure-endpoint-dlp"></a>Galapunkta DLP konfigurēšana

Microsoft galapunkta DLP ļauj paplašināt DLP aizsardzību un uzraudzības iespējas, iekļaujot sensitīvu informāciju Windows 10 ierīcēs. Pēc tam, kad ierīces ir iekļautas ierīču pārvaldībā, varat izveidot DLP politikas, lai ieviestu informācijas aizsardzības darbības ar vienumiem. Darbību pārlūku var izmantot, lai pārraudzītu sensitīvu vienumu darbības. Papildinformāciju skatiet rakstā [Ierīču pievienošana ierīču pārvaldībai](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Lai sāktu darbu ar Galapunkta DLP.

- Pārliecinieties, vai jums ir atbilstoša SKU/abonementu licencēšana. Papildinformāciju skatiet rakstā [SKU/abonementu licencēšanas](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Pārbaudiet atļaujas, kas nepieciešamas, lai iespējotu ierīces pārvaldību, piekļūtu pievienošanas lapai vai ieslēgtu/izslēgtu ierīces uzraudzību. Papildinformāciju skatiet rakstā [Licenču piešķiršana](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Pievienojiet ierīces ierīču pārvaldībai, veicot pievienošanas ierīču procedūru. Ja sadaļā M365 atbilstības **iestatījumi** trūkst opcijas Ierīces iebūvēšana (priekšskatījums), pārliecinieties, ka jums ir iepriekš minētā atbilstošā licence un atļaujas. Papildinformāciju skatiet rakstā [Ierīču pievienošana](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Izveidojiet DLP politikas, lai aizsargātu savus sensitīvos vienumus. Papildinformāciju skatiet rakstā [Galapunkta DLP politikas scenāriji](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios &preserve-view=true).

Papildinformāciju par Microsoft galapunkta DLP skatiet rakstā [Papildinformācija par Microsoft 365 galapunkta datu zuduma novēršanu (priekšskatījums)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Svarīgas datu apkopošanas darbības, ja nepieciešams atbalsts.**

1. Lejupielādējiet MDATP klienta analizētāja priekšskatījumu no [https://aka.ms/betamdatpanalyzer](https://aka.ms/betamdatpanalyzer "https://aka.ms/betamdatpanalyzer")
2. Palaidiet rīku kā administrators, izmantojot cmd logu:
3. MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t
4. Kad tiek prasīts “Ievadiet minūšu skaitu, lai apkopotu izsekošanas vaicājumus:”, ievadiet minūšu skaitu, kas nepieciešams scenārija izpildei
5. Palaist scenāriju

Zip faila izvades apkopošana, kas jāpiešķir atbalsta dienesta darbiniekam.
