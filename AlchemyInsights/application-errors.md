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
ms.openlocfilehash: ce4c89da79112726ed4fb25527edc8d082bd37f239595b9eab7279abeeecfd7e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53931456"
---
# <a name="application-errors"></a>Lietojumprogrammas kļūdas

Vai meklējat informāciju par **AADSTS** kļūdu kodiem, kas tiek atgriezti no Azure Active Directory (Azure AD) drošības pilnvaru pakalpojuma (STS)? Izlasiet [Azure AD Authentication un authorization kļūdu](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) kodus, lai atrastu AADSTS kļūdu aprakstus, labojumus un dažus ieteiktos risinājumus.

Autorizācijas kļūdas var rasties vairāku dažādu problēmu rezultātā, no kurām lielākā daļa ģenerē kļūdu 401 vai 403. Piemēram, turpmāk minētās darbības var radīt autorizācijas kļūdas:

- Nepareizas [piekļuves pilnvaru iegūšanas plūsmas](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes) 
- Nepareizi konfigurēti [atļauju tvērumi](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes) 
- [Piekrišanas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) trūkums

Lai novērstu bieži sastopamas autorizācijas kļūdas, izmēģiniet tālāk norādītās darbības, kas visvairāk atbilst saņemtajām kļūdām. Var tikt piemēroti vairāki.

**Kļūda 401 — neautorizēts: vai jūsu pilnvara ir derīga?**

