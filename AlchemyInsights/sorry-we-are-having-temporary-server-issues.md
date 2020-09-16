---
title: Microsoft 365 programmu labošana Diemžēl mums ir ziņojumi par pagaidu servera problēmām
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
- "3420"
- "9001430"
ms.openlocfilehash: e00504d318efdea4968ddf98b3ce9591f8993e38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47758252"
---
# <a name="fixing-the-microsoft-365-apps-sorry-we-are-having-temporary-server-issues-message"></a>Izlabojot Microsoft 365 lietojumprogrammas, tiek parādīts ziņojums "Diemžēl radās īslaicīgas problēmas ar serveri"

Ja tiek parādīts šis ziņojums, izmēģiniet tālāk norādītās darbības.

1. Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Microsoft 365 programmām. Skatiet [vietrāžus URL un IP adrešu diapazoni](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Dodieties uz **Sākt**  >  **izpildi**un pēc tam ierakstiet **Services. msc**. Pārliecinieties, vai visi šie pakalpojumi darbojas:
    - Tīkla pievienotās ierīces automātiskā iestatīšana
    - Tīkla saraksta pakalpojums
    - Tīkla vietas izpratne
    - Windows notikumu žurnāls

Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet sākt to. Ja rodas problēmas, sākot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:

**sfc/scannow**

Kad šī komanda ir pabeigta, restartējiet datoru.

Detalizētu informāciju skatiet rakstā ["Diemžēl mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, mēģiniet vēlreiz vēlāk, kad aktivizējat](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).