---
title: Problēmas, kas izstrādā lietojumprogrammas ar API
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
- "9004343"
- "7755"
ms.openlocfilehash: 26d732819b64efa4fb84da44cc2a279368aa28b0
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974622"
---
# <a name="issues-developing-applications-with-apis"></a>Problēmas, kas izstrādā lietojumprogrammas ar API

Lai sāktu izmantot Azure Active Directory Graph API, skatiet [AZURE ad GRAPH API Quickstart Guide](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) vai skatiet [interaktīvo AZURE ad Graph API atsauces dokumentāciju](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Azure Active Directory autentifikācijas bibliotēkas (ADAL) un Azure AD Graph API (AAD Graph) atbalsta beigas**

**Sākot no 30. jūnija, 2020**, vairs nepievienosit nekādus jaunus līdzekļus, kas ADAL un Azure AD Graph. Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, taču vairs nenodrošinās līdzekļu atjauninājumus.

**Sākot no 30. jūnija, 2022**, mēs NODROŠINĀSIM atbalstu ADAL un Azure AD Graph un vairs nenodrošinās tehnisko atbalstu vai drošības atjauninājumus.

Programmas, kas, izmantojot ADAL, pēc šī laika turpinās darboties, bet nesaņem nekādu tehnisku atbalstu vai drošības atjauninājumus.

Lietojumprogrammas, kas izmanto Azure AD Graph pēc šī laika, iespējams, vairs nesaņems atbildes no Azure AD Graph galapunkta.

**PārADAL migrācija**

Ieteicams atjaunināt [Microsoft autentifikācijas bibliotēkā (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurā ir jaunākie līdzekļi un drošības atjauninājumi.

Ja izmantojat Microsoft programmas, zināt, ka korporācija Microsoft pašlaik veic savas lietojumprogrammas migrāciju uz MSAL, izmantojot atbalsta termiņu, nodrošinot, ka tās gūs labumu no MSAL pastāvīgajiem drošības un līdzekļu uzlabojumiem.

1. [Lasiet bieži uzdotos jautājumus par ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. [Uzziniet, kā migrēt programmas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq).
1. Ja jums ir nepieciešama palīdzība, lai izprastu, kura lietojumprogramma izmanto ADAL, iesakām pārskatīt visu savu programmu avota kodu un pēc vajadzības sazināties ar citiem ISV vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsts var arī nodrošināt, ka jūsu nomniekā ir saraksts ar visām programmām, kas nav Microsoft ADAL.

**AAD Graph migrācija**

Lietojumprogrammas, kas izmanto Azure AD Graph, izpildiet mūsu norādījumus, lai migrētu [AZURE ad Graph programmas uz Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true).

1. [Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanas punktu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Jūsu Azure lietojumprogrammu reģistrācijas portālā ir parādīts, kuras lietojumprogrammas izmanto AAD Graph. Iesakām pārskatīt visu savu lietojumprogrammu avota kodu un, ja nepieciešams, sazināties ar citiem ISV vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsts var arī nodrošināt, lai jūsu nomniekā tiktu parādīts visu AAD Graph izmantošanas saraksts.
1. Lai jūsu programmai piekļūtu datiem programmā Microsoft Graph, lietotājam vai administratoram tā ir jāpiešķir pareizas atļaujas, izmantojot piekrišanas procesu. [Microsoft Graph atļauju atsaucēs](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) ir uzskaitītas atļaujas, kas ir saistītas ar katru galveno Microsoft Graph API kopu. Tajā sniegti arī norādījumi par to, kā izmantot atļaujas.
