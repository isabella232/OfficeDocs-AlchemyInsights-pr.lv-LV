---
title: Problēmas ar resursu vai pakalpojuma galveno nosaukumu
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
ms.openlocfilehash: 52b9b2e950d66c2f4105b76c4e2c70ed51320e4a57eb0008c353a9587fcc6510
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54028083"
---
# <a name="issues-with-a-resource-or-service-principal"></a>Problēmas ar resursu vai pakalpojuma galveno nosaukumu

1. Ja tikai sākat darbu, lietojumprogrammu un pakalpojumu galvenie objekti programmā [Azure Active Directory](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals) apraksta programmas reģistrāciju, lietojumprogrammas objektus un pakalpojuma galvenos nosaukumus programmā Azure Active Directory: kas tie ir, kā tie tiek izmantoti un kā tie ir saistīti. Tiek parādīts arī vairāku nomnieku piemēra scenārijs, lai ilustrētu relāciju starp lietojumprogrammas objektu un atbilstošajiem pakalpojuma pamatobjektiem.
2. Papildinformāciju par lietojumprogrammu un pakalpojumu pamatsummu relācijām varat uzzināt, lasot lietojumprogrammas un pakalpojuma galvenos objektus [Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/develop/app-objects-and-service-principals)
3. [How to:](https://docs.microsoft.com/azure/active-directory/develop/howto-create-service-principal-portal) Use the portal to create an Azure AD application and service principal that can access resources shows you how to create a new Azure Active Directory (Azure AD) application and service principal that can be used with the role-based access control.
4. Izmantojot pakalpojuma [galveno API,](https://docs.microsoft.com/graph/api/resources/serviceprincipal)varat programmiski pārvaldīt lietojumprogrammu instances un kontrolēt, kādas darbības lietojumprogramma var veikt jūsu nomniekā.
5. [servicePrincipal resursu tips uzskaita](https://docs.microsoft.com/graph/api/resources/serviceprincipal) visus servicePrincipal resursu tipa rekvizītus un metodes.
6. [Azure AD lietojumprogrammu un Microsoft Graph](https://docs.microsoft.com/graph/migrate-azure-ad-graph-resource-differences) resursu tipa Graph izceļ Azure AD Graph un Microsoft Graph atšķirības. Tā rāda resursus, kam ir atšķirīgi nosaukumi vai kuri nav pieejami. tas arī izceļ resursus, kas ir pieejami Microsoft Graph beta versijā, bet ne versijā v1.0.

**Problēmas ar vies lietotājiem**

- Īsā [pamācība:](https://docs.microsoft.com/azure/active-directory/external-identities/b2b-quickstart-add-guest-users-portal#prerequisites) Viesa lietotāju pievienošana Direktorijam Azure portālā parāda, kā pievienot jaunu viesa lietotāju savam Azure AD direktorijam, izmantojot Azure portālu, nosūtīt uzaicinājumu un skatīt, kā izskatās viesa lietotāja uzaicinājuma izpirkšanas process.
- [Apmācība: Izveidojiet lietotāju plūsmas Azure Active Directory B2C](https://docs.microsoft.com/azure/active-directory-b2c/tutorial-create-user-flows) parāda, kā izveidot dažas ieteicamās lietotāju plūsmas, izmantojot Azure portālu. Ja meklējat informāciju par to, kā lietojumprogrammā iestatīt resursu īpašnieka paroles akreditācijas datu (ROPC) plūsmu, skatiet rakstu Resursu īpašnieka paroles akreditācijas datu plūsmas konfigurēšana programmā Azure AD B2C.
