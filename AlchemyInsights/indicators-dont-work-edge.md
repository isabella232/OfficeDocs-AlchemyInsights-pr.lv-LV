---
title: Indikatori nedarbojas, izmantojot pārlūkprogrammu Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: ff7a2ee4c97c579422c7679c461f6fb288a9235ff9056be1c56e80b1d6379723
ms.sourcegitcommit: 920051182781bd97ce4d4d6fbd268cb37b84d239
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/11/2021
ms.locfileid: "57887447"
---
# <a name="indicators-dont-work-using-edge-browser"></a>Indikatori nedarbojas, izmantojot pārlūkprogrammu Edge

Kad esat izveidojis indikatoru, tas netiek pagodēts edge (Smartscreen). Papildinformāciju skatiet rakstā [IP un vietrāžu URL/domēnu indikatoru izveide.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)

## <a name="step-1-ensure-the-following"></a>1. darbība. Pārliecinieties, vai ir:

- Pārliecinieties, vai indikators ir pareizs (IP/URL pārrakstīšanās kļūda, pareizās RBAC grupas).
- Uzgaidiet minimālās 2 stundas pēc indikatora izveides, lai ņem vērā iespējamo latentumu.
- Pārliecinieties, vai sistēma(s) ir pievienota(s) programmatūrai Microsoft Defender galapunktam.
- Pārbaudiet, vai sistēma(s) var sazināties ar mākoni.
- Pārbaudiet, vai smartscreen ir iespējots un sasniedzams, dodoties uz [testa vietni.](https://demo.smartscreen.msft.net)

## <a name="step-2-troubleshoot-the-potential-issue"></a>2. darbība. Potenciālās problēmas novēršana

- Pārliecinieties, vai klients atbilst prasībām. Detalizētu informāciju skatiet rakstā [IP un URL/domēnu indikatoru izveide.](https://docs.microsoft.com/microsoft-365/security/defender-endpoint/indicator-ip-domain)
- Pārliecinieties, vai izmantojat jaunāko pārlūkprogrammas Edge versiju. Lai uzzinātu jaunāko versiju, skatiet [rakstu Uzziniet, kura Microsoft Edge jūsu versija.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)
- Restartējiet pārlūkprogrammu Edge.
- Naviģējiet uz vietni, kurai ir iestatīts indikators. Ja vietne netiek parādīta, kā paredzēts, pārejiet pie 3. darbības. 

## <a name="step-3-collect-data"></a>3. darbība. Datu apkopošana

- Apkopojiet **MDEClientAnalyzer diagnostikas** datus. Norādījumus skatiet rakstā Ar datoru [sēšanu saistītas problēmas līdz programmatūrai Microsoft Defender galapunktam.](issues-with-onboarding-machines.md)
- Ja esat ērti instalējis un apkopojis Fiddler izsekošanas programmu, skatiet [sadaļu Telerik Fiddler.](http://www.telerik.com/fiddler)
- Ja vēlaties saņemt norādījumus no Microsoft atbalsta dienesta, tālāk atlasiet ikonu Atbalsts, lai atvērtu atbalsta gadījumu.
