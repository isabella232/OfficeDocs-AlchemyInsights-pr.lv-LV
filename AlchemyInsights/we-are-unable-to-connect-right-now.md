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
ms.openlocfilehash: b46bac60633ad9a006b9446919b8c99e221b07e4
ms.sourcegitcommit: f28dafa0f727870038f72bc904da926daf4ec07b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/05/2020
ms.locfileid: "44581882"
---
# <a name="fixing-the-microsoft-365-apps-we-are-unable-to-connect-right-now-message"></a>Fixing Microsoft 365 progr "mēs nevaram izveidot savienojumu tieši tagad" ziņojums

Ja saņemat šo ziņojumu, mēģiniet veikt šādas darbības:

1. Pārbaudiet ugunsmūra, pretvīrusu programmatūras un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Microsoft 365 lietojumprogrammām. Skatiet [Microsoft URL un IP adrešu diapazoni](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Dodieties uz **Sākt**  >  **palaišanu**un pēc tam ierakstiet **Services. msc**. Pārliecinieties, vai darbojas šādi pakalpojumi:
    - Tīklam pievienotās ierīces automātiskā iestatīšana
    - Tīkla saraksta pakalpojums
    - Tīkla atrašanās vietas apzināšana
    - Windows notikumu žurnālā

Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt. Ja jums ir problēma, startējot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:

**sfc/scannow**

Pēc tam, kad šī komanda ir pabeigta, restartējiet datoru.

Lai iegūtu detalizētu informāciju, skatiet sadaļu ["Atvainojiet, mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz "kļūda, aktivizējot Office no Microsoft 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).