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
ms.openlocfilehash: bb19f0672a21ea8b99c433ad83db4d89536c9a1705245fd2a683471170ab51ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53994827"
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
> [!NOTE]
> **DomainGUID** ir teksts pa kreisi no **.mail.protection.outlook.com** pielāgotā MX ieraksta pielāgotajam domēnam (piemēram, contoso-com domēnam **contoso.com**). **InitialDomain** ir domēns, ko izmantojāt, kad reģistrējāties Office 365 (piemēram, **contoso.onmicrosoft.com**).

Papildinformāciju par DNS ierakstiem skatiet rakstā [DNS ierakstu izveide pakalpojumu sniedzējam, kas nodrošina Office 365.](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider)