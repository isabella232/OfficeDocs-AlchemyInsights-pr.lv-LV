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
ms.openlocfilehash: a856094d9152568c3c067da5856153230d6590a6
ms.sourcegitcommit: 9d03083ea6e18070296b87a1b02339ca4d8e6064
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/29/2021
ms.locfileid: "50714152"
---
# <a name="microsoft-graph-api-issues"></a>Microsoft Graph API problēmas

Šī tēma var attiekties arī uz izstrādātājiem, kuri joprojām izmanto Azure AD Graph API. Tomēr ir **stingri** ieteicams izmantot programmu Microsoft Graph visiem jūsu direktorija, identitātes un piekļuves pārvaldības scenārijiem.

**Autentifikācijas vai autorizācijas problēmas**

- Ja jūsu lietojumprogramma **nevar iegūt pilnvaras** , lai sasauktu Microsoft Graph, izvēlieties problēmu, kas rodas, **iegūstot piekļuves marķiera (autentifikāciju)** Microsoft Graph kategoriju, lai saņemtu konkrētāku palīdzību un atbalstu šajā tēmā.
- Ja jūsu programma **saņem 401 vai 403 autorizācijas kļūdas** , zvanot uz Microsoft Graph, izvēlieties, vai Microsoft Graph API kategorijā iegūt **Access denied kļūdu (autorizācija)** .

**Es vēlos izmantot programmu Microsoft Graph, taču neesat pārliecināts, kur sākt**

