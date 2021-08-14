---
title: Problēma ar AAD Savienošana darbspēju
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004649"
- "8427"
ms.openlocfilehash: 82cfcc6132549b52278b174fce3173f5566268864a207882a4dd639cb8024ee3
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923759"
---
# <a name="problem-with-aad-connect-health"></a>Problēma ar AAD Savienošana darbspēju

- Pārliecinieties, vai esat pilnvarots veikt šo darbību. Globālajiem administratoriem ir piekļuve pēc noklusējuma. Turklāt varat izmantot lomu piekļuves [vadīklu,](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) lai līdzstrādniekam deleģētu reģistrācijas atļaujas.
- Pārliecinieties, vai obligātie galapunkti ir iespējoti un nav bloķēti ugunsmūra dēļ. Detalizētu informāciju skatiet [prasības.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install)
- Reģistrācija var neizdoties, jo izejošā saziņa tīkla slānī veic SSL pārbaudi.
- Pārliecinieties, vai esat pārbaudījis Azure AD Savienošana Health paziņojumu iestatījumus. Lūdzu, pārskatiet savu iestatījumu. Šī [rokasgrāmata](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) var palīdzēt jums saprast, kā konfigurēt Azure AD Savienošana darbspējas paziņojumus.
- Papildinformāciju par AAD pakalpojuma Savienošana Health sinhronizācijas atskaiti un tās lejupielādi skatiet rakstā [Objekta līmeņa sinhronizācijas atskaite.](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync)

Lai novērstu AAD Savienošana darbspējas brīdinājumus, izpildiet [AAD Savienošana](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) darbspējas datu svaiguma brīdinājumus un bieži uzdotos jautājumus, skatiet rakstu Bieži uzdotie jautājumi par [AAD Savienošana](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)veiktspējas instalēšanu.
