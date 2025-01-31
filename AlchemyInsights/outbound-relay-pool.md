---
title: Izejošā pārraide pūls
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: 7e5bb1fda1dec0c0f72d1944d54b6f2747a6e909
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58326084"
---
# <a name="outbound-relay-pool"></a>Izejošā pārraide pūls

Microsoft veic dažas izmaiņas e-pasta pārsūtīšanas vai pārsūtīšanas konfigurācijā, izmantojot Microsoft 365. Ziņojumi noteiktos scenārijos tiek pārsūtīti vai izlaisti, Microsoft 365 izmanto īpašu pārraides pūlu. Ziņojumi, kas tiek sūtīti, izmantojot pārraides pūlu, var nokļūt adresāta nevēlamā e-pasta mapē. Papildinformāciju skatiet rakstā [Izejošā piegādes maršruts](https://docs.microsoft.com/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Lai izvairītos no scenārija, izmantojot pārraides pūlu, pārliecinieties, vai pārsūtītie/pārsūtītie ziņojumi atbilst vienam no šiem kritērijiem:

- Izejošais sūtītājs ir nomnieka akceptētais domēns.
- Sūtītāja politikas struktūra (Sender Policy Framework – SPF) nodod visu ziņojumu Microsoft 365.
- DomainKeys identificētais pasts (DomainKeys Identified Mail – DKIM) P2 sūtītāja domēnā tiek nododams, kad ziņojums Microsoft 365.
 
Ziņojumi, kas atbilst iepriekš minētajiem kritērijiem, netiek izlaisti caur pārraides pūlu.

Ja jūsu domēna MX ieraksts norāda uz trešās puses vai lokālo serveri, izmantojiet uzlaboto filtrēšanu, lai pārliecinātos, vai SPF validācija ir pareiza ienākošajiem e-pasta ziņojumiem un izvairītos no e-pasta sūtīšanas caur pārraides pūlu.

**Kā noteikt, vai pārraides pūls ietekmēs mūs?**

Ja pārsūtītie vai izlaistie e-pasta ziņojumi izmanto kādu no iepriekš minētajiem kritērijiem, ziņojumi netiks pārsūtīti caur pārraides pūlu. Taču, ja ziņojums tiek nosūtīts caur pārraides pūlu, izejošā servera IP adrese atrodas diapazonā 40.95.0.0/16 un izejošā servera nosaukumā ir iekļauts **rly.**