- [Pārskats par Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pārskats par identitāti un piekļuves pārvaldību programmā Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Darba sākšana Microsoft Graph programmu izveidē](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** — testējiet Microsoft Graph API nomniekā vai demonstrācijas nomniekā

**Es vēlos izmantot Microsoft Graph, bet vai tas atbalsta v 1.0 direktorija API, kas man ir nepieciešams?**

Microsoft Graph ir ieteicamais API direktorijam, identitātei un piekļuves pārvaldībai. Tomēr ir vēl dažas atšķirības starp to, kas ir iespējams Azure AD Graph un Microsoft Graph. Pārskatiet tālāk norādītos rakstus, kas izceļ visaktuālākās atšķirības, lai palīdzētu jums izvēlēties:

- [Resursu tipa atšķirības starp Azure AD Graph un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rekvizītu atšķirības starp Azure AD Graph un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Metodes atšķirības starp Azure AD un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**API, ko es saukšu, nedarbojas — kur varu veikt papildu testēšanu?**

**Microsoft Graph Explorer** — testējiet Microsoft Graph API savā nomniekā vai demonstrācijas nomniekā, kā arī skatiet **vaicājumu piemērus** programmā Microsoft Graph Explorer.

**Mana programma ir pārāk lēna, un tiek arī panākta ierobežošana. Kādus uzlabojumus varu veikt?**

Atkarībā no jūsu darbības ir pieejamas vairākas iespējas, kā izmantot savu lietojumprogrammu, lai nodrošinātu, ka jūsu lietojumprogramma darbojas, un dažos gadījumos tā ir mazāk nosliece uz pakalpojumu ierobežošanu (kad veicat pārāk daudz zvanu).

- [Microsoft Graph paraugprakse](https://docs.microsoft.com/graph/best-practices-concept)
- [Pakešapstrādes pieprasījumi](https://docs.microsoft.com/graph/json-batching)
- [Izmaiņu reģistrēšana, izmantojot Delta vaicājumu](https://docs.microsoft.com/graph/delta-query-overview)
- [Saņemiet paziņojumus par izmaiņām, izmantojot āķus](https://docs.microsoft.com/graph/webhooks)
- [Ierobežošanas norādījumi](https://docs.microsoft.com/graph/throttling)

**Kur var iegūt papildinformāciju par kļūdām un zināmajām problēmām?**

- [Microsoft Graph kļūdas atbilžu informācija](https://docs.microsoft.com/graph/errors)
- [Zināmās problēmas ar Microsoft Graph](https://docs.microsoft.com/graph/known-issues)

**Kur varu pārbaudīt pakalpojumu pieejamības un savienojamības statusu?**

Pamata pakalpojumu pieejamība un savienojamība, kam var piekļūt, izmantojot Microsoft Graph, var ietekmēt Microsoft Graph vispārējo pieejamību un veiktspēju.

- Azure Active Directory pakalpojuma darbspējas pārbaudei pārbaudiet statusu **drošības + identitātes** pakalpojumi, kas norādīti [Azure statusa lapā](https://azure.microsoft.com/status/).
- Office pakalpojumiem, kas sniedz ieguldījumu programmā Microsoft Graph, pārbaudiet pakalpojumu statusu, kas norādīti [Office pakalpojumu darbspējas informācijas panelī](https://portal.office.com/adminportal/home#/servicehealth).

Microsoft Graph autorizācijas kļūdas var būt vairāku atšķirīgu problēmu rezultāts, no kurām lielākā daļa rada 401 vai 403 kļūdu. Piemēram, tālāk norādītās darbības var izraisīt autorizācijas kļūdas.

- Nepareizas [piekļuves pilnvaru iegūšanas plūsmas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-authentication-scenarios)
- Nepareizi konfigurēti [atļauju tvērumi](https://docs.microsoft.com/azure/active-directory/develop/active-directory-v2-scopes)
- [Piekrišanas](https://docs.microsoft.com/azure/active-directory/develop/active-directory-devhowto-multi-tenant-overview#understanding-user-and-admin-consent) trūkums

**_Azure Active Directory autentifikācijas bibliotēkas (ADAL) un Azure AD Graph API (AAD Graph) atbalsta beigas_* _

* * Sākot Jūnijs 30, 2020 * *, mēs vairs nepievienos nekādus jaunus līdzekļus, kas ADAL un Azure AD Graph. Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, bet vairs nenodrošināsim līdzekļu atjauninājumus.

**Sākot no 30. jūnija, 2022**, mēs NODROŠINĀSIM atbalstu ADAL un Azure AD Graph un vairs nenodrošinās tehnisko atbalstu vai drošības atjauninājumus.

Programmas, kas, izmantojot ADAL, pēc šī laika turpinās darboties, bet *nesaņem nekādu tehnisku atbalstu vai drošības atjauninājumus*.

Lietojumprogrammas, kas izmanto Azure AD Graph pēc šī laika, iespējams, vairs nesaņems atbildes no Azure AD Graph galapunkta.

**PārADAL migrācija**

Iesakām veikt atjaunināšanu uz [Microsoft autentifikācijas bibliotēku (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurā ir jaunākie līdzekļi un drošības atjauninājumi.

Ja izmantojat Microsoft programmas, zināt, ka korporācija Microsoft pašlaik veic savas lietojumprogrammas migrāciju uz MSAL līdz atbalsta termiņa beigām, nodrošinot, ka tās gūs labumu no MSAL pastāvīgajiem drošības un līdzekļu uzlabojumiem.

1. [Lasīt bieži uzdotos jautājumus par ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Uzziniet, kā migrēt lietojumprogrammas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ja jums ir nepieciešama palīdzība, lai izprastu, kura lietojumprogramma izmanto ADAL, iesakām pārskatīt visu savu programmu avota kodu un pēc vajadzības sazināties ar citiem ISV vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsta dienests var jums sniegt sarakstu ar visām jūsu nomniekā esošajām lietojumprogrammām, kas nav Microsoft ADAL lietojumprogrammas.

**AAD Graph migrācija**

Lietojumprogrammas, kas izmanto Azure AD Graph, izpildiet mūsu norādījumus, lai [migrētu AZURE ad Graph programmas uz Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist).
2. Azure lietojumprogrammu reģistrācijas portālā tiek rādīts, kuras lietojumprogrammas izmanto AAD Graph. Iesakām pārskatīt visu jūsu lietojumprogrammu pirmkodu un, ja nepieciešams, sazināties ar jebkuru ISV vai lietojumprogrammu nodrošinātāju. Microsoft atbalsts var arī nodrošināt, lai jūsu nomniekā tiktu parādīts visu AAD Graph izmantošanas saraksts.
3. Lai jūsu programmai piekļūtu datiem programmā Microsoft Graph, lietotājam vai administratoram tā ir jāpiešķir pareizas atļaujas, izmantojot piekrišanas procesu. [Microsoft Graph atļauju atsaucēs](https://docs.microsoft.com/graph/permissions-reference) ir uzskaitītas atļaujas, kas ir saistītas ar katru galveno Microsoft Graph API kopu. Tajā sniegti arī norādījumi par to, kā izmantot atļaujas.
