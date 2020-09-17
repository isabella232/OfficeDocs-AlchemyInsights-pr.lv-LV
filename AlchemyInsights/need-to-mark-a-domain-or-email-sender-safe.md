---
title: Vai vēlaties atzīmēt, ka domēns vai e-pasta sūtītājs ir drošībā?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 0ea089b95ad7de25e77017196fb2db895d4d0178
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47803252"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Vai vēlaties atzīmēt, ka domēns vai e-pasta sūtītājs ir drošībā?

- **Drošo sūtītāju sarakstu izmantošana nav ieteicama** , jo tā atver jūsu organizāciju surogātpasta, adresi phish un izlikšanās uzbrukumiem.
- Tomēr, ja pastāv biznesa prasība, **iesakām izmantot** **[pasta plūsmas kārtulas](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** . Mūsu norādījumi nodrošina sūtītāja autentifikāciju (pārbauda, vai sūtītais domēns netiek viltots). **Piezīme**: neiesakām pārvaldīt viltus pozitīvos, izmantojot drošo sūtītāju sarakstus, jo surogātpasta filtrēšanas izņēmumi var atvērt jūsu organizāciju drošības uzbrukumiem. Ja jūsu lietotājs (i) saņem ziņojumus, kas nepareizi atzīmēti kā surogātpasts vai Nevēlamais e-pasts, lūdzu, **[Ziņojiet par ziņojumiem un failiem korporācijai Microsoft](https://protection.office.com/reportsubmission)**.
- Ir **jāizvairās no** drošo sūtītāju saraksta programmā Outlook, atļauto sūtītāju sarakstā vai atļauto domēnu sarakstā surogātpasta novēršanas politikā, jo sūtītāji apiet visu surogātpasta, mānīšanās un adresi phish aizsardzību un sūtītāja AUTENTIFIKĀCIJU (SPF, DKIM, DMARC). Šo metodi ieteicams izmantot tikai pagaidu pārbaudei.
