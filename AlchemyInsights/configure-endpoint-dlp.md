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
ms.openlocfilehash: 97a8d4e7db9aac65e6a505c0bef8b41d2ea23353
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58323925"
---
# <a name="configure-endpoint-dlp"></a>Galapunkta DLP konfigurēšana

Microsoft galapunkta DLP ļauj paplašināt DLP aizsardzību un uzraudzības iespējas, iekļaujot sensitīvu informāciju Windows 10 ierīcēs. Pēc tam, kad ierīces ir iekļautas ierīču pārvaldībā, varat izveidot DLP politikas, lai ieviestu informācijas aizsardzības darbības ar vienumiem. Darbību pārlūku var izmantot, lai pārraudzītu sensitīvu vienumu darbības. Papildinformāciju skatiet rakstā [Ierīču pievienošana ierīču pārvaldībai](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices-into-device-management).  

Lai sāktu darbu ar Galapunkta DLP.

- Pārliecinieties, vai jums ir atbilstoša SKU/abonementu licencēšana. Papildinformāciju skatiet rakstā [SKU/abonementu licencēšanas](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#skusubscriptions-licensing).
- Pārbaudiet atļaujas, kas nepieciešamas, lai iespējotu ierīces pārvaldību, piekļūtu pievienošanas lapai vai ieslēgtu/izslēgtu ierīces uzraudzību. Papildinformāciju skatiet rakstā [Licenču piešķiršana](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#permissions).
- Pievienojiet ierīces ierīču pārvaldībai, veicot pievienošanas ierīču procedūru. Papildinformāciju skatiet rakstā [Ierīču pievienošana](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-getting-started#onboarding-devices). 
- Izveidojiet DLP politikas, lai aizsargātu savus sensitīvos vienumus. Papildinformāciju skatiet rakstā [Galapunkta DLP politikas scenāriji](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-using?view=o365-worldwide#endpoint-dlp-policy-scenarios).

Papildinformāciju par Microsoft galapunkta DLP skatiet rakstā [Papildinformācija par Microsoft 365 galapunkta datu zuduma novēršanu (priekšskatījums)](https://docs.microsoft.com/microsoft-365/compliance/endpoint-dlp-learn-about).

**Svarīgas datu apkopošanas darbības, ja nepieciešams atbalsts.**

1. Lejupielādējiet [MDATP klienta analizētāja priekšskatījumu.](https://aka.ms/betamdatpanalyzer)
1. Palaidiet rīku kā administrators, izmantojot cmd logu:

    **MDATPClientAnalyzerPreview\MDATPClientAnalyzer.cmd –t**

1. Ja tiek **prasīts, kā ievadīt izsekošanas apkopošanas minūšu skaitu:**, ievadiet minūšu skaitu, kas nepieciešams, lai izpildītu scenāriju.
1. Palaidiet scenāriju.

Apkopojiet ZIP faila izvadi, lai to sniegtu atbalsta dienesta pārstāvim.
