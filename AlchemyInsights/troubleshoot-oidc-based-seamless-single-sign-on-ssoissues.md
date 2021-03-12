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
ms.openlocfilehash: e4ddde6176d9ab021b93e23b3cb363e10b1c1048
ms.sourcegitcommit: be246651064dfeacc866b2f69c0dbe4002a73f1c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2021
ms.locfileid: "50745025"
---
# <a name="troubleshoot-oidc-based-seamless-single-sign-on-sso-issues"></a>OIDC vienotās pierakstīšanās (SSO) problēmu novēršana

- Lai uzzinātu, kā pievienot OIDC lietojumprogrammu savam Azure nomniekam, skatiet rakstu [Quickstart: OIDC-bāzētās vienotās pierakstīšanās (SSO) iestatīšana lietojumprogrammas Azure Active Directory (AZURE AD) nomniekā](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-setup-oidc-sso).
- Papildinformāciju par programmām, kas izmanto OpenID Connect standartu, lai implementētu vienoto pierakstīšanos, skatiet rakstā [OIDC vienotās pierakstīšanās izpratne](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-oidc-single-sign-on).
- Lai iegūtu informāciju gadījumā, ja izvēlēsities uzrakstīt savu kodu, tieši sūtot un apstrādājot HTTP pieprasījumus, vai izmantot trešās puses atvērtā pirmkoda bibliotēku, nevis izmantot kādu no mūsu atvērtajām bibliotēku bibliotēkām, skatiet rakstu [OAuth 2,0 un OpenID Connect protokolus Microsoft identitātes platformā](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-protocols).

**Protokolus**

1. [Microsoft identitātes platforma un netiešas dotācijas plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-implicit-grant-flow) — netiešās dotācijas definēšanas iezīme ir tāda, ka marķieri (ID marķieri vai piekļuves pilnvaras) tiek atgriezti tieši no/Authorize galapunkta, nevis/token galapunkta. To bieži izmanto kā daļu no autorizācijas koda plūsmas, kas tiek dēvēts par **"hibrīdo plūsmu" —/Authorize pieprasījumā izgūstot ID marķieri kopā ar autorizācijas kodu**. Šajā rakstā ir paskaidrots, kā programmu tieši salīdzināt ar protokolu jūsu lietojumprogrammā, lai pieprasītu pilnvaras no Azure AD.
2. [Microsoft Identity Platform un oauth 2,0 autorizācijas koda plūdums](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) — OAuth 2,0 autorizācijas koda dotācija var tikt izmantota lietojumprogrammās, kas ierīcē ir instalētas, lai piekļūtu aizsargātajiem resursiem, piemēram, tīmekļa API. Izmantojot Microsoft Identity Platform, ko implementē 2,0, varat **Pievienot pierakstīšanās un API piekļuvi savām mobilajām un datora lietojumprogrammām**. Šajā rakstā ir paskaidrots, kā programmu tieši lietot pie protokola savā lietojumprogrammā, izmantojot jebkuru valodu.
3. [Microsoft Identity Platform un OpenID Connect protokols](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) — ja izmantojat Microsoft identitātes platformas funkciju OpenID Connect, varat pievienot pierakstīšanās un API piekļuvi savām programmām. Šajā rakstā ir parādīts, kā to izdarīt neatkarīgi no valodas, un aprakstīts, kā **nosūtīt un saņemt http ziņojumus, neizmantojot nevienu Microsoft atvērtā koda bibliotēku**.
4. [Microsoft Identity Platform un OAuth 2,0 klienta akreditācijas datu plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) — varat izmantot OAuth 2,0 klienta akreditācijas datus, kas norādīti RFC 6749, dažkārt dēvē par **divu kāju OAuth**, lai piekļūtu tīmekļa viesotiem resursiem, izmantojot lietojumprogrammas identitāti. Šis dotācijas veids parasti tiek izmantots servera un servera mijiedarbībai, kas ir jādarbojas fonā, neveicot tūlītēju mijiedarbību ar lietotāju. Šie lietojumprogrammu tipi bieži tiek dēvēti par **dēmoniem** vai **pakalpojumu kontiem**. Šajā rakstā ir paskaidrots, kā programmu tieši programmēt savā lietojumprogrammā.
