---
title: Autentifikācijas programma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405065"
---
# <a name="authentication-app"></a>Autentifikācijas programma

Ja esat globālais administrators, varat ātri uzzināt, kas noticis vai diagnosticētas problēmas saistībā ar lietotāju pierakstīšanu, izmantojot pierakstīšanās [diagnostiku.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Sāciet diagnostiku, noklikšķinot uz[pogas "Palaist diagnostiku".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Atrodiet analizējamu notikumu, ievadot detalizētu informāciju par lietotāju, lietojumprogrammu, pierakstīšanās laiku, pieprasījuma ID vai korelācijas ID.
1. Pārskatiet diagnostikas rezultātus, parādot detalizētu informāciju par to, kas noticis, un kādas darbības varat veikt, lai veiktu izmaiņas, ja ir nepieciešamas kādas izmaiņas.

**Skatiet attiecināmo scenāriju:**

1. Ja lietotājs nesaņem pašpiegādes paziņojumu programmā Microsoft Authenticator, pārbaudiet, vai tie netiek rādīti MFA bloķēto lietotāju sarakstā, kā aprakstīts rakstā Lietotāju bloķēšana [un atbloķēšana.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Ja lietotājs nav bloķēts MFA, bet nesaņem pašpiegādes paziņojumu, viņš var atvērt programmu Microsoft Authenticator, kas izvilks gaidošos apstiprināšanas pieprasījumus.
1. Kā alternatīvu pierakstīšanās metodi lietotājs var arī noklikšķināt uz Pierakstīties citā veidā un izvēlēties izmantot pārbaudes kodu manā mobilajā lietojumprogrammā.
1. Programma Microsoft Authenticator ir vienīgā pieejamā metode daudziem lietotājiem. [Uzziniet vairāk par drošības noklusējumus](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)— skatiet bieži uzdotos jautājumus par autentificētāja lietojumprogrammu — bieži uzdotos jautājumus un to atrisināšanu. [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq)
 
**Ieteicamie video**

[Kā iestatīt programmu Authenticator jaunā tālrunī (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
