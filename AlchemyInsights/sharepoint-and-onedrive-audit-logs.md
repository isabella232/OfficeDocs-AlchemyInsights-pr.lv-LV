---
title: Klasiskās SharePoint audita žurnālu atskaites
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662215"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a>SharePoint un OneDrive audita žurnāli

## <a name="sharepoint-classic-audit-logs"></a>SharePoint klasiskā audita žurnāli

SPO mantotā auditēšana ir migrēta uz vienotā audita žurnālu (UAL). Visas SPO mantotās auditēšanas atskaites tagad tiks darbinātas, izmantojot UAL, un mantotie audita signāli ir migrēti uz UAL.

Galvenās izmaiņas:

* Apgriešana nav pieejama kā iespēja.
* Konkrētu notikumu atlase auditam nav pieejama. [Šajā dokumentā](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) ir parādīts pilnīgs saraksts ar audita pasākumiem, kas pieejami pēc noklusējuma.
* Opcija **atrašanās vieta** sadaļā **pielāgotas atskaites** nav pieejama.
* Opcija **Atvērt vai lejupielādēt dokumentu** notikumus nav pieejama.

[Vietņu kolekcijas auditēšanas iestatījumu konfigurēšana](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a>SharePoint un OneDrive modernie vienotie audita žurnāli no atbilstības

* [Vienotās audita reģistrēšanas ieslēgšana/izslēgšana](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

Koplietošanas vidē SharePoint vai OneDrive papildu konfigurācija nav nepieciešama.

Izmantojiet audita reģistrēšanas meklēšanu, lai pārbaudītu failu (-s), mapju (-u), lietotāju (u), atļauju:

* [Failu un lapu darbības](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [Mapju darbības](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [Koplietošanas un piekļuves pieprasījumu darbības](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [Sinhronizēšanas darbības](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [Vietnes administrēšanas darbības](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

Papildinformāciju par to, kā izgūt šos notikumus, skatiet rakstā [meklēšana audita žurnālu](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).
