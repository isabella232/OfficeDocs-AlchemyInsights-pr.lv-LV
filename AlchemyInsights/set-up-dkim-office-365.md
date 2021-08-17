---
title: Iestatīt DKIM
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
ms.openlocfilehash: 5dc90965516cc4d360b9be56c7737c6d134123ea8ac263b092559dd1416faff4
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54108563"
---
# <a name="setup-dkim"></a>Iestatīt DKIM

Pilnīgas instrukcijas DKIM konfigurēšanai pielāgotiem domēniem pakalpojumā Microsoft 365 [šeit.](https://docs.microsoft.com/microsoft-365/security/office-365-security/use-dkim-to-validate-outbound-email#steps-you-need-to-do-to-manually-set-up-dkim)

1. Katram **pielāgotajam** domēnam ir jāizveido **divi** DKIM CNAME ieraksti domēna DNS viesošanas pakalpojumā (parasti domēnu reģistrētājs). Piemēram, contoso.com un fourthcoffee.com nepieciešami četri DKIM CNAME ieraksti: divi contoso.com divi fourthcoffee.com.

   DKIM CNAME ieraksti katram **pielāgotajam domēnam** izmanto šādus formātus:

   - **Resursdatora nosaukums:**`selector1._domainkey.<CustomDomain>`

     **Norāda uz adresi vai vērtību:**`selector1-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   - **Resursdatora nosaukums:**`selector2._domainkey.<CustomDomain>`

     **Norāda uz adresi vai vērtību:**`selector2-<DomainGUID>._domainkey.<InitialDomain>`

     **TTL:** 3600

   \<DomainGUID\> ir teksts pa kreisi no pielāgotā MX ieraksta pielāgotajam domēnam `.mail.protection.outlook.com` (piemēram, `contoso-com` domēna nosaukumam contoso.com). \<InitialDomain\>ir domēns, ko izmantojāt, kad reģistrējāties Microsoft 365 (piemēram, contoso.onmicrosoft.com).

2. Kad esat izveidojis CNAME ierakstus saviem pielāgotajiem domēniem, izpildiet šos norādījumus:

   a. [pierakstieties pakalpojumā Microsoft 365](https://support.office.microsoft.com/article/e9eb7d51-5430-4929-91ab-6157c5a050b4) ar savu darba vai mācību kontu.

   b. Augšējā kreisajā stūrī atlasiet lietojumprogrammu palaidēja ikonu un izvēlieties **Administrators.**

   c. Apakšējā kreisajā navigācijas sadaļā izvērsiet Administrēšana **un** izvēlieties **Exchange**.

   d. Dodieties **uz aizsardzības**  >  **DKIM**.

   e. Atlasiet domēnu un pēc tam pie **Parakstiet** **šī domēna ziņojumus ar DKIM parakstiem izvēlieties Iespējot.** Atkārtojiet šo darbību katram pielāgotajam domēnam.
