---
title: Problēmu Microsoft 365 Diemžēl mums ir īslaicīgu servera problēmu ziņojums
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
- "3420"
- "9001430"
ms.openlocfilehash: aa0d625856df1027146de5af57845224e3056d8c21d9ac4cefbd4a9c329f487c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54021603"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Ar programmu Microsoft 365 "Diemžēl mums ir īslaicīgas servera problēmas"

Ja saņemat šādu ziņojumu, mēģiniet veikt šādas darbības:

1. Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē piekļuvi Microsoft 365 programmām. Skatiet [rakstu URL un IP adrešu diapazoni.](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges)

2. Dodieties **uz Start**  >  **Run** un pēc tam ierakstiet **services.msc**. Pārliecinieties, vai darbojas tālāk sniegtie pakalpojumi.
    - Tīkla savienoto ierīču automātiskā iestatīšana
    - Tīkla saraksta pakalpojums
    - Tīkla atrašanās vietas informētība
    - Windows Notikumu žurnāls

Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt. Ja rodas problēma, startējot pakalpojumu, palaidiet tālāk norādīto komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:

**sfc /scannow**

Kad šī komanda ir pabeigta, restartējiet datoru.

Detalizētu informāciju skatiet sadaļā ["Diemžēl nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz", kad aktivizējat.](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)