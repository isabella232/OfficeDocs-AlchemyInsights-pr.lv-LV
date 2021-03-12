---
title: Problēmas ar resursu vai pakalpojumu pamatsummu
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
- "9004336"
- "7741"
ms.openlocfilehash: 9c37ad8e4dfecdb59a37d767f8eb4a5d99be7fa1
ms.sourcegitcommit: d13f23fb7994871d4e0e6e3e43672a101bd779e8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/28/2021
ms.locfileid: "50714078"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problēmas ar resursu vai pakalpojumu pamatsummu

1. Ja tikko esat sācis darbu, [lietojumprogrammu un pakalpojumu pamatobjekti Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) apraksta lietojumprogrammas reģistrācija, lietojumprogrammas objekti un pakalpojuma pamatrādītāji Azure Active Directory: kas tie ir, kā tie tiek izmantoti un kā tie ir savstarpēji saistīti. Tiek rādīts arī vairāku nomnieku piemērs, lai ilustrētu relāciju starp lietojumprogrammas objektu un atbilstošajiem pakalpojumu galvenajiem objektiem.
2. Varat uzzināt vairāk par relāciju starp lietojumprogrammām un pakalpojumu pamatprincipiem, izlasot [lietojumprogrammas un pakalpojuma pamatobjektus Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals).
3. [Kā: izmantot portālu, lai izveidotu AZURE ad lietojumprogrammu un pakalpojuma pamatsummu, kas var piekļūt resursiem](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) , ir parādīts, kā izveidot jaunu Azure Active Directory (Azure AD) lietojumprogrammu un pakalpojuma pamatsummu, ko var izmantot ar lomu piekļuves vadību.
4. Izmantojot [pakalpojuma galveno API](https://docs.microsoft.com/graph/api/resources/serviceprincipal), varat programmatiski pārvaldīt lietojumprogrammu gadījumus un kontrolēt to, ko lietojumprogramma var veikt jūsu nomniekā.
5. [servicePrincipal Resource Type](https://docs.microsoft.com/graph/api/resources/serviceprincipal) uzskaitīti visi servicePrincipal resursu tipa rekvizīti un metodes.
6. [Resursu tipa atšķirības starp AZURE ad Graph un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) izceļ atšķirības starp Azure AD Graph un Microsoft Graph Resource. Tajā ir parādīti resursi ar atšķirīgiem nosaukumiem vai nav pieejami. Tas arī izceļ resursus, kas pieejami Microsoft Graph beta versijā, bet nav v 1.0 versijā.

**Problēmas ar vieslietotājiem**

- [Quickstart: viesu lietotāju pievienošana direktorijam Azure portālā](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) ir parādīts, kā pievienot jaunu vieslietotāju savam Azure AD direktorijam, izmantojot Azure portālu, nosūtīt uzaicinājumu un uzzināt, kā izskatās viesa uzaicinājuma izpirkšanas process.
- [Apmācība: lietotāju plūsmu izveide pakalpojumā Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) rāda, kā izveidot dažas ieteicamās lietotāju plūsmas, izmantojot Azure portālu. Ja meklējat informāciju par to, kā iestatīt resursu īpašnieka paroles akreditācijas datu (ROPC) plūsmu lietojumprogrammā, skatiet rakstu resursu īpašnieka paroļu datu plūsmas konfigurēšana Azure AD B2C.
