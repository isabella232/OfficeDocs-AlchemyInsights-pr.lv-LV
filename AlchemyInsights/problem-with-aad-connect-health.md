---
title: Problēma ar AAD Connect darbspējas
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
ms.openlocfilehash: f5624069a2e96fde8aed08965ca6b753f3aad1e8
ms.sourcegitcommit: 5763fedfd5dd459249c81cdbb4af34181a757bd5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/04/2021
ms.locfileid: "50482070"
---
# <a name="problem-with-aad-connect-health"></a>Problēma ar AAD Connect darbspējas

- Pārliecinieties, vai jums ir atļauts veikt šo darbību. Globālajiem administratoriem pēc noklusējuma ir piekļuve. Turklāt varat izmantot [lomai bāzētu piekļuves vadību](https://docs.microsoft.com/azure/active-directory/connect-health/active-directory-aadconnect-health-operations) , lai deleģētu reģistrācijas atļaujas līdzstrādniekiem.
- Pārliecinieties, vai nepieciešamie galapunkti ir iespējoti, bet nav bloķēti ugunsmūra dēļ. Detalizētu informāciju skatiet sadaļā [prasības](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-agent-install).
- Reģistrācija var neizdoties, jo izejošā komunikācija tiek pakļauta SSL pārbaudei tīkla slānī.
- Pārliecinieties, vai esat pārbaudījis Azure AD Connect darbspējas paziņojumu iestatījumus. Lūdzu, pārskatiet savu iestatījumu. Šajā [rokasgrāmatā](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-operations) varat palīdzēt saprast, kā konfigurēt Azure AD Connect paziņojumi par paziņojumu iestatījumiem.
- Lai uzzinātu vairāk par to, kā AAD Connect Health sinhronizācijas atskaiti un kā to lejupielādēt, skatiet rakstu [objekta līmeņa sinhronizācijas atskaite](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-sync).

Lai novērstu AAD savienojumu ar veselību brīdinājumus, izpildiet [norādījumus par to, kā AAD savienos](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-health-data-freshness) un bieži uzdotos jautājumus skatiet rakstā [bieži sastopamas AAD savienojuma](https://docs.microsoft.com/azure/active-directory/hybrid/reference-connect-health-faq)problēmas.