Pārliecinieties, vai jūsu lietojumprogramma prezentē derīgu piekļuves Graph Microsoft lietojumprogrammai kā daļu no pieprasījuma. Šī kļūda bieži nozīmē to, ka piekļuves pilnvarai, iespējams, trūkst HTTP autentifikācijas pieprasījuma galvenes vai arī pilnvara ir nederīga vai ir beidzies tās derīgums. Iesakām izmantot Microsoft Authentication [Library (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/msal-overview) piekļuves pilnvaru iegūšanai. Turklāt šī kļūda var rasties, ja mēģināt izmantot pilnvaroto piekļuves pilnvaru, kas piešķirts personiskajam Microsoft kontam, lai piekļūtu API, kas atbalsta tikai darba vai mācību kontus (organizācijas kontus).

**Kļūda 403 — aizliegts: vai esat izvēlējies pareizo atļauju kopu?**

Pārliecinieties, vai esat pieprasījis pareizo atļauju kopu, pamatojoties uz Microsoft Graph PROGRAMMAS zvanu API. Ieteicamās privileģētās atļaujas tiek nodrošinātas visās Microsoft Graph API atsauces metodes tēmās. Turklāt lietotājam vai administratoram ir jāpiešķir šīs atļaujas lietojumprogrammai. Atļauju piešķiršana parasti notiek ar piekrišanas lapu vai piešķirot atļaujas, izmantojot Azure Portal lietojumprogrammu reģistrācijas asmens stieņu. Lietojumprogrammas panelī **Iestatījumi** noklikšķiniet uz **Nepieciešamās atļaujas** un pēc tam noklikšķiniet uz **Piešķirt atļaujas**.

- [Microsoft Graph atļaujas](https://docs.microsoft.com/graph/permissions-reference) 
- [Informācija par Azure AD atļaujām un piekrišanu](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 

**Kļūda 403 — aizliegts: vai jūsu lietojumprogramma ieguva pilnvaru, kas atbilst izvēlētajām atļaujām?**

Pārliecinieties, vai pieprasītās vai piešķirtās atļaujas atbilst piekļuves marķiera tipam, ko programma iegūst. Iespējams, jūs pieprasāt un piešķirat lietojumprogrammas atļaujas, bet izmantojat deleģētus interaktīvu kodu plūsmas marķierus, nevis klienta akreditācijas datu plūsmas marķierus vai pieprasāt un piešķirat deleģētās atļaujas, bet izmanto klienta akreditācijas datu plūsmas marķierus, nevis pilnvaroto kodu plūsmas marķierus.

- [Piekļuves iegūšana lietotāju vārdā un deleģētu atļauju iegūšana](https://docs.microsoft.com/graph/auth_v2_user) 
- [Azure AD v2.0 — OAuth 2.0 autorizācijas kodu plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Piekļuves iegūšana bez lietotāja (dēmona pakalpojuma) un lietojumprogrammas atļaujām](https://docs.microsoft.com/graph/auth_v2_service) 
- [Azure AD v2.0 — OAuth 2.0 klienta akreditācijas datu plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow) 

**Kļūda 403 — aizliegts: paroles atiestatīšana**

Pašlaik nav pieejamas lietojumprogrammas dēmona atļaujas no pakalpojuma uz pakalpojumu, kas atļautu lietotāju paroļu atiestatīšanu. Šie API tiek atbalstīti tikai tad, ja tiek izmantotas interaktīvas deleģētu kodu plūsmas un administrators ir pierakstījies.

- [Microsoft Graph atļaujas](https://docs.microsoft.com/graph/permissions-reference)

**403 — aizliegts: vai lietotājam ir piekļuve un vai tas ir licencēts?**

Ja deleģētais kods plūst, Microsoft Graph novērtē, vai pieprasījums ir atļauts, pamatojoties uz lietojumprogrammai piešķirtām atļaujām un atļaujām, kas piešķirtas lietotājam, kurš ir pierakstījies. Parasti šī kļūda norāda, ka lietotājs nav pietiekami privileģēts, lai izpildītu pieprasījumu vai lietotājam nav licences piekļūstamajiem datiem. Pieprasījumu sekmīgi var veikt tikai lietotāji, kuriem ir nepieciešamās atļaujas vai licences.

**403 — aizliegts: vai atlasījāt pareizo resursa API?**

API pakalpojumi, piemēram, Microsoft Graph, pārbauda, vai skaņas pieprasne (auditorija) saņemtajā piekļuves marķierī atbilst vērtībai, kas tiek gaidīta sev, un, ja tā nav, rodas kļūda 403 Aizliegts. Bieži vien šī kļūda rodas tad, ja mēģina izmantot pilnvaru, kas iegūta Azure AD Graph API, Outlook API vai SharePoint/OneDrive API, lai izsauktu Microsoft Graph (vai otrādi). Pārliecinieties, vai resurss (vai tvērums), kuram jūsu lietojumprogramma iegūst pilnvaru, atbilst API, kuru lietojumprogramma izsauc.

**400 — nederīgs pieprasījums vai 403 — aizliegts: vai lietotājs atbilst savas organizācijas nosacītās piekļuves (CA) politikām?**

Pamatojoties uz organizācijas CA politikām, lietotājs, kas piekļūst Microsoft Graph resursiem, izmantojot jūsu programmu, var tikt pieprasīts iegūt papildinformāciju, kas nav pieejama piekļuves marķierī, ko sākotnēji ieguvāt jūsu lietojumprogrammā. Šādā gadījumā lietojumprogramma saņem kļūdu 400 ar *interaction_required* piekļuves pilnvaras iegūšanas laikā vai kļūdu 403 ar *insufficient_claims*, izsaucot Microsoft Graph. Abos gadījumos kļūdas atbilde satur papildu informāciju, ko var norādīt autorizētajā galapunktā, lai lietotājs varētu pieprasīt papildu informāciju (piemēram, daudzpakāpju autentifikāciju vai ierīces reģistrāciju).

- [Nosacījuma piekļuves izaicinājumu apstrāde, izmantojot MSAL ](https://docs.microsoft.com/azure/active-directory/develop/msal-handling-exceptions#conditional-access-and-claims-challenges)
- [Norādījumi izstrādātājiem par Azure Active Directory nosacīto piekļuvi](https://docs.microsoft.com/azure/active-directory/develop/conditional-access-dev-guide)
