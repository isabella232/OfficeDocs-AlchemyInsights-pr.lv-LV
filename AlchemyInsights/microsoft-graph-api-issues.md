---
title: Microsoft Graph API problēmas
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
- "9004345"
- "7759"
ms.openlocfilehash: 9df021211c8a65997889d9303dbf28a27104cfa95841d4cb810427c652ba0784
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53975900"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API problēmas

Šī tēma var arī attiecas uz izstrādātājiem, kuri joprojām izmanto Azure AD Graph API. Tomēr ir stingri **ieteicams izmantot** Microsoft Graph visos direktorija, identitātes un piekļuves pārvaldības scenārijos.

**Autentifikācijas vai autorizācijas problēmas**

- Ja jūsu  lietojumprogramma nevar iegūt marķierus, lai zvanītu korporācijai Microsoft Graph, izvēlieties Problēma ar piekļuves pilnvaras **(autentifikācijas)** saņemšana Microsoft Graph kategoriju, lai saņemtu specifiskāku palīdzību un atbalstu šajā tēmā.
- Ja lietojumprogramma saņem **401 vai 403** autorizācijas kļūdas, zvanot Microsoft Graph, izvēlieties kategorijas Iegūt liegtu piekļuvi **kļūda (Autorizācija)** Microsoft Graph API, lai saņemtu specifiskāku palīdzību un atbalstu par šo tēmu.

**Es vēlos izmantot Microsoft Graph, taču nezinu, kur sākt**

