---
title: Problēmas saistībā ar lietojumprogrammu izstrādi ar API
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
ms.openlocfilehash: 1de4e9aa5078507eecdbe53366e446e733029ecb1342f20ca701fa7f95a06fa9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013467"
---
# <a name="issues-developing-applications-with-apis"></a>Problēmas saistībā ar lietojumprogrammu izstrādi ar API

Lai sāktu izmantot Azure Active Directory Graph API, skatiet [Azure AD Graph API īsās](https://docs.microsoft.com/azure/active-directory/develop/microsoft-graph-intro) lietošanas pamācību vai skatiet interaktīvo Azure AD Graph API [atsauču dokumentāciju](https://docs.microsoft.com/previous-versions/azure/ad/graph/api/api-catalog).

**Atbalsta beigas autentifikācijas Azure Active Directory bibliotēkai (ADAL) un Azure AD Graph API (AAD Graph)**

**Sākot ar 2020. gada 30.** jūnijs, mēs vairs ne pievienosim jaunus līdzekļus ADAL un Azure AD Graph. Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, bet vairs nenodrošināsim līdzekļu atjauninājumus.

**Sākot ar 2022. gada 30.** jūnijs, mēs nobeigsim atbalstu ADAL un Azure AD Graph un vairs nenodrošināsim tehniskā atbalsta vai drošības atjauninājumus.

Lietojumprogrammas, kas izmanto ADAL esošajās OS versijās, turpinās darboties pēc šī datuma, taču nesaņems tehnisko atbalstu vai drošības atjauninājumus.

Programmas, kas pēc Graph izmanto Azure AD Graph, iespējams, vairs nesaņems atbildes no Azure AD Graph galapunkta.

**ADAL migrācija**

Iesakām veikt atjaunināšanu uz [Microsoft autentifikācijas bibliotēku (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurā ir jaunākie līdzekļi un drošības atjauninājumi.

Ja izmantojat Microsoft programmas, ņemiet vērā, ka korporācija Microsoft pašlaik veic savu lietojumprogrammu migrāciju uz MSAL līdz atbalsta beigu termiņam, nodrošinot, ka to gūsit no MSAL pastāvīgas drošības un līdzekļu uzlabojumiem.

1. [Lasiet bieži uzdotos jautājumus par ADAL.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. [Uzziniet, kā migrēt programmas katrā platformā.](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
1. Ja jums nepieciešama palīdzība, lai saprastu, kuras jūsu lietojumprogrammas izmanto ADAL, ieteicams pārskatīt visu jūsu lietojumprogrammu avota kodu un, ja nepieciešams, sazināties ar kādu ISV vai lietojumprogrammu nodrošinātāju. Microsoft atbalsta dienests var jums sniegt sarakstu ar visām jūsu nomniekā esošajām lietojumprogrammām, kas nav Microsoft ADAL lietojumprogrammas.

**AAD Graph migrācija**

Lietojumprogrammām, kas izmanto Azure AD Graph, izpildiet mūsu norādījumus, lai [migrētu Azure AD Graph uz Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview?view=graph-rest-1.0&preserve-view=true)

1. [Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
1. Azure lietojumprogrammu reģistrācijas portālā tiek rādīts, kuras lietojumprogrammas izmanto AAD Graph. Iesakām pārskatīt visu jūsu lietojumprogrammu pirmkodu un, ja nepieciešams, sazināties ar jebkuru ISV vai lietojumprogrammu nodrošinātāju. Microsoft atbalsts var nodrošināt jums arī sarakstu ar visu AAD Graph lietojumu jūsu nomniekā.
1. Lai jūsu programma varētu piekļūt Microsoft Graph datiem, lietotājam vai administratoram tā ir jāpiešķir pareizās atļaujas, izmantojot piekrišanas procesu. Microsoft [Graph atsaucē ir](https://docs.microsoft.com/graph/permissions-reference?context=graph%2Fapi%2Fbeta&view=graph-rest-beta&preserve-view=true) uzskaitītas atļaujas, kas saistītas ar katru galveno Microsoft Graph API kopu. Tajā arī sniegti norādījumi par atļauju lietošanu.
