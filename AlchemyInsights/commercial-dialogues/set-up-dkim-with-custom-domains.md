---
title: DKIM iestatīšana ar pielāgotiem domēniem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/22/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002531"
- "7375"
ms.openlocfilehash: cb1f621dffc88464c339b55998efb5440cfd775c
ms.sourcegitcommit: ab75f66355116e995b3cb5505465b31989339e28
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/13/2021
ms.locfileid: "58332314"
---
# <a name="set-up-dkim-with-custom-domains"></a>DKIM iestatīšana ar pielāgotiem domēniem

Jums ir jāpublicē divi CNAME ieraksti katram pielāgotajam domēnam DNS. Lai to izdarītu, izmantojiet šādu formātu:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
**Piezīme.** **DomainGUID** ir teksts pa kreisi no **.mail.protection.outlook.com** pielāgotajā MX ierakstā pielāgotajam domēnam (piemēram, contoso-com domēnam **contoso.com).** **InitialDomain** ir domēns, ko izmantojāt, kad reģistrējāties Office 365 (piemēram, **contoso.onmicrosoft.com**).

Papildinformāciju par DNS ierakstiem skatiet rakstā DNS ierakstu izveide jūsu dns viesošanas [pakalpojumu sniedzēja Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)