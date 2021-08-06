---
title: Vaicājumu izmantošana Microsoft Graph API
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
- "7846"
ms.openlocfilehash: eda5d8d1d76d0d87312b1441aeae89d8e250abe0e8b613d4a43fcc2345a6f021
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53923246"
---
# <a name="querying-the-microsoft-graph-api"></a>Vaicājumu izmantošana Microsoft Graph API

Šī tēma var arī attiecas uz izstrādātājiem, kuri joprojām izmanto Azure AD Graph API. Tomēr ir stingri **ieteicams izmantot** Microsoft Graph visos direktorija, identitātes un piekļuves pārvaldības scenārijos.

**Autentifikācijas vai autorizācijas problēmas**

- Ja jūsu  lietojumprogramma nevar iegūt marķierus, lai zvanītu korporācijai Microsoft Graph, izvēlieties Problēma ar piekļuves pilnvaras **(autentifikācijas)** saņemšana Microsoft Graph kategoriju, lai saņemtu specifiskāku palīdzību un atbalstu šajā tēmā.
- Ja lietojumprogramma saņem **401 vai 403** autorizācijas kļūdas, zvanot Microsoft Graph, izvēlieties kategorijas Iegūt liegtu piekļuvi **kļūda (Autorizācija)** Microsoft Graph API, lai saņemtu specifiskāku palīdzību un atbalstu par šo tēmu.

**Es vēlos izmantot Microsoft Graph, taču nezinu, kur sākt**

Papildinformāciju par Microsoft Graph skatiet:

- [Pārskats par Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pārskats par identitātes un piekļuves pārvaldību programmā Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Darba sākšana, veidojot Microsoft Graph programmas](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** — microsoft Graph API jūsu nomniekā vai demonstrācijas nomniekā

**Es vēlos izmantot Microsoft Graph, bet vai tā atbalsta v1.0 direktorija API, kas nepieciešami?**

Microsoft Graph ir ieteicamais API direktorija, identitātes un piekļuves pārvaldībai. Tomēr starp Azure AD Graph un Microsoft Graph iespējamas atstarpes. Pārskatiet tālāk norādītos rakstus, kuros iezīmētas vistehnīgākās atšķirības, kas varētu palīdzēt izdarīt jūsu izvēli.

- [Azure AD Graph un Microsoft Graph resursu tipu atšķirības](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rekvizītu atšķirības starp Azure AD Graph un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Azure AD un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Veidojot vaicājumu lietotāja *objektam,* trūkst daudzu tā rekvizītu**

`GET https://graph.microsoft.com/v1.0/users`atgriež tikai 11 rekvizītus, jo Microsoft Graph automātiski atlasa noklusējuma lietotāja rekvizītu *kopu, kas* jāatgriež. Ja nepieciešami citi *lietotāja rekvizīti,* izmantojiet $select, lai izvēlētos lietojumprogrammas rekvizītus. Vispirms izmēģiniet to **pārlūkā Microsoft Graph Explorer.**

**Dažas lietotāja rekvizītu vērtības ir *Null pat tad,* ja es zinu, ka tās ir iestatītas**

Visdrīzāk tiek skaidrots, ka programmai ir piešķirta *atļauja User.ReadBasic.All.* Tādējādi lietojumprogramma var lasīt ierobežotu lietotāja rekvizītu kopu, atgriežot visus pārējos rekvizītus kā Null, pat ja tie ir iestatīti iepriekš. Mēģiniet piešķirt *lietojumprogrammu User.Read.All* atļauju.

Papildinformāciju skatiet rakstā [Microsoft Graph atļaujas](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Man ir problēmas, izmantojot OData vaicājuma parametrus, lai filtrētu manus pieprasījumus**

Lai gan Microsoft Graph atbalsta plašu OData vaicājumu parametru diapazonu, daudzi no šiem parametriem netiek pilnībā atbalstīti direktoriju pakalpojumi (resursi, kas pārmanto no *directoryObject*) programmā Microsoft Graph. Tie paši ierobežojumi, kas bija Azure AD Graph pastāv lielākajā daļā Microsoft Graph:

1. **Netiek atbalstīts**: $count, $search un $filter null *vai* *ne Null vērtībām*
2. **Netiek atbalstīts**: $filter par noteiktiem rekvizītiem (skatiet resursu tēmas par filtrējamiem rekvizītiem)
3. **Netiek atbalstīts:** vienlaikus lapošana, filtrēšana un kārtošana
4. **Netiek atbalstīts**: relācijas filtrēšana. Piemēram, atrodiet visus apvienotās Karalistes tehniskā grupa dalībniekus.
5. **Daļējs** atbalsts: $orderby *lietotājam* (tikai displayName un userPrincipalName) un *grupā*
6. **Daļējs** atbalsts : $filter (atbalsta tikai *eq*, start  *ar* *vai* *,* un , un ierobežots ) atbalstu, $expand (izvēršot viena objekta relācijas, tiek atgrieztas visas relācijas, bet objektu relāciju kolekcijas izvērššana ir ierobežota)

Papildinformāciju skatiet rakstā [Atbilžu pielāgošana, izmantojot vaicājuma parametrus.](https://docs.microsoft.com/graph/query-parameters)

**API, uz kuru zvanu, nedarbojas — kur var veikt papildu testēšanu?**

**Microsoft Graph Explorer** — pārbaudiet Microsoft Graph API jūsu nomniekā vai demonstrācijas nomniekā, kā arī skatiet vaicājumu **paraugus** programmā Microsoft Graph Explorer.

**Kad es izveidoju vaicājumu par datiem, šķiet, ka saņemu nepabeigtu datu kopu**

Ja vaicājumu kolekcijai (piemēram, *lietotājiem)* izmantojat microsoft Graph izmanto servera puses lapu ierobežojumus, lai rezultāti vienmēr tiek atgriezti ar noklusējuma lappuses izmēriem. Programmai vienmēr vajadzētu gaidīt, izmantojot pakalpojuma atgrieztās kolekcijas.

Papildinformāciju skatiet rakstā:

- [Microsoft Graph paraugprakse](https://docs.microsoft.com/graph/best-practices-concept)
- [Paging Microsoft Graph data in your app](https://docs.microsoft.com/graph/paging)

**Mana programma ir pārāk lēna un arī tiek ierobežošana. Kādus uzlabojumus var veikt?**

Atkarībā no scenārija jūsu rīcībā ir dažādas opcijas, lai padarītu lietojumprogrammu izpildāmāku, un dažos gadījumos arī mazāk noslodzētas pakalpojuma darbības laikā (ja veicat pārāk daudz zvanu).

Lai uzzinātu vairāk, skatiet:

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
