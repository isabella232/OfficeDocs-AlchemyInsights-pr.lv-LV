---
title: SSO savienojuma problēmas
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
- "7810"
ms.openlocfilehash: 33074d70377866332feeccfb8b6400eff2de5a73
ms.sourcegitcommit: e188ec7a583837a3e07880d05b3607b8bdac729c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/21/2021
ms.locfileid: "49935152"
---
# <a name="sso-connection-issues"></a>SSO savienojuma problēmas

1. Izpildiet [Quickstart: konfigurējiet](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure) lietojumprogrammas rokasgrāmatas rekvizītus, lai konfigurētu lietojumprogrammu.
2. Atkarībā no izmantotās lietojumprogrammas un [vienotās pierakstīšanās opcijas](https://docs.microsoft.com/azure/active-directory/manage-apps/sso-options) veiciet tālāk norādītās darbības.
    - Lai konfigurētu **lokālo lietojumprogrammu** **SAML vienotās pierakstīšanās** vajadzībām, skatiet [SAML Single-Sign-On lokālās lietojumprogrammas, izmantojot lietojumprogrammas starpniekserveri](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-on-premises-apps).
    - Lai konfigurētu **mākoņa lietojumprogrammu** ar **paroli pamatotai vienotā pierakstīšanās** lietošanai, skatiet rakstu  [paroles vienotās](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-password-single-sign-on-non-gallery-applications)pierakstīšanās konfigurēšana.
    - Lai konfigurētu **lokālo lietojumprogrammu** **vienotās pierakstīšanās lietošanai, izmantojot lietojumprogrammu starpniekserveri**, skatiet rakstu [paroļu velves izveide vienotā pierakstīšanās ar lietojumprogrammas starpniekserveri](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-configure-single-sign-on-password-vaulting).
3. **Lietojumprogrammas starpniekservera problēmu novēršana**: iesakām sākt ar problēmu novēršanas plūsmu pārskatīšanu, [atkļūdošanas lietojumprogrammas starpniekservera savienotāja problēmas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-connectors), lai noteiktu, vai lietojumprogrammas starpniekservera savienotāji ir pareizi konfigurēti. Ja joprojām rodas problēmas, veidojot savienojumu ar lietojumprogrammu, izpildiet problēmu novēršanas plūsmu [atkļūdošanas lietojumprogrammas starpniekservera lietojumprogrammas problēmas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-debug-apps). [CORS problēmas varat identificēt](https://docs.microsoft.com/azure/active-directory/manage-apps/application-proxy-understand-cors-issues#understand-and-identify-cors-issues) , izmantojot pārlūka atkļūdošanas rīkus.
    - Palaidiet pārlūkprogrammu un pārlūkojiet līdz tīmekļa programmai.
    - Nospiediet taustiņu **F12** , lai atvērtu atkļūdošanas konsoli.
    - Mēģināt reproducēt transakciju un pārskatīt konsoles ziņojumu. CORS pārkāpums izveido konsoles kļūdu par izcelsmi.
    - Dažas CORS problēmas nevar atrisināt, piemēram, kad lietojumprogramma novirza uz login.microsoft.com, lai autentificētu, un piekļuves pilnvaras derīguma termiņš beigsies. CORS pēc tam neizdosies. Risinājums šajā scenārijā ir pagarināt piekļuves marķiera kalpošanas laiku, lai neļautu tam beigties lietotāja sesijas laikā. Papildinformāciju par to, kā to paveikt, skatiet rakstā [konfigurējamas marķierierīces ilgumus Microsoft identitātes platformā](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
4. **SAML vienotās pierakstīšanās problēmu novēršana**: iesakām pārbaudīt problēmas, kas rodas [, pierakstoties, izmantojot SAML vienotās pierakstīšanās programmas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-problem-federated-sso-gallery), lai atrastu to problēmu risinājumus, kuras jūs, iespējams, saskārušies.
5. Ar **paroli pamatotas vienotās pierakstīšanās problēmu novēršana**: iesakām pārbaudīt ar [paroli pamatotas vienotās pierakstīšanās Azure AD](https://docs.microsoft.com/azure/active-directory/manage-apps/troubleshoot-password-based-sso), lai atrastu risinājumus problēmām, kuras jūs, iespējams, saskārušies.
6. Savienojuma problēmas, izmantojot VPN, skatiet rakstā [vienotās pierakstīšanās (SSO) izmantošana pa VPN un Wi-Fi savienojumiem](https://docs.microsoft.com/windows/security/identity-protection/vpn/how-to-use-single-sign-on-sso-over-vpn-and-wi-fi-connections).
