---
title: Ierobežotas piekļuves problēmas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014885"
---
# <a name="conditional-access-issues"></a>Ierobežotas piekļuves problēmas

**Problēmu novēršana saistībā ar pierakstīšanās diagnostiku**

Varat ātri noskaidrot, kas notika vai diagnosticēt problēmas, kas saistītas ar lietotāja pierakstīšanos, izmantojot [pierakstīšanās diagnostiku](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):

1. Palaidiet pierakstīšanās diagnostiku.
1. Meklēšanas notikuma atrašana, ievadot detalizētu informāciju par lietotāju, lietojumprogrammu, pierakstīšanās, pieprasījuma ID vai korelācijas ID.
1. Pārskatiet diagnostikas rezultātus, parādot detalizētu informāciju par to, kas noticis un kādas darbības varat veikt, lai veiktu izmaiņas (ja nepieciešamas izmaiņas).

**Darbības, kas jāveic, lai novērstu pierakstīšanos** 

1. Pārejiet uz Azure AD pierakstīšanās lapu.
1. Filtrējiet pierakstīšanās pēc lietotāja, laika diapazona, lietojumprogrammas, statusa, klienta lietojumprogrammas un tā tālāk.
1. Atlasiet pierakstīšanās notikumu un skatiet cilni nosacījuma piekļuve, lai skatītu, kuras politikas ir novērtētas.
1. Noklikšķiniet uz politikas rindas, lai skatītu detalizētu informāciju par politiku un saprastu, kāpēc tā tiek lietota.

**Rīki, kas novērš nosacījuma piekļuves politiku**

- Tikai atskaišu režīms ļauj novērtēt politiku, neietekmējot lietotājus.
- Iespēju rīks ļauj simulēt pierakstīšanās notikumus un skatīt, kuras politikas tiek lietotas.
- Ieskatu un ziņošanas darbgrāmatā parāda katras politikas reāllaika ietekmi.

**Bāzlīnijas aizsardzības politikas**

Pamata aizsardzības politika ir novecojusi. Tie vairs netiek ieviesti un drīzumā tiks noņemti no Azure portāla. Iesakām iespējot [drošības noklusējumus](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).

Papildinformāciju par ierobežotu piekļuvi skatiet rakstā:

[Labākā prakse nosacījuma piekļuvei Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Nosacījuma piekļuves nosacījumi](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ierobežotas piekļuves vadīklas](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Ierobežotas piekļuves atrašanās vietas](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
