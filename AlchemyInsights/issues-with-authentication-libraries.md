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
ms.openlocfilehash: ab4ffbc78a7cadd8acee3c98eaa5f3323da9c7e3
ms.sourcegitcommit: 7e6d89f47eca1babf5aeba4995bceccd990c3963
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/28/2021
ms.locfileid: "50063637"
---
# <a name="issues-with-authentication-libraries"></a>Problēmas ar autentifikācijas bibliotēkām

1. [Microsoft identitātes platformas autentifikācijas bibliotēkas](https://docs.microsoft.com/azure/active-directory/develop/reference-v2-libraries) norāda Microsoft atbalstītās un saderīgās klienta un starpprogrammatūras bibliotēkas.
2. Microsoft autentifikācijas bibliotēka (MSAL) atbalsta vairākas [autentifikācijas plūsmas](https://docs.microsoft.com/azure/active-directory/develop/msal-authentication-flows) , kas jāizmanto dažādos lietojumprogrammas scenārijos.
3. Lai autentificētu un iegūtu marķierierīces, kodā inicializējiet jaunu publisku vai konfidenciālu klienta lietojumprogrammu. Varat iestatīt vairākas konfigurācijas opcijas, ja inicializējat klienta programmu Microsoft autentifikācijas bibliotēkā (MSAL). Lai uzzinātu vairāk, skatiet sadaļu [lietojumprogrammas konfigurācijas opcijas](https://docs.microsoft.com/azure/active-directory/develop/msal-client-application-configuration).

**Azure Active Directory autentifikācijas bibliotēkas (ADAL) un Azure AD Graph API (AAD Graph) atbalsta beigas**

**Sākot no 30. jūnija, 2020**, vairs nepievienosit nekādus jaunus līdzekļus, kas ADAL un Azure AD Graph. Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, bet vairs nenodrošināsim līdzekļu atjauninājumus.

**Sākot no 30. jūnija, 2022**, mēs NODROŠINĀSIM atbalstu ADAL un Azure AD Graph un vairs nenodrošinās tehnisko atbalstu vai drošības atjauninājumus.

Programmas, kas, izmantojot ADAL, pēc šī laika turpinās darboties, bet *nesaņem nekādu tehnisku atbalstu vai drošības atjauninājumus*.

Lietojumprogrammas, kas izmanto Azure AD Graph pēc šī laika, iespējams, vairs nesaņems atbildes no Azure AD Graph galapunkta.

**PārADAL migrācija**

Iesakām veikt atjaunināšanu uz [Microsoft autentifikācijas bibliotēku (MSAL)](https://docs.microsoft.com/azure/active-directory/develop/v2-overview), kurā ir jaunākie līdzekļi un drošības atjauninājumi.

Ja izmantojat Microsoft programmas, zināt, ka korporācija Microsoft pašlaik veic savu lietojumprogrammu migrēšanu uz MSAL, izmantojot atbalsta termiņu, lai nodrošinātu, ka tās gūs labumu no MSAL pašreizējiem drošības un līdzekļu uzlabojumiem.

Papildinformāciju skatiet šeit:

1. [Lasīt bieži uzdotos jautājumus par ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
2. [Uzziniet, kā migrēt lietojumprogrammas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq)
3. Ja jums ir nepieciešama palīdzība, lai izprastu, kura lietojumprogramma izmanto ADAL, iesakām pārskatīt visu savu programmu avota kodu un pēc vajadzības sazināties ar citiem ISV vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsta dienests var jums sniegt sarakstu ar visām jūsu nomniekā esošajām lietojumprogrammām, kas nav Microsoft ADAL lietojumprogrammas.

**AAD Graph migrācija**

Lietojumprogrammas, kas izmanto Azure AD Graph, izpildiet mūsu norādījumus, lai [migrētu AZURE ad Graph programmas uz Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-overview).

1. [Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanas punktu.](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist)
2. Azure lietojumprogrammu reģistrācijas portālā tiek rādīts, kuras lietojumprogrammas izmanto AAD Graph. Iesakām pārskatīt visu jūsu lietojumprogrammu pirmkodu un, ja nepieciešams, sazināties ar jebkuru ISV vai lietojumprogrammu nodrošinātāju. Microsoft atbalsts var arī nodrošināt, lai jūsu nomniekā tiktu parādīts visu AAD Graph izmantošanas saraksts.
3. Lai jūsu programmai piekļūtu datiem programmā Microsoft Graph, lietotājam vai administratoram tā ir jāpiešķir pareizas atļaujas, izmantojot piekrišanas procesu. [Microsoft Graph atļauju atsaucēs](https://docs.microsoft.com/graph/permissions-reference) ir uzskaitītas atļaujas, kas ir saistītas ar katru galveno Microsoft Graph API kopu. Tajā sniegti arī norādījumi par to, kā izmantot atļaujas.
