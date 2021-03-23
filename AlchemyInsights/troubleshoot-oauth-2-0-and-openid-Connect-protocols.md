---
title: OAuth 2,0 un OpenID Connect protokolu problēmu novēršana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/17/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9776"
- "9004342"
ms.openlocfilehash: d2f14d4d16bea890b564cdb9bd9ac3875c28d115
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036404"
---
# <a name="troubleshoot-oauth-20-and-openid-connect-protocols"></a>OAuth 2,0 un OpenID Connect protokolu problēmu novēršana

Lai atrisinātu OAuth 2,0 un OpenID Connect problēmas, veiciet tālāk norādītās ieteicamās darbības.

Skatiet tālāk norādītos rakstus, kas saistīti ar konfigurēšanas un problēmu novēršanas OAuth 2,0 un OpenID Connect protokoliem:

- [Microsoft Identity Platform un OAuth 2,0 autorizācijas koda plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) — šajā rakstā ir paskaidrots, kā programmēt tieši programmā **Code Grant (PKCE)** , izmantojot jebkuru valodu.
- [Microsoft Identity Platform un OAuth 2,0 klienta akreditācijas datu plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) — šajā rakstā ir paskaidrots, kā programmu tieši salīdzināt ar **klienta akreditācijas datiem** jūsu lietojumprogrammā.
- [Microsoft Identity Platform un OAuth 2,0 resursu īpašnieka paroļu akreditācijas dati](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth-ropc) — šajā rakstā paskaidrots, kā programmēt tieši programmā **ROPC plūsmu** lietojumprogrammā.
    - Microsoft Identity Platform atbalsta tikai ROPC Azure AD nomniekiem, nevis personiskajiem kontiem. Tas nozīmē, ka ir jāizmanto nomnieka konkrēts galapunkts **( https://login.microsoftonline.com/{TenantId_or_Name})** vai **organizācijas** galapunkts.
    - Privātie konti, kas tiek uzaicināti uz Azure AD nomnieku, nevar izmantot ROPC.
    - Konti, kuriem nav paroļu, nevar pierakstīties, izmantojot ROPC. Šajā scenārijā ieteicams tā vietā izmantot citu programmas plūdumu.
    - Ja lietotājiem ir jāizmanto [daudzfaktoru autentifikācija (MFA)](https://docs.microsoft.com/azure/active-directory/authentication/concept-mfa-howitworks) , lai pieteiktos lietojumprogrammā, tie tiks bloķēti.
    - ROPC netiek atbalstīts [hibrīdo identitātes Federācijas](https://docs.microsoft.com/azure/active-directory/hybrid/whatis-fed) scenārijos (piemēram, Azure AD un ADFS, ko izmanto, lai autentificētu lokālos kontus). Ja lietotāji ir pāradresēti uz lokālo identitātes nodrošinātāju, Azure AD nevar pārbaudīt lietotājvārdu un paroli pret šo identitātes nodrošinātāju. [Tranzīta autentifikācija](https://docs.microsoft.com/azure/active-directory/hybrid/how-to-connect-pta) tiek atbalstīta ar ROPC, tomēr.
    - Izņēmums hibrīdās identitātes Federācijas scenārijā ir šāds: mājas valstības atklāšanas politika ar **AllowCloudPasswordValidation** , kas ir **patiess** , ļaus ROPC plūsmu darboties ar Federatīvajām lietotājiem, ja lokālā parole ir sinhronizēta ar mākoni. Papildinformāciju skatiet rakstā [integrētās lietojumprogrammas tiešo ROPC autentifikācija](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-authentication-for-federated-users-portal#enable-direct-ropc-authentication-of-federated-users-for-legacy-applications) 
- [Microsoft identitātes platforma un OAuth 2,0 uz](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-on-behalf-of-flow) priekšu — šajā rakstā ir paskaidrots, kā programmēt tieši programmā, kas atrodas uz jūsu lietojumprogrammas **(OBO) plūsmas** .
- [Microsoft Identity Platform un OpenID Connect protokols](https://docs.microsoft.com/azure/active-directory/develop/v2-protocols-oidc) — šajā rakstā ir parādīts, kā ieviest OpenID Connect protokolu neatkarīgi no valodas un aprakstīts, kā nosūtīt un saņemt http ziņojumus, neizmantojot nevienu Microsoft atvērtā koda bibliotēku.

**Piekļuves marķieri**

[Microsoft identitātes platformas piekļuves marķieri](https://docs.microsoft.com/azure/active-directory/develop/access-tokens) — Uzziniet, kā jūsu API var validēt un izmantot prasības piekļuves pilnvarā. Visa šī raksta dokumentācija, izņemot gadījumus, kad tas ir norādīts, attiecas tikai uz pilnvarām, kas emitētas par jūsu reģistrēto API. Tas neattiecas uz pilnvarām, kas ir izsniegtas korporācijai Microsoft piederošiem API, un šīs pilnvaras nevar izmantot, lai validētu, kā Microsoft identitātes platforma izdos marķierus jūsu izveidotajam API.

**Lietojumprogrammas konfigurācija**

[NOVIRZĪT URI (atbildes URL) ierobežojumus un ierobežojumus](https://docs.microsoft.com/azure/active-directory/develop/reply-url) — Uzziniet, kā konfigurēt savu novirzīšanas URI (atbildes URL). Novirzīšanas URI vai atbildes vietrādis URL ir atrašanās vieta, kur autorizācijas serveris nosūta lietotāju pēc tam, kad lietojumprogramma ir veiksmīgi autorizēta un piešķirta autorizācijas kods vai piekļuves pilnvara. Autorizācijas serveris nosūta kodu vai marķieri uz pāradresēšanas URI. tāpēc ir svarīgi reģistrēt pareizo atrašanās vietu lietojumprogrammas reģistrācijas procesa ietvaros.

**Lietojumprogrammas nodrošinājums**

[Apmācība: SCIM galapunkta nodrošināšanas un plānošanas plānošana](https://docs.microsoft.com/azure/active-directory/app-provisioning/use-scim-to-provision-users-and-groups) — šajā rakstā ir paskaidrots, kā izveidot SCIM galapunktu un to integrēt ar AAD nodrošināšanas pakalpojumu.


