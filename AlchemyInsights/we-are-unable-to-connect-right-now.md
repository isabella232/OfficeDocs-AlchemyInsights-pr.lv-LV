---
title: Aktivizācijas problēma-mēs nevaram izveidot savienojumu tieši tagad
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3408"
- "9001423"
ms.openlocfilehash: 56accf68f2cf41dbe6119281b74e2cb56b702789
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43716179"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Office lietojumprogrammu labošana "mēs nevaram izveidot savienojumu tieši tagad" ziņojums

Ja saņemat šo ziņojumu, mēģiniet veikt šādas darbības:

1. Pārbaudiet ugunsmūra, pretvīrusu programmatūras un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Office lietojumprogrammām. Skatiet [Microsoft URL un IP adrešu diapazoni](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Dodieties uz **Sākt** > **palaišanu**un pēc tam ierakstiet **Services. msc**. Pārliecinieties, vai darbojas šādi pakalpojumi:
    - Tīklam pievienotās ierīces automātiskā iestatīšana
    - Tīkla saraksta pakalpojums
    - Tīkla atrašanās vietas apzināšana
    - Windows notikumu žurnālā

Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt. Ja jums ir problēma, startējot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:

**sfc/scannow**

Pēc tam, kad šī komanda ir pabeigta, restartējiet datoru.

Lai iegūtu detalizētu informāciju, skatiet sadaļu ["Atvainojiet, mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz "kļūda, aktivizējot Office no Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).