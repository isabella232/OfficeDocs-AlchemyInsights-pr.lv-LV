---
title: OIDC vienotās pierakstīšanās (SSO) problēmu novēršana
ms.author: v-jmathew
author: v-jmathew
manager: scotv
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004357"
- "9375"
ms.openlocfilehash: 5880ee37a2fcc98b34231cc9960fb3f87fa184b07bd81ccd37d0ea5a78170af0
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54105785"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC vienotās pierakstīšanās (SSO) problēmu novēršana

- Lai uzzinātu, kā Azure nomniekam pievienot OIDC lietojumprogrammu, skatiet rakstu Īsā pamācība: OIDC vienotās pierakstīšanās [(Single sign-on — SSO) iestatīšana lietojumprogrammai Azure Active Directory (Azure AD) nomniekā.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso)
- Papildinformāciju par lietojumprogrammām, kas izmanto OpenID Savienošana vienotās pierakstīšanās ieviešanai, skatiet rakstā [OIDC](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on)vienotās pierakstīšanās izpratne.
- Informāciju gadījumā, ja izvēlaties rakstīt kodu, tieši nosūtot un apstrādājot HTTP pieprasījumus, vai izmantojat trešās puses atklātā pirmkoda bibliotēku, nevis kādu no mūsu atklātā pirmkoda bibliotēkām, skatiet rakstu [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols)un OpenID Savienošana protokoli Microsoft indentitāšu platforma.

**Protokoli**

1. [Microsoft indentitāšu platforma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) un netieša piešķires plūsma — definēšanas pazīme netiešās piešķiršanas iezīme ir tā, ka marķieri (ID marķieri vai piekļuves marķieri) tiek atgriezti tieši no /authorize galapunkta, nevis /marķiera galapunkta. To bieži izmanto kā daļu no autorizācijas koda plūsmas jeb **"hibrīdās plūsmas"**— ID marķiera izgūšanu /autorizējot pieprasījumā kopā ar autorizācijas kodu . Šajā rakstā ir aprakstīts, kā tieši programmai lietot lietojumprogrammas protokolu pieprasīt marķierus no Azure AD.
2. Microsoft indentitāšu platforma un [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) autorizācijas koda plūsma — autorizācijas koda OAuth 2.0 piešķiri var izmantot ierīcē instalētās lietojumprogrammās, lai piekļūtu aizsargātiem resursiem, piemēram, tīmekļa API. Izmantojot OAuth 2.0 Microsoft indentitāšu platforma ieviešanu, varat pievienot pierakstīšanās un API piekļuvi savām mobilajām un datora **programmām.** Šajā rakstā ir paskaidrots, kā tieši veikt programmi, salīdzinot ar protokolu jūsu lietojumprogrammā, izmantojot jebkuru valodu.
3. Microsoft indentitāšu platforma un [OpenID Savienošana](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) protokols — ja Microsoft indentitāšu platforma lieto OpenID Savienošana ieviešanu, varat pievienot pierakstīšanās un API piekļuvi savām lietojumprogrammām. Šajā rakstā paskaidrots, kā veikt šīs darbības neatkarīgi no valodas, kā arī aprakstīts, kā nosūtīt un saņemt HTTP ziņojumus, neizmantojot Microsoft atklātā **pirmkoda bibliotēkas.**
4. Microsoft indentitāšu platforma un [OAuth 2.0](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) klienta akreditācijas datu plūsma — varat izmantot OAuth 2.0 klienta akreditācijas datu piešķiršanu, kas norādīta pakalpojumā RFC 6749 (dažreiz dēvēta par divkāršo **OAuth),** lai piekļūtu tīmeklī viesotiem resursiem, izmantojot lietojumprogrammas identitāti. Šāda veida piešķiršana parasti tiek izmantota mijiedarbībai starp serveriem, kas ir jāveic fona režīmā, nekavējot mijiedarbību ar lietotāju. Šāda veida lietojumprogrammas bieži sauc par **dēmoniem vai** **pakalpojumu kontiem.** Šajā rakstā ir paskaidrots, kā tieši programmai izmantot protokolu jūsu lietojumprogrammā.
