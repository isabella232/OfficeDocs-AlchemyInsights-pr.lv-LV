---
title: Setup DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0acaed476dbd06bc933bf466f9bf6116413a44bb
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44509391"
---
# <a name="setup-dkim"></a>Setup DKIM

Pilnu instrukciju konfigurēšana DKIM pielāgotu domēnu Microsoft 365 ir [šeit](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. **Katram** pielāgotajam domēnam ir jāizveido **divi** DKIM CNAME ieraksti domēna DNS viesošanas pakalpojumā (parasti domēna reģistrētājā). Piemēram, contoso.com un fourthcoffee.com nepieciešami četri DKIM CNAME ieraksti: divi contoso.com un divi fourthcoffee.com.

   DKIM CNAME ierakstus **katram** pielāgotajam domēnam izmantot šādus formātus:

   - **Resursdatora nosaukums**:`selector1._domainkey.<CustomDomain>`

     **Norāda uz adresi vai vērtību**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Resursdatora nosaukums**:`selector2._domainkey.<CustomDomain>`

     **Norāda uz adresi vai vērtību**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\>ir teksts pa kreisi no `.mail.protection.outlook.com` Pielāgotā domēna PIELĀGOTĀ MX ieraksta (piemēram, `contoso-com` domēna contoso.com). \<InitialDomain\>ir domēns, ko izmantojāt, kad reģistrījāties Microsoft 365 (piemēram, contoso.onmicrosoft.com).

2. Kad esat izveidojis CNAME ierakstus pielāgotajiem domēniem, izpildiet tālāk sniegtos norādījumus.

   A. [pierakstieties Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) ar savu darba vai skolas kontu.

   B. Augšējā kreisajā stūrī atlasiet programmas palaidēja ikonu un izvēlieties **admin**.

   C. Apakšējā kreisajā navigācijas, izvērsiet **admin** un izvēlieties **Exchange**.

   D. Iet uz **aizsardzība**  >  **DKIM**.

   E. Atlasiet domēnu un pēc tam izvēlieties **Iespējot** , lai **parakstītu ziņojumus šim domēnam ar DKIM parakstiem**. Atkārtojiet šo darbību katram pielāgotajam domēnam.
