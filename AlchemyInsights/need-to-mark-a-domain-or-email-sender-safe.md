---
title: Vai ir nepieciešams atzīmēt domēnu vai e-pasta sūtītāju kā drošu?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002921"
- "5673"
ms.openlocfilehash: 7dc1576fd61e87b319c7486c59ed125943b4d959
ms.sourcegitcommit: 43acdecef129bfffc8bbe8ebb08fdd581b238a03
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/18/2020
ms.locfileid: "44281178"
---
# <a name="need-to-mark-a-domain-or-email-sender-safe"></a>Vai ir nepieciešams atzīmēt domēnu vai e-pasta sūtītāju kā drošu?

- **Drošo sūtītāju sarakstu** izmantošana nav ieteicama, jo tā atver jūsu organizācijai surogātpastu, phish un izlikšanās uzbrukumiem.
- Tomēr, ja ir biznesa prasības, **ieteicams izmantot** **[pasta plūsmas kārtulas](https://docs.microsoft.com/microsoft-365/security/office-365-security/create-safe-sender-lists-in-office-365?view=o365-worldwide#recommended-use-mail-flow-rules)** . Mūsu norādījumi nodrošina sūtītāja autentifikāciju (pārbauda sūtīšanas domēns netiek viltoti). **Piezīme**: nav ieteicams pārvaldīt viltus pozitīvi, izmantojot drošo sūtītāju sarakstus, jo surogātpasta filtrēšanas izņēmumi var atvērt jūsu organizācijas drošības uzbrukumiem. Ja jūsu lietotājs (i) saņem ziņojumus, kas nepareizi atzīmēti kā surogātpasts vai Nevēlamais e-pasts, lūdzu, **[ziņojiet par ziņojumiem un failiem korporācijai Microsoft](https://protection.office.com/reportsubmission)**.
- Droši sūtītāji programmā Outlook, atļauto sūtītāju sarakstā vai atļauto domēnu sarakstā pretsurogātpasta politikā **ir jāizvairās** , jo sūtītāji apiet visus surogātpastu, mānību, un phish aizsardzību un sūtītāja AUTENTIFIKĀCIJU (SPF, DKIM, dmarc). Šo metodi ieteicams izmantot tikai pagaidu testēšanai.
