---
title: Aktivizēšanas problēma — pašlaik nevaram izveidot savienojumu
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 24fe9910d1715b4f5f7d8d06b1d1344d4b8675bc
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47725990"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Microsoft 365 programmu labošana "pašlaik nevar izveidot savienojumu"

Ja tiek parādīts šis ziņojums, izmēģiniet tālāk norādītās darbības.

1. Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Microsoft 365 programmām. Skatiet [Microsoft vietrāžus URL un IP adrešu diapazoni](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Dodieties uz **Sākt**  >  **izpildi**un pēc tam ierakstiet **Services. msc**. Pārliecinieties, vai visi šie pakalpojumi darbojas:
    - Tīkla pievienotās ierīces automātiskā iestatīšana
    - Tīkla saraksta pakalpojums
    - Tīkla vietas izpratne
    - Windows notikumu žurnāls

Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet sākt to. Ja rodas problēmas, sākot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:

**sfc/scannow**

Kad šī komanda ir pabeigta, restartējiet datoru.

Detalizētu informāciju skatiet rakstā ["Diemžēl mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, mēģiniet vēlreiz vēlāk, kad aktivizējat Office no Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).