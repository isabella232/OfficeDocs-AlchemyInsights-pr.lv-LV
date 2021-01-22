---
title: Nemanāmi SSO lietotāja pierakstīšanās problēmas
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "7811"
ms.openlocfilehash: 347ef8f8176583f2a7c15fa82435eeb118b58c39
ms.sourcegitcommit: 67c873fa6e23ec39a826d60ac830969073bf79e1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935174"
---
# <a name="seamless-sso-user-sign-in-issues"></a>Nemanāmi SSO lietotāja pierakstīšanās problēmas

Pēc tam, kad lietotājs ir autentificēts, pārlūkprogrammā tiks kešatmiņas lietotāja akreditācijas dati, lai tajā pašā pārlūkprogrammā lietojumprogramma automātiski pierakstītos ar to pašu kontu. Tādējādi citam lietotājam vai vienam lietotājam var būt grūti pieteikties vairākos kontos vienā ierīcē. Lai atrisinātu šo: 1. Mēģiniet pierakstīties citā pārlūkprogrammā. 2. Iztīriet pārlūkprogrammas kešatmiņu un/vai sīkfailus un vēlreiz mēģiniet pierakstīties.

Ja joprojām rodas pierakstīšanās problēmas, iesakām veikt tālāk norādītās darbības, lai diagnosticētu un automatizētu risināšanas darbības:

1. Instalējiet [manas lietojumprogrammas drošas pārlūkprogrammas paplašinājumu](https://docs.microsoft.com/azure/active-directory/manage-apps/access-panel-extension-problem-installing) , lai palīdzētu Azure Active Directory (Azure AD) nodrošināt labāku diagnosticēšanu un atrisinājumus, izmantojot Azure portālā pieejamās pārbaudes iespējas.
2. Atveidojiet kļūdu, izmantojot testēšanas pieredzi Azure portāla programmas konfigurācijas lapā. Lai uzzinātu vairāk, skatiet rakstu [SAML vienotās pierakstīšanās lietojumprogrammu atkļūdošana](https://docs.microsoft.com/azure/active-directory/azuread-dev/howto-v1-debug-saml-sso-issues).
3. Ja izmantojat Azure portālā esošo testēšanas pieredzi ar drošas pārlūkprogrammas paplašinājumu manas lietojumprogrammas, varat **Izlaist 4. darbību**.
4. Lai atvērtu SAML vienotās pierakstīšanās konfigurācijas lapu:
    - Atveriet [Azure portālu](https://portal.azure.com/) un pierakstieties kā **globālais administrators** vai **līdzadministrators**.
    - Atveriet **Azure Active Directory paplašinājumu** , noklikšķinot uz **Visi pakalpojumi** galvenā kreisās puses navigācijas izvēlnes augšpusē.
    - Filtra meklēšanas lodziņā ierakstiet "Azure Active Directory" un atlasiet **Azure Active Directory** vienumu.
    - Atlasiet **uzņēmuma lietojumprogrammas** Azure Active Directory kreisās puses navigācijas izvēlnē.
    - Atlasiet **Visas programmas** , lai skatītu visu savu lietojumprogrammu sarakstu. Ja neredzat lietojumprogrammu, kuru vēlaties parādīt, izmantojiet **filtra** vadīklu **saraksta visas lietojumprogrammas** augšdaļā un iestatiet opciju **Rādīt** **visām lietojumprogrammām**.
    - Atlasiet lietojumprogrammu, kuru vēlaties konfigurēt, lai veiktu vienotās pierakstīšanās.
    - Pēc lietojumprogrammas ielādes atlasiet **vienotā pierakstīšanās** lietojumprogrammas kreisās puses navigācijas izvēlnē.
    - Atlasiet **SAML**.
5. Atkarībā no kļūdas, lai uzzinātu vairāk par ieteicamajām darbībām, skatiet rakstu problēmas, [Pierakstoties SAML, izmantojot atsevišķas pierakstīšanās lietojumprogrammas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery#application-not-found-in-directory).
6. Lai novērstu citas lietotāja pierakstīšanās problēmas, skatiet šos norādījumus:
    - [Viens Sign-On SAML protokols](https://docs.microsoft.com/azure/active-directory/develop/single-sign-on-saml-protocol)
    - [Pierakstīšanās kļūdu problēmu novēršana, izmantojot Azure Active Directory atskaites](https://docs.microsoft.com/azure/active-directory/reports-monitoring/howto-troubleshoot-sign-in-errors)
    - [Negaidīta piekrišanas uzvedne](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-prompt)
    - [Lietotāja piekrišanas kļūda](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)
    - [Problēmas, pierakstoties no manas lietojumprogrammas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-other-problem-access-panel)
    - [Kļūda lietojumprogrammas pierakstīšanās lapā](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-application-error)
    - [Problēma, pierakstoties Microsoft lietojumprogrammā](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-first-party-microsoft)
