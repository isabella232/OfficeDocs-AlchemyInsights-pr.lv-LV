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
ms.openlocfilehash: 5dad4b43efac2468b57351a4d6c96379ed505071ca144ec0aa518e975633bb18
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53998164"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Tiek izlabots Microsoft 365 ziņojums "Šobrīd nevar izveidot savienojumu"

Ja saņemat šādu ziņojumu, mēģiniet veikt šādas darbības:

1. Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē piekļuvi Microsoft 365 programmām. Skatiet [rakstu Microsoft URL un IP adrešu diapazoni.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Dodieties **uz Start**  >  **Run** un pēc tam ierakstiet **services.msc**. Pārliecinieties, vai darbojas tālāk sniegtie pakalpojumi.
    - Tīkla savienoto ierīču automātiskā iestatīšana
    - Tīkla saraksta pakalpojums
    - Tīkla atrašanās vietas informētība
    - Windows Notikumu žurnāls

Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt. Ja rodas problēma, startējot pakalpojumu, palaidiet tālāk norādīto komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:

**sfc /scannow**

Kad šī komanda ir pabeigta, restartējiet datoru.

Detalizētu informāciju skatiet sadaļā ["Diemžēl nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz", kad aktivizējat Office no Microsoft 365.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)