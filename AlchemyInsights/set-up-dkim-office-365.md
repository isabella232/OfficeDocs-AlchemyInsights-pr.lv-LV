---
title: DKIM Office 365 uzstādīšanas
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1388
ms.assetid: ''
ms.openlocfilehash: 0f81fe02135f3d0901ffe5a26d7aa3dad70c3770
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34765231"
---
# <a name="setup-dkim-in-office-365"></a>DKIM Office 365 uzstādīšanas

Pilnīgas instrukcijas konfigurēšanai DKIM pielāgotiem domēniem Office 365 ir [šeit](https://docs.microsoft.com/office365/SecurityCompliance/use-dkim-to-validate-outbound-email#what-you-need-to-do-to-manually-set-up-dkim-in-office-365).

1. Par **katru** pielāgoto domēnu, jums ir nepieciešams, lai izveidotu **divas** DKIM CNAME ierakstu jūsu domēna DNS viesošanas pakalpojumā (parasti, domēnu reģistrators). Piemēram, contoso.com un fourthcoffee.com prasīt četrus DKIM CNAME ierakstu: divi contoso.com un divus fourthcoffee.com.

   DKIM CNAME ierakstus par **katru** pielāgoto domēnu izmantot šādus formātus:

   - **Host nosaukums**:`selector1._domainkey.<CustomDomain>`

     **Norāda uz adresi vai vērtību**:`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   - **Host nosaukums**:`selector2._domainkey.<CustomDomain>`

     **Norāda uz adresi vai vērtību**:`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL**: 3600

   \<DomainGUID\> ir pa kreisi no teksta `.mail.protection.outlook.com` pielāgotu MX ierakstā par pielāgoto domēnu (piemēram, `contoso-com` par domēnu contoso.com). \<InitialDomain\> ir domēnu izmantojāt reģistrējoties Office 365 (piemēram, contoso.onmicrosoft.com).

2. Pēc tam, kad esat izveidojis CNAME ierakstu jūsu pielāgoto domēnu, izpildiet šādus norādījumus:

   a. [Office 365 pierakstīties](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) ar jūsu darba vai skolas konts.

   b. Atlasiet app granātmetējs ikonu augšējā kreisajā un izvēlieties **Admin**.

   c. Apakšējā kreisajā navigācijas, izvērsiet **Admin** un izvēlieties **Exchange**.

   d. Dodieties uz **aizsardzības** > **DKIM**.

   e. Atlasiet domēnu un pēc tam izvēlieties **Iespējot** **parakstīt**ziņojumu šim domēnam ar DKIM parakstiem. Atkārtojiet šo darbību ar katru pielāgoto domēnu.
