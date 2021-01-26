---
title: Lietojumprogrammas kļūdas
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
- "9004342"
- "7841"
ms.openlocfilehash: 2ef90b54ce222a06740e05891fabe87b6565cb14
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49984586"
---
# <a name="application-errors"></a>Lietojumprogrammas kļūdas

Vai meklējat informāciju par **AADSTS kļūdu kodiem** , kas tiek atgriezti Azure Active Directory (Azure AD) drošības marķierierīces pakalpojumā (STS)? Izlasiet [AZURE ad autentifikāciju un autorizācijas kļūdu kodus](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , lai atrastu AADSTS kļūdu aprakstus, labojumus un dažus ieteicamos risinājumus.

Autorizācijas kļūdas var būt vairāku atšķirīgu problēmu rezultāts, no kurām lielākā daļa ģenerē 401 vai 403 kļūdu. Piemēram, tālāk norādītās darbības var izraisīt autorizācijas kļūdas.

- Nepareiza [piekļuves marķiera iegūšanas plūsma](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Vāji konfigurēti [atļauju tvērumi](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [Piekrišanas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) trūkums

Lai atrisinātu biežāk sastopamās autorizācijas kļūdas, izmēģiniet tālāk norādītās darbības, kas visvairāk atbilst saņemtajai kļūdai. Var lietot vairāk nekā vienu.

**401 nesankcionēta kļūda: vai jūsu pilnvara ir derīga?**

Pārliecinieties, vai lietojumprogrammā ir redzama derīga piekļuves pilnvara programmai Microsoft Graph kā pieprasījuma daļa. Šī kļūda bieži nozīmē to, ka piekļuves pilnvara, iespējams, trūkst HTTP autentificēšanas pieprasījuma galvenē vai šī pilnvara nav derīga vai tai ir beidzies derīguma termiņš. Stingri ieteicams izmantot [Microsoft autentifikācijas bibliotēku (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) , lai saņemtu piekļuves tiesības. Turklāt šī kļūda var rasties, ja mēģināt izmantot pilnvarotu piekļuves pilnvaru, kas piešķirta personiskam Microsoft kontam, lai piekļūtu API, kas atbalsta tikai darba vai mācību iestādes kontus (organizācijas konti).

**403 Forbidden kļūda: vai esat izvēlējies pareizo atļauju kopu?**

Pārliecinieties, vai esat pieprasījis pareizo atļauju kopu, kuras pamatā ir Microsoft Graph API jūsu programmu zvani. Ieteicamās vismazāk priviliģētās atļaujas ir sniegtas visās Microsoft Graph API atsauču metodes tēmās. Turklāt šīs atļaujas lietojumprogrammai ir jāpiešķir lietotājam vai administratoram. Atļauju piešķiršana parasti notiek, izmantojot piekrišanas lapu vai piešķirot atļaujas, izmantojot Azure portāla lietojumprogrammas reģistrācijas disku. Lietojumprogrammā **Iestatījumi** noklikšķiniet uz **nepieciešamās atļaujas** un pēc tam noklikšķiniet uz **piešķirt atļaujas**.

- [Microsoft Graph atļaujas](https://docs.microsoft.com/graph/permissions-reference) 
- [Izpratne par Azure AD atļaujām un piekrišana](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**403 Forbidden kļūda: vai jūsu lietojumprogramma ir padarījusi atgādinājumu atbilstoši izvēlētām atļaujām?**

Pārliecinieties, vai pieprasīšanas vai piešķirto atļauju tips atbilst lietojumprogrammas piekļuves pilnvarām veidam. Iespējams, jums būs jāpieprasa un jāpiešķir lietojumprogrammas atļaujas, bet, izmantojot pilnvarotas interaktīvas koda plūsmas marķierus, nevis klienta akreditācijas datu plūsmas marķierus vai pieprasot un piešķirot pilnvarotās atļaujas, bet izmantojot klienta akreditācijas datu plūsmas marķierus.

- [Piekļuves iegūšana lietotāju vārdā un pilnvarotās atļaujas](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v 2.0-OAuth 2,0 autorizācijas koda plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Piekļuves iegūšana, neizmantojot lietotāju (dēmona pakalpojumu) un lietojumprogrammas atļaujas](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v 2.0-OAuth 2,0 klienta akreditācijas datu plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**403 Forbidden kļūda: paroles atiestatīšana**

Pašlaik nav nevienas lietojumprogrammas atļauju dēmona pakalpojumu atļaujas, kas ļauj atiestatīt lietotāju paroles. Šie API tiek atbalstīti tikai, izmantojot interaktīvo pilnvaroto kodu plūsmu ar pierakstījies administratoru.

- [Microsoft Graph atļaujas](https://docs.microsoft.com/graph/permissions-reference)

**403 aizliegts: vai lietotājam ir piekļuve un vai tie ir licencēti?**

Attiecībā uz pilnvarotajām kodu plūsmām Microsoft Graph novērtē, vai pieprasījums ir atļauts, pamatojoties uz lietojumprogrammai piešķirtajām atļaujām un atļaujām, kas ir pierakstījies lietotājam. Parasti šī kļūda norāda, ka lietotājs nav pietiekami privileģēts, lai izpildītu pieprasījumu, vai arī lietotājam nav atļauts piekļūt datiem. Pieprasījumu var veiksmīgi veikt tikai lietotāji ar nepieciešamajām atļaujām vai licencēm.

**403 Forbidden: vai atlasījāt pareizo resursu API?**

API pakalpojumus, piemēram, Microsoft Graph, pārbaudiet, vai AUD prasība (auditorija) saņemtajā piekļuves pilnvarā atbilst vērtībai, ko tas sagaida, un, ja tā nav, tā izraisa 403 Forbidden kļūdu. Izplatīta kļūda, kuras rezultātā rodas šī kļūda, mēģina izmantot Azure AD Graph API, Outlook API vai SharePoint/OneDrive API, lai sasauktu Microsoft Graph (vai otrādi). Pārliecinieties, vai jūsu lietojumprogramma resurss (jeb tvērums) atbilst API, uz kuru tiek zvanīts.

**400 nederīgs pieprasījums vai 403 Forbidden: vai lietotājs atbilst savas organizācijas nosacījuma piekļuves (CA) politikām?**

Pamatojoties uz organizācijas CA politikām, lietotājam, kas piekļūst Microsoft Graph resursiem, izmantojot lietojumprogrammu, var tikt apstrīdēta papildu informācija, kas nav pieejama jūsu lietojumprogrammā, kas sākotnēji tika iegūta. Šajā gadījumā jūsu lietojumprogramma saņem 400, izmantojot *interaction_required* kļūdu, pie403 kļūstot Microsoft Graph, izmantojot *insufficient_claims* kļūdu. Abos gadījumos kļūdas atbilde ir papildinformācija, kas var tikt parādīta atļaut galapunktā, lai lietotājam apstrīdētu papildu informāciju (piemēram, vairāku faktoru autentifikācija vai ierīces reģistrācija).

- [Ierobežotas piekļuves problēmu novēršana, izmantojot MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Izstrādātāja norādījumi Azure Active Directory nosacījuma piekļuvei](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
