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
ms.openlocfilehash: 2f413e863e6aa23548e425de5901f8158e1d48ab
ms.sourcegitcommit: ba3118b7ad5e02756d0e5c2113245090f54370af
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49976856"
---
# <a name="authentication-issues"></a>Autentifikācijas problēmas

**Vai meklējat informāciju par AADSTS kļūdu kodiem, kas tiek atgriezti no Azure Active Directory (Azure AD) drošības pilnvaru pakalpojuma (STS)?** Skatiet rakstu [Azure AD autentifikācijas un autorizācijas kļūdu kodi](https://docs.microsoft.com/azure/active-directory/develop/reference-aadsts-error-codes), lai atrastu AADSTS kļūdu aprakstus, labojumus un dažus ieteiktos risinājumus.

Autorizācijas kļūdas var rasties vairāku dažādu problēmu rezultātā, no kurām lielākā daļa ģenerē kļūdu 401 vai 403. Piemēram, tālāk minētās problēmas var izraisīt autorizācijas kļūdas.

- Nepareizas [piekļuves pilnvaru iegūšanas plūsmas](https://docs.microsoft.com/azure/active-directory/develop/authentication-vs-authorization) 
- Nepareizi konfigurēti [atļauju tvērumi](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) 
- [Piekrišanas](https://docs.microsoft.com/azure/active-directory/develop/howto-convert-app-to-be-multi-tenant#understanding-user-and-admin-consent) trūkums

Lai novērstu biežāk sastopamās autorizācijas kļūdas, izmēģiniet tālāk norādītās darbības, kas vislabāk atbilst saņemtajai kļūdai. Saņemtajai kļūdai var tikt lietota vairāk nekā viena darbība.

**Kļūda 401 — neautorizēts: vai jūsu pilnvara ir derīga?**

Pārliecinieties, vai jūsu lietojumprogrammai pieprasījuma ietvaros ir derīga piekļuves pilnvara risinājumam Microsoft Graph. Šī kļūda bieži nozīmē to, ka piekļuves pilnvarai, iespējams, trūkst HTTP autentifikācijas pieprasījuma galvenes vai arī pilnvara ir nederīga vai ir beidzies tās derīgums. Stingri iesakām izmantot Microsoft autentifikācijas bibliotēku (MSAL) piekļuves pilnvaru iegūšanai. Turklāt šī kļūda var rasties, ja mēģināt izmantot deleģētu piekļuves pilnvaru, kura piešķirta personiskajam Microsoft kontam, lai piekļūtu API, kas atbalsta tikai darba vai mācību kontus (organizācijas kontus).

**Kļūda 403 — aizliegts: vai esat izvēlējies pareizo atļauju kopu?**

Pārliecinieties, vai esat pieprasījis pareizo atļauju kopu, ņemot vērā Microsoft Graph API, kuru izsauc jūsu lietojumprogramma. Ieteicamās mazāk privileģētās atļaujas tiek nodrošinātas visās Microsoft Graph API atsauču metožu tēmās. Turklāt lietotājam vai administratoram ir jāpiešķir šīs atļaujas lietojumprogrammai. Atļauju piešķiršana parasti notiek, izmantojot piekrišanas lapu vai lietojot Azure portāla lietojumprogrammas reģistrācijas paneli. Lietojumprogrammas panelī **Iestatījumi** noklikšķiniet uz **Nepieciešamās atļaujas** un pēc tam noklikšķiniet uz **Piešķirt atļaujas**. Papildinformāciju skatiet šeit:

- [Microsoft Graph atļaujas](https://docs.microsoft.com/graph/permissions-reference) 
- [Informācija par Azure AD atļaujām un piekrišanu](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent)

**Kļūda 403 — aizliegts: vai jūsu lietojumprogramma ieguva pilnvaru, kas atbilst izvēlētajām atļaujām?**

Pārliecinieties, vai pieprasīto vai piešķirto atļauju tipi atbilst piekļuves pilnvaras tipam, ko iegūst jūsu lietojumprogramma. Iespējams, jūs pieprasāt un piešķirat lietojumprogrammas atļaujas, taču tas notiek, izmantojat deleģētu interaktīvu kodu plūsmas pilnvaras, nevis klienta akreditācijas datu plūsmas pilnvaras, vai arī jūs pieprasāt un piešķirat deleģētas atļaujas, taču tas notiek, izmantojat klienta akreditācijas datu plūsmas pilnvaras, nevis deleģētu kodu plūsmas pilnvaras.

Papildinformāciju par pilnvaru iegūšanu skatiet šeit:

- [Piekļuves iegūšana lietotāju vārdā un deleģētu atļauju iegūšana](https://docs.microsoft.com/graph/auth-v2-user) 
- [Azure AD v2.0 — OAuth 2.0 autorizācijas kodu plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-auth-code-flow) 
- [Piekļuves iegūšana bez lietotāja (dēmona pakalpojuma) un lietojumprogrammas atļaujām](https://docs.microsoft.com/graph/auth-v2-service) 
- [Azure AD v2.0 — OAuth 2.0 klienta akreditācijas datu plūsma](https://docs.microsoft.com/azure/active-directory/develop/v2-oauth2-client-creds-grant-flow)

**Kļūda 403 — aizliegts: paroles atiestatīšana**

Pašlaik nav pieejamas lietojumprogrammas dēmona atļaujas no pakalpojuma uz pakalpojumu, kas atļautu lietotāju paroļu atiestatīšanu. Šie API tiek atbalstīti tikai tad, ja tiek izmantotas interaktīvas deleģētu kodu plūsmas un administrators ir pierakstījies. Papildinformāciju skatiet rakstā [Microsoft Graph atļaujas](https://docs.microsoft.com/graph/permissions-reference).

**403 — aizliegts: vai lietotājam ir piekļuve un vai tas ir licencēts?**

Attiecībā uz deleģētu kodu plūsmām Microsoft Graph novērtē, vai pieprasījums ir atļauts, pamatojoties uz lietojumprogrammai piešķirtajām atļaujām, kā arī pierakstītā lietotāja atļaujām. Parasti šī kļūda norāda, ka lietotājs nav pietiekami privileģēts, lai izpildītu pieprasījumu **vai** lietotājam nav licences piekļūstamajiem datiem. Pieprasījumu sekmīgi var veikt tikai lietotāji, kuriem ir nepieciešamās atļaujas vai licences.

**403 — aizliegts: vai atlasījāt pareizo resursa API?**

API pakalpojumi, piemēram, Microsoft Graph, pārbauda, vai *auditorijas* prasība saņemtajā piekļuves pilnvarā atbilst paredzētajai vērtībai. Ja tā nav, rodas kļūda 403 — aizliegts. Bieži vien šī kļūda rodas tad, ja mēģina izmantot pilnvaru, kas iegūta Azure AD Graph API, Outlook API vai SharePoint/OneDrive API, lai izsauktu Microsoft Graph (vai otrādi). Pārliecinieties, vai resurss (vai tvērums), kuram jūsu lietojumprogramma iegūst pilnvaru, atbilst API, kuru lietojumprogramma izsauc.

**400 — nederīgs pieprasījums vai 403 — aizliegts: vai lietotājs atbilst savas organizācijas nosacītās piekļuves (CA) politikām?**

Pamatojoties uz organizācijas nosacītās piekļuves (CA) politikām, lietotājam, kurš piekļūst Microsoft Graph resursiem, izmantojot jūsu lietojumprogrammu, var tikt pieprasīta papildinformācija, kuras nav jūsu lietojumprogrammas sākotnēji iegūtajā piekļuves pilnvarā. Šādā gadījumā lietojumprogramma saņem kļūdu **400 ar *interaction_required*** piekļuves pilnvaras iegūšanas laikā vai kļūdu **403 ar *insufficient_claims***, izsaucot Microsoft Graph. Abos gadījumos kļūdas atbilde satur papildinformāciju, ko var iesniegt pilnvarotajam galapunktam, lai lietotājam pieprasītu papildinformāciju (piemēram, daudzfaktoru autentifikācija vai ierīces reģistrācija).

Papildinformāciju par nosacīto piekļuvi skatiet šeit:

- [Nosacītās piekļuves izaicinājumu risināšana, izmantojot MSAL](https://docs.microsoft.com/azure/active-directory/develop/msal-error-handling-dotnet#conditional-access-and-claims-challenges) 
- [Norādījumi izstrādātājiem par Azure Active Directory nosacīto piekļuvi](https://docs.microsoft.com/azure/active-directory/develop/v2-conditional-access-dev-guide)

**_Azure Active Directory autentifikācijas bibliotēkas (ADAL) un Azure AD Graph API (AAD Graph) atbalsta beigas_* _

- Sākot ar 2020. gada 30. jūniju, mēs vairs nepievienosim jaunus līdzekļus Azure Active Directory autentifikācijas bibliotēkai (ADAL) un Azure AD Graph API (AAD Graph). Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, bet vairs nenodrošināsim līdzekļu atjauninājumus.
- Sākot ar 2022. gada 30. jūniju, mēs vairs nesniegsim ADAL un AAD Graph atbalstu un vairs nenodrošināsim tehnisko atbalstu vai drošības atjauninājumus.
    - Lietojumprogrammas, kas izmanto ADAL esošajās OS versijās, turpinās darboties pēc šī datuma, taču nesaņems tehnisko atbalstu vai drošības atjauninājumus.
    - Lietojumprogrammas, kas izmanto AAD Graph, pēc šī datuma, iespējams, vairs nesaņems atbildes no AAD Graph galapunkta.

_ *ADAL migrācija**

Iesakām veikt atjaunināšanu uz [Microsoft autentifikācijas bibliotēku (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurā ir jaunākie līdzekļi un drošības atjauninājumi. Šis ieteikums tiek sniegts saistībā ar Microsoft lietojumprogrammu migrēšanu uz MSAL līdz atbalsta termiņa beigām. Microsoft lietojumprogrammu migrēšanas uz MSAL mērķis ir nodrošināt, ka lietojumprogrammas gūst priekšrocības no MSAL pastāvīgajiem drošības un līdzekļu uzlabojumiem.

- [Lasīt bieži uzdotos jautājumus par ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- [Uzziniet, kā migrēt lietojumprogrammas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
- Ja jums ir nepieciešama palīdzība, lai saprastu, kuras jūsu lietojumprogrammas izmanto ADAL, iesakām pārskatīt visu jūsu lietojumprogrammu pirmkodu un, ja nepieciešams, sazināties ar jebkuru neatkarīgu programmatūras izstrādātāju (ISV) vai lietojumprogrammu nodrošinātāju. Microsoft atbalsta dienests var jums sniegt sarakstu ar visām jūsu nomniekā esošajām lietojumprogrammām, kas nav Microsoft ADAL lietojumprogrammas.

**AAD Graph migrācija**

Saistībā ar lietojumprogrammām, kas izmanto AAD Graph, izpildiet norādījumus, lai [migrētu Azure AD Graph lietojumprogrammas uz Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist?view=graph-rest-1.0&preserve-view=true).

- [Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
- Azure lietojumprogrammu reģistrācijas portālā tiek rādīts, kuras lietojumprogrammas izmanto AAD Graph. Iesakām pārskatīt visu jūsu lietojumprogrammu pirmkodu un, ja nepieciešams, sazināties ar jebkuru ISV vai lietojumprogrammu nodrošinātāju. Microsoft atbalsta dienests var jums sniegt informāciju par visu AAD Graph lietojumu jūsu nomniekā.

 










