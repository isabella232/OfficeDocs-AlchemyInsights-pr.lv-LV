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
ms.openlocfilehash: 84e3a7700558ad8a5fad5b7ded6354fe8736e0f7
ms.sourcegitcommit: 358e7ed05c262f909bfa9ed0df730e1fd89266b8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/27/2019
ms.locfileid: "39628249"
---
# <a name="fixing-the-office-apps-we-are-unable-to-connect-right-now-message"></a>Office lietojumprogrammu labošana "mēs nevaram izveidot savienojumu tieši tagad" ziņojums

Ja saņemat šo ziņojumu, mēģiniet veikt šādas darbības:

1. Pārbaudiet ugunsmūra, pretvīrusu programmatūras un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Office lietojumprogrammām. Skatiet [Office 365 vietrāžus URL un IP adrešu diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Dodieties uz **Sākt** > **palaišanu**un pēc tam ierakstiet **Services. msc**. Pārliecinieties, vai darbojas šādi pakalpojumi:
    - Tīklam pievienotās ierīces automātiskā iestatīšana
    - Tīkla saraksta pakalpojums
    - Tīkla atrašanās vietas apzināšana
    - Windows notikumu žurnālā

Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt. Ja jums ir problēma, startējot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:

**sfc/scannow**

Pēc tam, kad šī komanda ir pabeigta, restartējiet datoru.

Lai iegūtu detalizētu informāciju, skatiet sadaļu ["Atvainojiet, mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz "kļūda, aktivizējot Office no Office 365](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).