- [Pārskats par Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pārskats par identitātes un piekļuves pārvaldību programmā Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Darba sākšana, veidojot Microsoft Graph programmas](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** — microsoft Graph API jūsu nomniekā vai demonstrācijas nomniekā

**Es vēlos izmantot Microsoft Graph, bet vai tā atbalsta v1.0 direktorija API, kas nepieciešami?**

Microsoft Graph ir ieteicamais API direktorija, identitātes un piekļuves pārvaldībai. Tomēr starp Azure AD Graph un Microsoft Graph iespējamas atstarpes. Pārskatiet tālāk norādītos rakstus, kuros iezīmētas vistehnīgākās atšķirības, kas varētu palīdzēt izdarīt jūsu izvēli.

- [Azure AD Graph un Microsoft Graph resursu tipu atšķirības](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rekvizītu atšķirības starp Azure AD Graph un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API, uz kuru zvanu, nedarbojas — kur var veikt papildu testēšanu?**

**Microsoft Graph Explorer** — pārbaudiet Microsoft Graph API jūsu nomniekā vai demonstrācijas nomniekā, kā arī skatiet vaicājumu **paraugus** programmā Microsoft Graph Explorer.

**Mana programma ir pārāk lēna un arī tiek ierobežošana. Kādus uzlabojumus var veikt?**

Atkarībā no jūsu scenārija ir pieejamas dažādas opcijas, lai padarītu lietojumprogrammu vairāk izpildāmu, un dažos gadījumos mazāk noslodzētas pakalpojuma darbības laikā (ja veicat pārāk daudz zvanu).

- [Microsoft Graph paraugprakse](https://docs.microsoft.com/graph/best-practices-concept)
- [Pakešveida pieprasījumi](https://docs.microsoft.com/graph/json-batching)
- [Izmaiņu reģistrēšana, izmantojot delta vaicājumu](https://docs.microsoft.com/graph/delta-query-overview)
- [Paziņojumu par izmaiņām veikšana tīmeklī](https://docs.microsoft.com/graph/webhooks)
- [Ierobežošanas norādījumi](https://docs.microsoft.com/graph/throttling)

**Kur var atrast papildinformāciju par kļūdām un zināmajām problēmām?**

- [Microsoft Graph informācija par kļūdu atbildēm](https://docs.microsoft.com/graph/errors)
- [Zināmās problēmas ar Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Kur var pārbaudīt pakalpojumu pieejamības un savienojamības statusu?**

To pamatā esošo pakalpojumu pieejamība un savienojamība, kuriem var piekļūt, izmantojot Microsoft Graph, var ietekmēt Microsoft Graph kopējo pieejamību un veiktspēju.

- Lai Azure Active Directory pakalpojuma darbspēju, pārbaudiet **Azure** statusa lapā norādīto drošības un [identitātes pakalpojumu statusu.](https://azure.microsoft.com/status/)
- Lai Office pakalpojumus, kas veicina Microsoft Graph, pārbaudiet to pakalpojumu statusu, kas uzskaitīti [Office pakalpojuma darbspējas informācijas panelī.](https://portal.office.com/adminportal/home#/servicehealth)

Microsoft Graph autorizācijas kļūdas var izraisīt vairākas dažādas problēmas, un lielākā daļa ģenerē kļūdu 401 vai 403. Piemēram, turpmāk minētās darbības var radīt autorizācijas kļūdas:

- Nepareizas [piekļuves pilnvaru iegūšanas plūsmas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Nepareizi konfigurēti [atļauju tvērumi](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [Piekrišanas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) trūkums

***Atbalsta beigas autentifikācijas Azure Active Directory bibliotēkai (ADAL) un Azure AD Graph API (AAD Graph)***

**Sākot ar 2020. gada 30.** jūnijs, mēs vairs ne pievienosim jaunus līdzekļus ADAL un Azure AD Graph. Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, bet vairs nenodrošināsim līdzekļu atjauninājumus.

**Sākot ar 2022. gada 30.** jūnijs, mēs nobeigsim atbalstu ADAL un Azure AD Graph un vairs nenodrošināsim tehniskā atbalsta vai drošības atjauninājumus.

Programmas, kas izmanto ADAL esošajās OS versijās, pēc šī laika turpinās darboties, bet netiks *saņemts tehniskais atbalsts vai drošības atjauninājumi.*

Programmas, kas pēc Graph izmanto Azure AD Graph, iespējams, vairs nesaņems atbildes no Azure AD Graph galapunkta.

**ADAL migrācija**

Iesakām veikt atjaunināšanu uz [Microsoft autentifikācijas bibliotēku (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurā ir jaunākie līdzekļi un drošības atjauninājumi.

Ja izmantojat Microsoft programmas, ņemiet vērā, ka korporācija Microsoft pašlaik veic savu lietojumprogrammu migrāciju uz MSAL līdz atbalsta beigu termiņam, nodrošinot, ka uz tām attiecas MSAL pastāvīgie drošības un līdzekļu uzlabojumi.

1. [Lasīt bieži uzdotos jautājumus par ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Uzziniet, kā migrēt lietojumprogrammas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ja jums nepieciešama palīdzība, lai saprastu, kuras jūsu lietojumprogrammas izmanto ADAL, ieteicams pārskatīt visu jūsu lietojumprogrammu avota kodu un, ja nepieciešams, sazināties ar kādu ISV vai lietojumprogrammu nodrošinātāju. Microsoft atbalsta dienests var jums sniegt sarakstu ar visām jūsu nomniekā esošajām lietojumprogrammām, kas nav Microsoft ADAL lietojumprogrammas.

**AAD Graph migrācija**

Lietojumprogrammām, kas izmanto Azure AD Graph, izpildiet mūsu norādījumus, lai [migrētu Azure AD Graph uz Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Azure lietojumprogrammu reģistrācijas portālā tiek rādīts, kuras lietojumprogrammas izmanto AAD Graph. Iesakām pārskatīt visu jūsu lietojumprogrammu pirmkodu un, ja nepieciešams, sazināties ar jebkuru ISV vai lietojumprogrammu nodrošinātāju. Microsoft atbalsts var nodrošināt jums arī sarakstu ar visu AAD Graph lietojumu jūsu nomniekā.
3. Lai jūsu programma varētu piekļūt Microsoft Graph datiem, lietotājam vai administratoram tā ir jāpiešķir pareizās atļaujas, izmantojot piekrišanas procesu. Microsoft [Graph atsaucē ir](https://docs.microsoft.com/graph/permissions-reference) uzskaitītas atļaujas, kas saistītas ar katru galveno Microsoft Graph API kopu. Tajā arī sniegti norādījumi par atļauju lietošanu.
