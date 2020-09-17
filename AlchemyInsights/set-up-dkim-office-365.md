---
title: Iestatīšanas DKIM
ms.author: chrisda
author: chrisda
manager: dansimp
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: b34bfdafcab6229a4dd2e9d9f23103fa13556482
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47808714"
---
# <a name="setup-dkim"></a>Iestatīšanas DKIM

Visi norādījumi par DKIM konfigurēšanu pielāgotiem domēniem pakalpojumā Microsoft 365 ir pieejami [šeit](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim).

1. **Katram** pielāgotam domēnam ir jāizveido **divi** DKIM CNAME ieraksti jūsu domēna DNS viesošanas pakalpojumā (parasti domēnu reģistrētājs). Piemēram, contoso.com un fourthcoffee.com prasa četrus DKIM CNAME ierakstus: divas for contoso.com un divas for fourthcoffee.com.

   DKIM CNAME ieraksti **katram** pielāgotam domēnam tiek izmantoti šādos formātos:

   - **Resursdatora nosaukums**: `selector1._domainkey.<CustomDomain>`

     **Norāda uz adresi vai vērtību**: `selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Resursdatora nosaukums**: `selector2._domainkey.<CustomDomain>`

     **Norāda uz adresi vai vērtību**: `selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> ir teksts, kas atrodas pa kreisi no pielāgotā `.mail.protection.outlook.com` domēna pielāgotā MX ieraksta (piemēram, `contoso-com` domēna contoso.com). \<InitialDomain\> ir domēns, ko izmantojāt, reģistrējoties Microsoft 365 (piemēram, contoso.onmicrosoft.com).

2. Pēc tam, kad esat izveidojis savam pielāgotajiem domēniem CNAME ierakstus, izpildiet šos norādījumus:

   izveide. [pierakstieties pakalpojumā Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) ar savu darba vai mācību iestādes kontu.

   b. Augšējā kreisajā stūrī atlasiet lietojumprogrammu palaidēja ikonu un izvēlieties **administrators**.

   c. Apakšējā kreisajā navigācijas rūtī izvērsiet **administrators** un izvēlieties **Exchange**.

   d. Dodieties uz **aizsardzības**  >  **DKIM**.

   e. Atlasiet domēnu un pēc tam izvēlieties **Iespējot** , lai **parakstītu ziņojumus šajā domēnā ar DKIM parakstiem**. Atkārtojiet šo darbību katram pielāgotam domēnam.
