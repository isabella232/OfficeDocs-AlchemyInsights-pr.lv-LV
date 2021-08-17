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
ms.openlocfilehash: 1ac3158914455502d2de493dd1320034b1d09573ebb3ffef24c23eb1e816cad0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54082949"
---
# <a name="authentication-app"></a>Autentifikācijas programma

Ja esat globālais administrators, varat ātri uzzināt, kas noticis vai diagnosticētas problēmas saistībā ar lietotāju pierakstīšanu, izmantojot pierakstīšanās [diagnostiku.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Sāciet diagnostiku, noklikšķinot uz[pogas "Palaist diagnostiku".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom) 
1. Atrodiet analizējamu notikumu, ievadot detalizētu informāciju par lietotāju, lietojumprogrammu, pierakstīšanās laiku, pieprasījuma ID vai korelācijas ID.
1. Pārskatiet diagnostikas rezultātus, parādot detalizētu informāciju par to, kas noticis, un kādas darbības varat veikt, lai veiktu izmaiņas, ja ir nepieciešamas kādas izmaiņas.

**Skatiet attiecināmo scenāriju:**

1. Ja lietotājam netiek rādīts pašpiegādes paziņojums Microsoft Authenticator programmā, pārbaudiet, vai tie netiek rādīti MFA bloķēto lietotāju sadaļā, kā aprakstīts rakstā Lietotāju bloķēšana [un atbloķēšana.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)
1. Ja lietotājs nav bloķēts MFA, bet nesaņem pašpiegādes paziņojumu, viņš var atvērt programmu Microsoft Authenticator, kas izvilks gaidošos apstiprināšanas pieprasījumus.
1. Kā alternatīvu pierakstīšanās metodi lietotājs var arī noklikšķināt uz Pierakstīties citā veidā un izvēlēties izmantot pārbaudes kodu manā mobilajā lietojumprogrammā.
1. Lietojumprogramma Microsoft Authenticator ir vienīgā pieejamā metode daudziem lietotājiem. [Papildinformāciju par drošības noklusējumiem](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)skatiet sadaļā [Bieži Authenticator skatiet](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) bieži uzdotos jautājumus par lietojumprogrammām un to atrisināšanu.
 
**Ieteicamie video**

[Programmas Authenticator jaunā tālrunī (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)
