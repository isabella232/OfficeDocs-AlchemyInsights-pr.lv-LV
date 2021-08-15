---
title: Kļūdas Lietojumprogramma netika atrasta novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9000171"
- "1712"
ms.openlocfilehash: 34b2024257c88512db170cbb0e672c1628ad8e3935342f87c5032492e1ad0259
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54026121"
---
# <a name="mitigate-the-application-was-not-detected-error"></a>Kļūdas Lietojumprogramma netika atrasta novēršana

Lietojumprogrammas instalēšanas kļūda “Lietojumprogramma nav atrasta pēc veiksmīgas instalēšanas”, par kuru ziņo Intune, var notikt visās lielākajās operētājsistēmās (Windows, iOS un Android).

Scenāriji, kas ģenerē šo problēmu visbiežāk:

- Pēc sākotnējās izvietošanas lietojumprogramma tika atjaunināta ārpus Intune (no trešās puses lietojumprogrammu veikala). Piemēram, lietojumprogramma Google Chrome var veikt automātisko atjaunināšanu.
- Lietotājs ir atinstalējis lietojumprogrammu pēc sākotnējās instalēšanas.

Lai novērstu šo problēmu, vispirms ir jāpārskata skartās ierīces, lai noteiktu scenārijus, kuros notiek šī kļūda.

- Ja lietojumprogramma tika atjaunināta ārpus Intune, lietojumprogrammas izvietošanu var iestatīt, lai tā ignorētu lietojumprogrammas versiju. Lai to izdarītu, sadaļā **Lietojumprogrammas konfigurācija > Informācija** iestatiet **Ignorēt lietojumprogrammas** versiju uz **Jā**.
- Veicot ar klientu saistītās darbības, atbilstošs risinājums var būt lietojumprogrammu izvietošana “pēc vajadzības”, lai nodrošinātu jaunākās versijas izvietošanu.
- Alternatīvs risinājums iOS platformā ir izmantot **automātiskās atjaunināšanas** funkciju, kas ir saistīta ar Apple lielapjoma pirkumu programmu, kuru ir iespējams konfigurēt automātiskai atjaunināšanai tiklīdz ir pieejamas jaunas lietojumprogrammas versijas.

Lai uzzinātu vairāk par instalēšanas problēmu novēršanu, lasiet [Lietojumprogrammu instalēšanas problēmu novēršana](https://docs.microsoft.com/intune/troubleshoot-app-install).
