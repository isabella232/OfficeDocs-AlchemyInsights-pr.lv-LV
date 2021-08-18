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
ms.openlocfilehash: afc865a7b91036bd2d982e21dce059a87e109e3e
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58319955"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Vai vēlaties atzīmēt domēnu vai e-pasta sūtītāju kā drošu?

- Drošo **sūtītāju sarakstu izmantošana nav ieteicama,** jo tādējādi jūsu organizācija tiek atvērta surogātpasta, pikšķerēšanas un izlikšanās uzbrukumiem.
- Tomēr, ja ir biznesa prasības, iesakām **šim nolūkam** **[Flow pasta Flow](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** kārtulas. Mūsu norādījumi nodrošina, ka sūtītāja autentifikācija (verificē domēna sūtīšanu netiek izlikšanās). 
    **Piezīme.** Nav ieteicams pārvaldīt aplami pozitīvos ziņojumus, izmantojot drošo sūtītāju sarakstus, jo surogātpasta filtrēšanas izņēmumi var atvērt jūsu organizāciju drošības uzbrukumiem. Ja lietotājs(i) saņem ziņojumus, kas nepareizi atzīmēti kā surogātpasts vai nevēlamais e-pasts, ziņojiet par **[ziņojumiem un failiem korporācijai Microsoft.](https://protection.office.com/reportsubmission)**
- Seifs Ir jāizvairās no sūtītājiem pakalpojumā Outlook, atļauto sūtītāju  sarakstā vai atļauto domēnu sarakstā pretsurogātpasta politikās, jo sūtītāji apiet visu surogātpastu, izlikšanās un pikšķerēšanas aizsardzību, kā arī sūtītāju autentifikāciju (SPF, DKIM, DMARC). Šī metode ir vislabāk izmantojama tikai pagaidu testēšanai.
- Lai pārbaudītu, vai noteiktu e-pasta apieto Antispam novērtējumu var veikt, atzīmējiet ziņojuma galveni "X-Forefront-Antispam-Report" (SFV:SFE, SFV:SKA, SFV:SKN), skatiet rakstu Pretsurogātpasta ziņojumu **[iesākumi.](https://docs.microsoft.com/microsoft-365/security/office-365-security/anti-spam-message-headers)**
- Tā kā Microsoft pēc noklusējuma vēlas [paturēt](https://docs.microsoft.com/microsoft-365/security/office-365-security/secure-by-default#exceptions)mūsu klientu drošību, daži nomnieka ignorēšana netiek lietota ļaunprogrammatūrai un ļoti drošai pikšķerēšanas programmatūrai. Šie ignorēšanas iestatījumi ietver: o Atļautie sūtītāju saraksti vai atļautie domēnu saraksti (pretsurogātpasta politikas), Outlook Seifs sūtītāju o IP atļauto adrešu saraksts (savienojuma filtrēšana) 
- Vienīgais ignorēšana, kas nodrošina augstas ticamības pikšķerēšanas ziņojumu filtrēšanas apiešanu, Exchange pasta plūsmas kārtulas (tiek dēvētas arī par transporta kārtulām). Lai izmantotu pasta plūsmas kārtulas filtrēšanas apiešanai, skatiet rakstu Pasta plūsmas kārtulu izmantošana, lai iestatītu surogātpasta ticamības līmeni **[(SCL) ziņojumos.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-mail-flow-rules-to-set-the-spam-confidence-level-scl-in-messages)**