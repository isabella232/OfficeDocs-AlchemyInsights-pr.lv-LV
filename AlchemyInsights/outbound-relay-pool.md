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
ms.openlocfilehash: 8750c9036f258d9c5edc94bb027d564140bbd9914712cc1f25ff3abc3f4b9468
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54041593"
---
# <a name="outbound-relay-pool"></a>Izejošā pārraide pūls

Microsoft veic dažas izmaiņas e-pasta pārsūtīšanas vai pārsūtīšanas konfigurācijā, izmantojot Microsoft 365. Ziņojumi noteiktos scenārijos tiek pārsūtīti vai izlaisti, Microsoft 365 izmanto īpašu pārraides pūlu. Ziņojumi, kas tiek sūtīti, izmantojot pārraides pūlu, var nokļūt adresāta nevēlamā e-pasta mapē. Papildinformāciju skatiet rakstā [Izejošā piegādes maršruts](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)

Lai izvairītos no scenārija, izmantojot pārraides pūlu, pārliecinieties, vai pārsūtītie/pārsūtītie ziņojumi atbilst vienam no šiem kritērijiem:

- Izejošais sūtītājs ir nomnieka akceptētais domēns.
- Sūtītāja politikas struktūra (Sender Policy Framework – SPF) nodod šādu Microsoft 365.
- DomainKeys identificētais pasts (DomainKeys Identified Mail – DKIM) P2 sūtītāja domēnā tiek nododams, kad ziņojums Microsoft 365.
 
Ziņojumi, kas atbilst iepriekš minētajiem kritērijiem, netiek izlaisti caur pārraides pūlu.

Ja jūsu domēna MX ieraksts norāda uz trešās puses vai lokālo serveri, izmantojiet uzlaboto filtrēšanu, lai pārliecinātos, vai SPF validācija ir pareiza ienākošajiem e-pasta ziņojumiem un izvairītos no e-pasta sūtīšanas caur pārraides pūlu.

**Kā noteikt, vai pārraides pūls ietekmēs mūs?**

Ja pārsūtītie vai izlaistie e-pasta ziņojumi izmanto kādu no iepriekš minētajiem kritērijiem, ziņojumi netiks pārsūtīti caur pārraides pūlu. Taču, ja ziņojums tiek nosūtīts caur pārraides pūlu, izejošā servera IP adrese atrodas diapazonā 40.95.0.0/16 un izejošā servera nosaukumā ir iekļauts **rly.**

