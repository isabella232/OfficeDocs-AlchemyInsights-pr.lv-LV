---
title: Autentifikācijas problēmas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7748"
- "9004339"
ms.openlocfilehash: 53bd0d8f8edaead519d0282239d3a6d338b297b9
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974485"
---
# <a name="authentication-issues"></a>Autentifikācijas problēmas

**Vai meklējat informāciju par AADSTS kļūdu kodiem, kas tiek atgriezti Azure Active Directory (Azure AD) drošības marķierierīces pakalpojumā (STS)?** Skatiet [AZURE ad autentifikāciju un autorizācijas kļūdu kodus](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) , lai atrastu AADSTS kļūdu aprakstus, labojumus un dažus ieteicamos risinājumus.

Autorizācijas kļūdas var būt vairāku atšķirīgu problēmu rezultāts, no kurām lielākā daļa ģenerē 401 vai 403 kļūdu. Piemēram, var rasties šādas problēmas:

- Nepareiza [piekļuves marķiera iegūšanas plūsma](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Vāji konfigurēti [atļauju tvērumi](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [Piekrišanas](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) trūkums

Lai atrisinātu biežāk sastopamās autorizācijas kļūdas, izmēģiniet tālāk norādītās darbības, kas visvairāk atbilst saņemtajai kļūdai. Saņemot kļūdas ziņojumu, var tikt piemērota vairāk nekā viena darbība.

- **401 nesankcionēta kļūda: vai jūsu pilnvara ir derīga?**

Pārliecinieties, vai jūsu programmai ir derīga piekļuves pilnvara programmai Microsoft Graph kā pieprasījuma daļa. Šī kļūda bieži nozīmē to, ka piekļuves pilnvara, iespējams, trūkst HTTP autentificēšanas pieprasījuma galvenē vai šī pilnvara nav derīga vai tai ir beidzies derīguma termiņš. Stingri ieteicams izmantot Microsoft autentifikācijas bibliotēku (MSAL), lai saņemtu piekļuves tiesības. Turklāt šī kļūda var rasties, ja mēģināt izmantot pilnvarotu piekļuves pilnvaru, kas piešķirta personiskam Microsoft kontam, lai piekļūtu API, kas atbalsta tikai darba vai mācību iestādes kontus (organizācijas konti).

**403 Forbidden kļūda: vai esat izvēlējies pareizo atļauju kopu?**

Pārliecinieties, vai esat pieprasījis pareizo atļauju kopu, kuras pamatā ir Microsoft Graph API jūsu programmu zvani. Ieteicamās vismazāk priviliģētās atļaujas ir sniegtas visās Microsoft Graph API atsauču metodes tēmās. Turklāt šīs atļaujas lietojumprogrammai ir jāpiešķir lietotājam vai administratoram. Atļauju piešķiršana parasti notiek, izmantojot piekrišanas lapu vai Azure portāla lietojumprogrammas reģistrācijas diska lietošanu. Lietojumprogrammā **Iestatījumi** noklikšķiniet uz **nepieciešamās atļaujas** un pēc tam noklikšķiniet uz **piešķirt atļaujas**. Papildinformāciju skatiet rakstā:

- [Microsoft Graph atļaujas](https://docs.microsoft.com/graph/permissions-reference) 
- [Izpratne par Azure AD atļaujām un piekrišana](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**403 Forbidden kļūda: vai jūsu lietojumprogramma ir padarījusi atgādinājumu atbilstoši izvēlētām atļaujām?**

Pārliecinieties, vai piešķiramo vai piešķirto atļauju tipi atbilstu lietojumprogrammas piekļuves veidam. Iespējams, jums būs jāpieprasa un jāpiešķir lietojumprogrammas atļaujas, bet, izmantojot pilnvarotas interaktīvas koda plūsmas marķierus, nevis klienta akreditācijas datu plūsmas marķierus, vai pieprasot un piešķirot pilnvarotās atļaujas, bet izmantojot klienta akreditācijas datu plūsmas marķierus, nevis deleģētās kodu plūsmas marķierus.

Papildinformāciju saistībā ar marķieru iegādi skatiet rakstā:

- [Piekļuves iegūšana lietotāju vārdā un pilnvarotās atļaujas](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v 2.0-OAuth 2,0 autorizācijas koda plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Piekļuves iegūšana, neizmantojot lietotāju (dēmona pakalpojumu) un lietojumprogrammas atļaujas](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v 2.0-OAuth 2,0 klienta akreditācijas datu plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**403 Forbidden kļūda: paroles atiestatīšana**

Pašlaik nav nevienas lietojumprogrammas atļauju dēmona pakalpojumu atļaujas, kas ļauj atiestatīt lietotāju paroles. Šie API tiek atbalstīti tikai, izmantojot interaktīvo pilnvaroto kodu plūsmu ar pierakstījies administratoru. Lai iegūtu papildinformāciju, skatiet rakstu [Microsoft Graph atļaujas](https://docs.microsoft.com/graph/permissions-reference).

**403 aizliegts: vai lietotājam ir piekļuve un vai tie ir licencēti?**

Attiecībā uz pilnvarotajām kodu plūsmām Microsoft Graph novērtē, vai pieprasījums ir atļauts, pamatojoties uz lietojumprogrammai piešķirtajām atļaujām un atļaujām, kas ir pierakstījies lietotājam. Parasti šī kļūda norāda, ka lietotājs nav pietiekami privileģēts, lai izpildītu pieprasījumu, **vai** arī lietotājam nav atļauts piekļūt datiem. Pieprasījumu var veiksmīgi veikt tikai lietotāji ar nepieciešamajām atļaujām vai licencēm.

**403 Forbidden: vai atlasījāt pareizo resursu API?**

API pakalpojumi tāpat kā Microsoft Graph pārbaudiet, vai *AUD* prasība (auditorija) saņemtajā piekļuves pilnvarā atbilst vērtībai, kas tiek gaidīta, un, ja tā nav, rodas 403 Forbidden kļūda. Izplatīta kļūda, kuras rezultātā rodas šī kļūda, mēģina izmantot Azure AD Graph API, Outlook API vai SharePoint/OneDrive API, lai sasauktu Microsoft Graph (vai otrādi). Pārliecinieties, vai jūsu lietojumprogramma resurss (jeb tvērums) atbilst API, uz kuru tiek zvanīts.

**400 nederīgs pieprasījums vai 403 Forbidden: vai lietotājs atbilst savas organizācijas nosacījuma piekļuves (CA) politikām?**

Pamatojoties uz organizācijas nosacījuma piekļuves (CA) politikām, lietotājam, kas piekļūst Microsoft Graph resursiem, izmantojot lietojumprogrammu, var tikt apstrīdēta papildu informācija, kas nav pieejama jūsu lietojumprogrammā, kas sākotnēji tika iegūta. Šajā gadījumā jūsu lietojumprogramma saņem **400, izmantojot *interaction_required*** kļūdu, Pie403 kļūstot Microsoft Graph, **izmantojot *insufficient_claims*** kļūdu. Abos gadījumos kļūdas atbilde ir papildinformācija, kas tiek rādīta pilnvarotajā galapunktā, lai lietotājam apstrīdētu papildu informāciju (piemēram, vairāku faktoru autentifikācija vai ierīces reģistrācija).

Papildinformāciju par ierobežotu piekļuvi skatiet rakstā:

- [Ierobežotas piekļuves problēmu novēršana, izmantojot MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Izstrādātāja norādījumi Azure Active Directory nosacījuma piekļuvei](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Azure Active Directory autentifikācijas bibliotēkas (ADAL) un AZURE ad GRAPH API (AAD Graph) atbalsta beigas_*

- Sākot no 30. jūnija, 2020 vairs nepievienosit jaunus līdzekļus Azure Active Directory autentifikācijas bibliotēkai (ADAL) un Azure AD Graph API (AAD Graph). Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, taču vairs nenodrošinās līdzekļu atjauninājumus.
- Sākot no 30. jūnija, 2022, mēs nodrošināsim atbalstu ADAL un AAD Graph un vairs nenodrošinās tehnisko atbalstu vai drošības atjauninājumus.
    - Programmas, kas, izmantojot ADAL, pēc šī laika turpinās darboties, bet nesaņem nekādu tehnisku atbalstu vai drošības atjauninājumus.
    - Pēc šī laika lietojumprogrammas, kas izmanto AAD Graph, var vairs nesaņemt atbildes no AAD Graph galapunkta.

*PārADAL migrācija**

Ieteicams atjaunināt [Microsoft autentifikācijas bibliotēkā (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurā ir jaunākie līdzekļi un drošības atjauninājumi. Šis ieteikums ir saistībā ar Microsoft, kas migrē tās lietojumprogrammas uz MSAL līdz atbalsta termiņa beigām. Microsoft apps migrēšanas uz MSAL mērķis ir nodrošināt, lai lietojumprogrammas izmantotu MSAL drošības un līdzekļu uzlabojumus.

- [ADAL bieži uzdoto jautājumu lasīšana](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Uzziniet, kā migrēt programmas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Ja jums ir nepieciešama palīdzība saistībā ar to, kuras programmas izmanto ADAL, iesakām pārskatīt visu savu programmu avota kodu un, ja nepieciešams, sazināties ar visiem neatkarīgajiem programmatūras piegādātājiem (ISV) vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsts var arī nodrošināt, ka jūsu nomniekā ir saraksts ar visām programmām, kas nav Microsoft ADAL.

**AAD Graph migrācija**

Lietojumprogrammas, kas izmanto AAD Graph, sekojiet mūsu norādījumiem, lai [migrētu AZURE ad Graph programmas uz Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanas punktu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Jūsu Azure lietojumprogrammu reģistrācijas portālā ir parādīts, kuras lietojumprogrammas izmanto AAD Graph. Iesakām pārskatīt visu savu lietojumprogrammu avota kodu un, ja nepieciešams, sazināties ar citiem ISV vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsts var arī sniegt informāciju par visu AAD Graph lietojumu jūsu nomniekā.

 










