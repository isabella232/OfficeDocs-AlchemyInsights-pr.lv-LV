---
title: Labošana Office Apps Atvainojiet, mums ir pagaidu servera problēmas ziņojums
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3420"
- "9001430"
ms.openlocfilehash: a1ac62f3587e318d563cfea1df8db23b720358a6
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43764124"
---
# <a name="fixing-the-office-apps-sorry-we-are-having-temporary-server-issues-message"></a>Office lietojumprogrammu labošana "Atvainojiet, mums ir pagaidu servera problēmas" ziņojums

Ja saņemat šo ziņojumu, mēģiniet veikt šādas darbības:

1. Pārbaudiet ugunsmūra, pretvīrusu programmatūras un starpniekservera iestatījumus, lai pārliecinātos, vai tie nebloķē interneta piekļuvi Office lietojumprogrammām. Skatiet [vietrāžus URL un IP adrešu diapazonus](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges).

2. Dodieties uz **Sākt** > **palaišanu**un pēc tam ierakstiet **Services. msc**. Pārliecinieties, vai darbojas šādi pakalpojumi:
    - Tīklam pievienotās ierīces automātiskā iestatīšana
    - Tīkla saraksta pakalpojums
    - Tīkla atrašanās vietas apzināšana
    - Windows notikumu žurnālā

Ja kāds no šiem pakalpojumiem nedarbojas, mēģiniet to startēt. Ja jums ir problēma, startējot pakalpojumu, izpildiet šādu komandu, atverot komandu uzvedni ar paaugstinātām atļaujām:

**sfc/scannow**

Pēc tam, kad šī komanda ir pabeigta, restartējiet datoru.

Lai iegūtu detalizētu informāciju, skatiet sadaļu ["Atvainojiet, mēs nevaram izveidot savienojumu ar jūsu kontu. Lūdzu, vēlāk mēģiniet vēlreiz "kļūda, aktivizējot](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365).