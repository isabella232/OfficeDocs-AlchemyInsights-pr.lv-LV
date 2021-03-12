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
ms.openlocfilehash: c448956f0dad0738f4de7507ec4686c738a90a55
ms.sourcegitcommit: 6312ee31561db36104f32282d019d069ede69174
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745254"
---
# <a name="set-up-dkim-with-custom-domains"></a>DKIM iestatīšana ar pielāgotiem domēniem

Katram pielāgotam domēnam DNS ir jāpublicē divi CNAME ieraksti. Lai to izdarītu, izmantojiet šādu formātu:

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> **DomainGUID** ir teksts, kas atrodas pa kreisi no **. Mail.Protection.Outlook.com** pielāgoto domēnu (piemēram, contoso-com for Domain **contoso.com**) pielāgoto MX ierakstu. **InitialDomain** ir domēns, ko izmantojāt, reģistrējoties pakalpojumā Office 365 (piemēram, **contoso.onmicrosoft.com**).

Lai iegūtu papildinformāciju par DNS ierakstiem, skatiet rakstu [DNS ierakstu izveide pie jebkura DNS viesošanas pakalpojumu sniedzēja pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).