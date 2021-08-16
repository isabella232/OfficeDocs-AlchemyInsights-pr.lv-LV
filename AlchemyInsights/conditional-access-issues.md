---
title: Nosacījum piekļuves problēmas
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
ms.openlocfilehash: 85cbd89e461f36a51eed816619fd132ea60dfdb0014eb850c7ec3f38d41e1ca2
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54069971"
---
# <a name="conditional-access-issues"></a>Nosacījum piekļuves problēmas

**Ar pierakstīšanās diagnostiku saistītas problēmas**

Varat ātri noskaidrot, kas noticis vai diagnosticētas problēmas saistībā ar lietotāju pierakstīību, izmantojot [pierakstīšanās diagnostiku:](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)

1. Palaidiet pierakstīšanās diagnostiku.
1. Atrodiet analizējamu notikumu, ievadot detalizētu informāciju par lietotāju, lietojumprogrammu, pierakstīšanās laiku, pieprasījuma ID vai korelācijas ID.
1. Pārskatiet diagnostikas rezultātus, parādot detalizētu informāciju par to, kas noticis, un kādas darbības varat veikt, lai veiktu izmaiņas (ja ir nepieciešamas kādas izmaiņas).

**Darbības, kas jāveic, lai novērstu pierakstīšanās problēmas** 

1. Naviģējiet uz Azure AD pierakstīšanās lapu.
1. Filtrējiet pierakstīšanās pēc lietotāja, laika diapazona, lietojumprogrammas, statusa, klienta lietojumprogrammas utt.
1. Atlasiet pierakstīšanās notikumu un skatiet cilni Nosacījuma piekļuve, lai skatītu, kuras politikas tika novērtētas.
1. Noklikšķiniet uz politikas rindas, lai skatītu detalizētu informāciju par politiku un izprastu tās lietošanas iemeslu.

**Rīki nosacījum piekļuves politikas problēmu novēršana**

- Tikai atskaišu režīms sniedz iespēju novērtēt politiku, neietekmējot lietotājus.
- Iespēju rīks sniedz iespēju simulēt pierakstīšanās notikumus un skatīt, kuras politikas tiek lietotas.
- Ieskati un atskaišu izveides darbgrāmatā redzama katras politikas reāllaika ietekme.

**Bāzlīniju aizsardzības politikas**

Bāzlīniju aizsardzības politikas ir novecojušas. Tās vairs netiek ieviestas un drīzumā tiks noņemtas no Azure portāla. Iesakām iespējot drošības [noklusējumus.](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)

Papildinformāciju par nosacījum piekļuvi skatiet rakstā:

[Paraugprakse attiecībā uz nosacījum piekļuvi programmā Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Vadīklas nosacījumformatēšanas programmā](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Atrašanās vietas nosacījuma piekļuves](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)
