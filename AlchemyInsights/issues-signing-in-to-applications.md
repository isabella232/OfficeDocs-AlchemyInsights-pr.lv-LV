---
title: Problēmas saistībā ar pierakstīšanos lietojumprogrammās
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7788"
- "9004355"
ms.openlocfilehash: 2d073367dc1c3e8e117c0b68e205297a65024872
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901030"
---
# <a name="issues-signing-in-to-applications"></a>Problēmas saistībā ar pierakstīšanos lietojumprogrammās

Lai noteiktu iemeslus vai diagnosticētu problēmas, kas saistītas ar lietotāja pierakstīšanos, veiciet tālāk norādītās darbības.

1. Palaidiet [pierakstīšanās diagnostiku](https://ms.portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).
2. Atrodiet notikumu, kas jāanalizē, ievadot detalizētu informāciju par lietotāju, lietojumprogrammu, pierakstīšanās laiku, pieprasījuma ID vai korelācijas ID.
3. Pārskatiet diagnostikas rezultātus, parādot detalizētu informāciju par to, kas noticis, un kādas darbības, ko varat veikt, lai veiktu izmaiņas, ja nepieciešamas jebkādas izmaiņas.

Tālāk norādītas dažas bieži sastopamas problēmas, kas var rasties, pierakstoties lietojumprogrammās:

1. Jūs vai lietotājs **ir pabeigusi AZURE ad pierakstīšanos, bet tiek rādīts neparedzēts uzaicinājums** — raksti [negaidīta piekrišana, pierakstoties lietojumprogrammā](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt) un [neparedzēta kļūda, kad veicat piekrišanu lietojumprogrammai](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error).
2. Jūs vai lietotājs **ir pierakstījies lietojumprogrammā tieši, taču nevarat tajā pierakstīties no deeplink pielāgotajā portālā vai piekļuves panelī**: skatiet rakstu problēmu novēršana saistībā ar [pierakstīšanos lietojumprogrammā Azure AD manas lietojumprogrammas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel).
3. Jūs vai lietotājs **ir pabeidzis AZURE ad pierakstīšanos, bet lietojumprogrammā tiek rādīts kļūdas ziņojums un tas neļauj lietotājam pabeigt pierakstīšanās plūsmu**: problēma ir tā, ka lietojumprogramma neakceptēja Azure AD izdoto atbildi. Lai novērstu problēmas, veiciet [tālāk norādītās darbības](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-application-error) .
4. Jūs vai lietotājs **nevar pierakstīties programmā, kas nav galerija un ir konfigurēta, lai veiktu paroļu vienotās pierakstīšanās**: izpildiet [šīs darbības](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) , lai novērstu problēmu.
5. Jūs vai lietotājs **nevar pierakstīties AZURE ad Gallery lietojumprogrammā, kas konfigurēta, lai veiktu paroļu vienotās pierakstīšanās**: veiciet [tālāk norādītās darbības](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso) , lai novērstu problēmas.
6. Jūs vai lietotājs **nevar pierakstīties Microsoft lietojumprogrammā**: veiciet [tālāk norādītās darbības](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft) , lai novērstu problēmas.
7. Jūs vai lietotājs **nevar pierakstīties programmā, kas nav galerija un kura ir konfigurēta integrētās vienotās pierakstīšanās gadījumā**: veiciet [tālāk norādītās darbības](https://docs.microsoft.com/azure/active-directory/application-sign-in-problem-federated-sso-non-gallery) , lai novērstu problēmas.
8. Jūs vai lietotājs **nevar pierakstīties AZURE ad Gallery lietojumprogrammā, kas konfigurēta integrētās vienotās pierakstīšanās gadījumā**: izpildiet [šīs darbības](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) , lai novērstu problēmas.
9. Jūs vai lietotājs **nevar pierakstīties pielāgotā lietojumprogrammā**: veiciet [tālāk norādītās darbības](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery) , lai novērstu problēmas.
10. Jūs vai lietotājs **nevar pierakstīties lokālajā lietojumprogrammā, kas izmanto AZURE ad lietojumprogrammas starpniekserveri**: veiciet [tālāk norādītās darbības](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-on-premises-application-proxy) , lai novērstu problēmas.

