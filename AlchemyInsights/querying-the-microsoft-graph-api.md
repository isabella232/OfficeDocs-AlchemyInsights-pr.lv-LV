---
title: Microsoft Graph API vaicājumu
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
ms.openlocfilehash: 527e88c7b3cb1cc4f5535e3b0d2bc4d8d1163336
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974422"
---
# <a name="querying-the-microsoft-graph-api"></a>Microsoft Graph API vaicājumu

Šī tēma var attiekties arī uz izstrādātājiem, kuri joprojām izmanto Azure AD Graph API. Tomēr ir **stingri** ieteicams izmantot programmu Microsoft Graph visiem jūsu direktorija, identitātes un piekļuves pārvaldības scenārijiem.

**Autentifikācijas vai autorizācijas problēmas**

- Ja jūsu lietojumprogramma **nevar iegūt pilnvaras** , lai sasauktu Microsoft Graph, izvēlieties problēmu, kas rodas, **iegūstot piekļuves marķiera (autentifikāciju)** Microsoft Graph kategoriju, lai saņemtu konkrētāku palīdzību un atbalstu šajā tēmā.
- Ja jūsu programma **saņem 401 vai 403 autorizācijas kļūdas** , zvanot uz Microsoft Graph, izvēlieties, vai Microsoft Graph API kategorijā iegūt **Access denied kļūdu (autorizācija)** .

**Es vēlos izmantot programmu Microsoft Graph, taču neesat pārliecināts, kur sākt**

Lai uzzinātu vairāk par Microsoft Graph, skatiet:

- [Pārskats par Microsoft Graph](https://docs.microsoft.com/graph/overview)
- [Pārskats par identitāti un piekļuves pārvaldību programmā Microsoft Graph](https://docs.microsoft.com/graph/azuread-identity-access-management-concept-overview)
- [Darba sākšana Microsoft Graph programmu izveidē](https://docs.microsoft.com/graph/)
- **Microsoft Graph Explorer** — testējiet Microsoft Graph API nomniekā vai demonstrācijas nomniekā

**Es vēlos izmantot Microsoft Graph, bet vai tas atbalsta v 1.0 direktorija API, kas man ir nepieciešams?**

Microsoft Graph ir ieteicamais API direktorijam, identitātei un piekļuves pārvaldībai. Tomēr ir vēl dažas atšķirības starp to, kas ir iespējams Azure AD Graph un Microsoft Graph. Pārskatiet tālāk norādītos rakstus, kas izceļ visaktuālākās atšķirības, lai palīdzētu jums izvēlēties:

- [Resursu tipa atšķirības starp Azure AD Graph un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences)
- [Rekvizītu atšķirības starp Azure AD Graph un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-property-differences)
- [Metodes atšķirības starp Azure AD un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-method-differences)

**Veicot vaicājumu *lietotāja* objektam, trūkst daudz tā rekvizītu**

`GET https://graph.microsoft.com/v1.0/users` atgriež tikai 11 rekvizītus, jo Microsoft Graph automātiski atlasa noklusējuma *lietotāju* rekvizītu kopu, kas jāatgriež. Ja ir nepieciešami citi *lietotāja* rekvizīti, izmantojiet $SELECT, lai izvēlētos lietojumprogrammas rekvizītus. Vispirms izmēģiniet to programmā **Microsoft Graph Explorer** .

**Dažas lietotāja rekvizīta vērtības ir *Null* , kaut gan es zinu, ka tās ir iestatītas**

Visticamākais skaidrojums ir tāds, ka lietojumprogrammai ir piešķirts *lietotājs. ReadBasic. All* permissions. Tas ļauj lietojumprogrammai lasīt ierobežotu lietotāja rekvizītu kopu, atgriežot visus pārējos rekvizītus kā Null pat tad, ja tie ir iepriekš iestatīti. Mēģiniet piešķirt lietojumprogrammas *lietotāju. Read. All* Permission tā vietā.

Lai iegūtu papildinformāciju, skatiet rakstu [Microsoft Graph lietotāju atļaujas](https://docs.microsoft.com/graph/permissions-reference#user-permissions).

**Man rodas problēmas, izmantojot OData vaicājuma parametrus, lai filtrētu datus manos pieprasījumos**

Kamēr Microsoft Graph atbalsta plašu OData vaicājuma parametru diapazonu, daudzus no šiem parametriem pilnībā neatbalsta direktoriju pakalpojumi (resursi, kas pārmanto no *directoryObject*) programmā Microsoft Graph. Tie paši ierobežojumi, kas bija atrodami Azure AD Graph programmā Microsoft Graph, joprojām ir iespējami lielākoties:

1. **Netiek atbalstīts**: $count, $search un $Filter vērtību *Null* vai *Not Null*
2. **Netiek atbalstīts**: $Filter noteiktos rekvizītos (skatīt resursu tēmas, kuru rekvizītus var filtrēt)
3. **Netiek atbalstīts**: lapošana, filtrēšana un kārtošana vienlaikus
4. **Netiek atbalstīts**: relācijas filtrēšana. Piemēram, atrodiet visus tās tehniskās grupas dalībniekus, kas ir Apvienotajā Karalistē.
5. **Daļējs atbalsts**: $orderby *lietotājam* (tikai displayName un userPrincipalName) un *grupu*
6. **Daļējs atbalsts**: $Filter (atbalsta tikai *EQ*, startswith *,* *kā arī* *un ierobežots)* atbalstu, $Expand (viena objekta relāciju izvēršana atgriež visas relācijas, taču objektu kopuma paplašināšana ir ierobežota) 

Lai iegūtu papildinformāciju, skatiet rakstu [atbilžu pielāgošana ar vaicājuma parametriem](https://docs.microsoft.com/graph/query-parameters).

**API, ko es saukšu, nedarbojas — kur varu veikt papildu testēšanu?**

**Microsoft Graph Explorer** — testējiet Microsoft Graph API savā nomniekā vai demonstrācijas nomniekā, kā arī skatiet **vaicājumu piemērus** programmā Microsoft Graph Explorer.

**Veicot vaicājumu, lai iegūtu datus, šķiet, ka tiek atgriezta nepilnīga datu kopa**

Ja veicat vaicājumu par kolekciju (piemēram, *lietotāji*), Microsoft Graph izmanto servera puses lappušu ierobežojumus, tāpēc rezultāti vienmēr tiek atgriezti, izmantojot noklusējuma lappuses izmērus. Jūsu programmai vienmēr būtu jāgaida no pakalpojuma atdots kolekcijas.

Papildinformāciju skatiet rakstā:

- [Microsoft Graph paraugprakse](https://docs.microsoft.com/graph/best-practices-concept)
- [Microsoft Graph datu lapošana jūsu lietojumprogrammā](https://docs.microsoft.com/graph/paging)

**Mana programma ir pārāk lēna, un tiek arī panākta ierobežošana. Kādus uzlabojumus varu veikt?**

Atkarībā no tā jūsu rīcībā ir dažādi varianti, kā jūsu lietojumprogrammā veikt papildu darbības, un dažos gadījumos mazāk noslieces uz darbu, izmantojot pakalpojumu (kad veicat pārāk daudz zvanu).

Lai uzzinātu vairāk, skatiet:

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
