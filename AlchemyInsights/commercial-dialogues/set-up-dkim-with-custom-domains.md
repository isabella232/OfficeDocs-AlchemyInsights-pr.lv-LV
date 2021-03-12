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
# <a name="set-up-dkim-with-custom-domains"></a><span data-ttu-id="1f914-102">DKIM iestatīšana ar pielāgotiem domēniem</span><span class="sxs-lookup"><span data-stu-id="1f914-102">Set up DKIM with custom domains</span></span>

<span data-ttu-id="1f914-103">Katram pielāgotam domēnam DNS ir jāpublicē divi CNAME ieraksti.</span><span class="sxs-lookup"><span data-stu-id="1f914-103">You must publish two CNAME records for each custom domain in DNS.</span></span> <span data-ttu-id="1f914-104">Lai to izdarītu, izmantojiet šādu formātu:</span><span class="sxs-lookup"><span data-stu-id="1f914-104">To do this, use the following format:</span></span>

```console
Host name:            selector1._domainkey
Points to address or value:    selector1-<domainGUID>._domainkey.<initialDomain>
TTL:                3600

Host name:            selector2._domainkey
Points to address or value:    selector2-<domainGUID>._domainkey.<initialDomain>
TTL:                3600
```
> [!NOTE]
> <span data-ttu-id="1f914-105">**DomainGUID** ir teksts, kas atrodas pa kreisi no **. Mail.Protection.Outlook.com** pielāgoto domēnu (piemēram, contoso-com for Domain **contoso.com**) pielāgoto MX ierakstu.</span><span class="sxs-lookup"><span data-stu-id="1f914-105">**DomainGUID** is the text to the left of **.mail.protection.outlook.com** in the customized MX record for the custom domain (for example, contoso-com for the domain **contoso.com**).</span></span> <span data-ttu-id="1f914-106">**InitialDomain** ir domēns, ko izmantojāt, reģistrējoties pakalpojumā Office 365 (piemēram, **contoso.onmicrosoft.com**).</span><span class="sxs-lookup"><span data-stu-id="1f914-106">**InitialDomain** is the domain you used when you signed up for Office 365 (for example, **contoso.onmicrosoft.com**).</span></span>

<span data-ttu-id="1f914-107">Lai iegūtu papildinformāciju par DNS ierakstiem, skatiet rakstu [DNS ierakstu izveide pie jebkura DNS viesošanas pakalpojumu sniedzēja pakalpojumā Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span><span class="sxs-lookup"><span data-stu-id="1f914-107">For more information about DNS records, see [Create DNS records at any DNS hosting provider for Office 365](https://docs.microsoft.com/microsoft-365/admin/get-help-with-domains/create-dns-records-at-any-dns-hosting-provider).</span></span>