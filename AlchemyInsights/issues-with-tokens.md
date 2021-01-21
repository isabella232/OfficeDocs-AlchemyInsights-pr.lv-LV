---
title: Problēmas ar marķieriem
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7774"
- "9004351"
ms.openlocfilehash: 14a9681c08920094813497e7a75eb87bb0733cbc
ms.sourcegitcommit: e378232f4c9ef4e962208100db752221e7bd2dd6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/20/2021
ms.locfileid: "49917041"
---
# <a name="issues-with-tokens"></a>Problēmas ar marķieriem

Lai pārvaldītu ar pilnvarām saistītas problēmas, varat veikt tālāk norādītās darbības.

1. Varat norādīt Microsoft identitātes platformā izsniegtu Access, ID vai SAML marķierierīces ilgumu. Varat iestatīt token mūžus visās programmās savā organizācijā, vairāku nomnieku (vairāku organizāciju) lietojumprogrammai vai konkrētam pakalpojumu pilnvarotājam jūsu organizācijā. Papildinformāciju skatiet rakstā [konfigurējamas marķierierīces ilgumus Microsoft identitātes platformā (priekšskatījums)](https://docs.microsoft.com/azure/active-directory/develop/active-directory-configurable-token-lifetimes).
2. Piekļuves pilnvaras nodrošina klientiem drošus zvanus uz aizsargāto tīmekļa API, un tās izmanto tīmekļa API, lai veiktu autentifikāciju un autorizāciju. Atbilstoši OAuth specifikācijai piekļuves marķieri ir necaurredzamas virknes, bet nav iestatīts formāts-daži identitātes pakalpojumu sniedzēji (IPP) izmanto GUID, citi lietotāji izmanto šifrētus BLOB. Microsoft identitātes platformā tiek izmantoti dažādi piekļuves pilnvaras formāti atkarībā no API konfigurācijas, kas akceptē marķieri. Lai uzzinātu, kā jūsu API var validēt un izmantot prasības piekļuves pilnvarā, skatiet rakstu [Microsoft identitātes platformas piekļuves marķieri](https://docs.microsoft.com/azure/active-directory/develop/userinfo#calling-the-userinfo-endpoint).
3. Microsoft autentifikācijas bibliotēka (MSAL) atbalsta vairākas autentifikācijas plūsmas, kas jāizmanto dažādos lietojumprogrammas scenārijos. Papildinformāciju skatiet rakstā [autentifikācijas plūsmas](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows#how-each-flow-emits-tokens-and-codes).
4. OAuth 2,0 autorizācijas koda dotāciju var izmantot lietojumprogrammās, kas ir instalētas ierīcē, lai piekļūtu aizsargātajiem resursiem, piemēram, tīmekļa API. Izmantojot Microsoft Identity Platform, ko implementē 2,0, varat pievienot pierakstīšanās un API piekļuvi savām mobilajām un datora programmām. Skatiet [Microsoft identitātes platformu un OAuth 2,0 autorizācijas koda plūsmu](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow#refresh-the-access-token) par to, kā programmā tieši lietot lietojumprogrammu, izmantojot jebkuru valodu.
5. OpenID Connect (OIDC) ir autentifikācijas protokols, kas izveidots, izmantojot OAuth 2,0, ko varat izmantot, lai lietotājam nodrošinātu drošu pierakstīšanos lietojumprogrammā. Ja izmantojat Microsoft identitātes platformas galapunkta īstenošanu OpenID Connect, varat pievienot pierakstīšanās un API piekļuvi savām programmām. [Microsoft Identity Platform un OpenID Connect protokols](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc#send-the-sign-in-request) parāda, kā to paveikt neatkarīgi no valodas, un aprakstīts, kā nosūtīt un saņemt http ziņojumus, neizmantojot nevienu Microsoft atvērtā koda bibliotēku.
    - UserInfo galapunkts ir daļa no OIDC standarta, kas paredzēts, lai atgrieztu prasības par autentificēto lietotāju. Papildinformāciju skatiet rakstā [Microsoft identitātes platformas UserInfo galapunkts](https://docs.microsoft.com/azure/active-directory/develop/userinfo#consider-use-an-id-token-instead).
    - [Zvana tīmekļa API tīmekļa lietojumprogrammā, izmantojot AZURE ad un OpenID Connect](https://docs.microsoft.com/samples/azure-samples/active-directory-dotnet-webapp-webapi-openidconnect/active-directory-dotnet-webapp-webapi-openidconnect/) paraugu, ir parādīts, kā izveidot MVC tīmekļa lietojumprogrammu, kas izmanto Azure AD, lai pierakstītos, izmantojot OpenID Connect protokolu, un pēc tam zvanīt uz tīmekļa API lietotāja identitāti, izmantojot pilnvaras, kas iegūtas ar OAuth 2,0. Šajā piemērā ir izmantota OpenID Connect ASP .NET OWIN starpprogrammatūra un ADAL .net.
6. [Lietojumprogrammas konfigurēšana, lai atklātu Web API](https://docs.microsoft.com/azure/active-directory/develop/quickstart-configure-app-expose-web-apis) -šajā Quickstart, reģistrējiet tīmekļa API ar Microsoft identitātes platformu un Atklājiet to klienta programmās, pievienojot piemēra tvērumu. Reģistrējot savu tīmekļa API un piedāvājot to, izmantojot tvērumus, varat nodrošināt piekļuves tiesības saviem resursiem autorizētiem lietotājiem un klienta programmām, kas piekļūst jūsu API.
7. Azure Active Directory B2C (Azure AD B2C) gadījumā resursu īpašnieka paroļu akreditācijas dati (ROPC) plūsma ir OAuth standarta autentifikācijas plūsma. Šajā plūsmā lietojumprogramma, kas tiek dēvēta arī par pakārtoto pusi, maina derīgus akreditācijas datus. Akreditācijas dati ietver lietotāja ID un paroli. Atgrieztās pilnvaras ir ID marķieris, piekļuves pilnvara un atsvaidzināšanas pilnvara. Lai iegūtu papildinformāciju, skatiet rakstu [resursu īpašnieka paroļu datu plūsmas izveide Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/add-ropc-policy?tabs=app-reg-ga&pivots=b2c-user-flow). 

