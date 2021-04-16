---
title: Aktivizācijas problēma — pašlaik nevar izveidot savienojumu
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 2dd3c97bb85254215b13ee8a1222941c0492b204
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51806449"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 programmu kļūdas ziņojums "Šobrīd nevar izveidot savienojumu"

Ja saņemat šādu ziņojumu, mēģiniet veikt šādas darbības:

1. Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, vai nebloķē piekļuvi internetam Microsoft 365 programmām. Skatiet [rakstu Microsoft URL un IP adrešu diapazoni.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Dodieties **uz Start**  >  **Run** un pēc tam ierakstiet **services.msc**. Pārliecinieties, vai darbojas tālāk sniegtie pakalpojumi.
    - Tīkla savienoto ierīču automātiskā iestatīšana
    - Tīkla saraksta pakalpojums
    - Tīkla atrašanās vietas informētība
    - Windows notikumu žurnāls

Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt. Ja rodas problēma, startējot pakalpojumu, palaidiet tālāk norādīto komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:

**sfc /scannow**

Kad šī komanda ir pabeigta, restartējiet datoru.

Detalizētu informāciju skatiet sadaļā ["Diemžēl nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz", aktivizējot Office no Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)