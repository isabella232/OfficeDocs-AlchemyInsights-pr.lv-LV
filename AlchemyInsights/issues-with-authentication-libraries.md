---
title: Problēmas ar autentifikācijas bibliotēkām
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
- "9004333"
- "7731"
ms.openlocfilehash: 39336fa8840a28befcad449d0afa59c1df5c6bef5988cb197916a03aa2aa66c9
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028011"
---
# <a name="issues-with-authentication-libraries"></a>Problēmas ar autentifikācijas bibliotēkām

1. [Microsoft indentitāšu platforma bibliotēkās ir uzskaitītas](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) Microsoft atbalstītās un saderīgas klientu un starpprogrammatūras bibliotēkas.
2. Microsoft autentifikācijas bibliotēka (MSAL) atbalsta vairākas [autentifikācijas plūsmas](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) izmantošanai dažādos programmas scenārijos.
3. Lai autentificētu un iegūtu marķierus, jūs inicializējiet jaunu publisko vai konfidenciālu klienta lietojumprogrammu savā kodā. Varat iestatīt vairākas konfigurācijas opcijas, inicializējot klienta lietojumprogrammu Microsoft Authentication Library (MSAL). Papildinformāciju skatiet rakstā [Lietojumprogrammu konfigurācijas opcijas](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Atbalsta beigas autentifikācijas Azure Active Directory bibliotēkai (ADAL) un Azure AD Graph API (AAD Graph)**

**Sākot ar 2020. gada 30.** jūnijs, mēs vairs ne pievienosim jaunus līdzekļus ADAL un Azure AD Graph. Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, bet vairs nenodrošināsim līdzekļu atjauninājumus.

**Sākot ar 2022. gada 30.** jūnijs, mēs nobeigsim atbalstu ADAL un Azure AD Graph un vairs nenodrošināsim tehniskā atbalsta vai drošības atjauninājumus.

Programmas, kas izmanto ADAL esošajās OS versijās, pēc šī laika turpinās darboties, bet netiks *saņemts tehniskais atbalsts vai drošības atjauninājumi.*

Programmas, kas pēc Graph izmanto Azure AD Graph, iespējams, vairs nesaņems atbildes no Azure AD Graph galapunkta.

**ADAL migrācija**

Iesakām veikt atjaunināšanu uz [Microsoft autentifikācijas bibliotēku (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurā ir jaunākie līdzekļi un drošības atjauninājumi.

Ja izmantojat Microsoft programmas, ņemiet vērā, ka korporācija Microsoft pašlaik veic savu lietojumprogrammu migrāciju uz MSAL līdz atbalsta beigu termiņam, nodrošinot, ka to gūs labumu no MSAL pastāvīgaajiem drošības un līdzekļu uzlabojumiem.

Papildinformāciju skatiet rakstā:

1. [Lasīt bieži uzdotos jautājumus par ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Uzziniet, kā migrēt lietojumprogrammas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ja jums nepieciešama palīdzība, lai saprastu, kuras jūsu lietojumprogrammas izmanto ADAL, ieteicams pārskatīt visu jūsu lietojumprogrammu avota kodu un, ja nepieciešams, sazināties ar kādu ISV vai lietojumprogrammu nodrošinātāju. Microsoft atbalsta dienests var jums sniegt sarakstu ar visām jūsu nomniekā esošajām lietojumprogrammām, kas nav Microsoft ADAL lietojumprogrammas.

**AAD Graph migrācija**

Lietojumprogrammām, kas izmanto Azure AD Graph, izpildiet mūsu norādījumus, lai [migrētu Azure AD Graph uz Microsoft Graph.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview)

1. [Mūsu migrācijas kontrolsaraksts sniedz darba sākšanas punktu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure lietojumprogrammu reģistrācijas portālā tiek rādīts, kuras lietojumprogrammas izmanto AAD Graph. Iesakām pārskatīt visu jūsu lietojumprogrammu pirmkodu un, ja nepieciešams, sazināties ar jebkuru ISV vai lietojumprogrammu nodrošinātāju. Microsoft atbalsts var nodrošināt jums arī sarakstu ar visu AAD Graph lietojumu jūsu nomniekā.
3. Lai jūsu programma varētu piekļūt Microsoft Graph datiem, lietotājam vai administratoram tā ir jāpiešķir pareizās atļaujas, izmantojot piekrišanas procesu. Microsoft [Graph atsaucē ir](https://docs.microsoft.com/graph/permissions-reference) uzskaitītas atļaujas, kas saistītas ar katru galveno Microsoft Graph API kopu. Tajā arī sniegti norādījumi par atļauju lietošanu.
