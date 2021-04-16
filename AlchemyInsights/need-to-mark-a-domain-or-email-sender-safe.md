---
title: Vai vēlaties atzīmēt domēnu vai e-pasta sūtītāju kā drošu?
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
- "9002921"
- "5673"
ms.openlocfilehash: a1c4c4d2fadaf75eda9b5b322aca35c32dfee8ea
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51792139"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Vai vēlaties atzīmēt domēnu vai e-pasta sūtītāju kā drošu?

- Drošo **sūtītāju sarakstu izmantošana nav ieteicama,** jo tādējādi jūsu organizācija tiek atvērta surogātpasta, pikšķerēšanas un izlikšanās uzbrukumiem.
- Tomēr, ja ir biznesa prasības, iesakām **šim nolūkam** **[izmantot pasta](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** plūsmas kārtulas. Mūsu norādījumi nodrošina, ka sūtītāja autentifikācija (verificē domēna sūtīšanu netiek izlikšanās). **Piezīme.** Nav ieteicams pārvaldīt aplami pozitīvos ziņojumus, izmantojot drošo sūtītāju sarakstus, jo surogātpasta filtrēšanas izņēmumi var atvērt jūsu organizāciju drošības uzbrukumiem. Ja lietotājs(i) saņem ziņojumus, kas nepareizi atzīmēti kā surogātpasts vai nevēlamais e-pasts, lūdzu, ziņojiet par **[ziņojumiem un failiem korporācijai Microsoft.](https://protection.office.com/reportsubmission)**
- Ir jāizvairās no drošiem sūtītājiem programmā Outlook, atļauto  sūtītāju sarakstam vai atļautajiem domēnu sarakstiem pretsurogātpasta politikās, jo sūtītāji apiet visu surogātpastu, izlikšanās un pikšķerēšanas aizsardzību, kā arī sūtītāju autentifikāciju (SPF, DKIM, DMARC). Šo metodi ir vislabāk izmantot tikai pagaidu testēšanai.
