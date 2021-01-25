---
title: Problēmas, izstrādājot lietojumprogrammas
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7754"
- "9004342"
ms.openlocfilehash: 652fd6431201380e8e96619f63ecac15a6704d4f
ms.sourcegitcommit: 029c4697b77ce996d41ca74c4fa86de1bb84bd99
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974471"
---
# <a name="issues-developing-applications"></a>Problēmas, izstrādājot lietojumprogrammas

Lai novērstu izplatītākās problēmas, būvējot Azure Active Directory (AD) lietojumprogrammas, skatiet šos rakstus:

- [Man ir problēmas ar pierakstīšanos lietojumprogrammā (-ām), izmantojot tikai Chrome pārlūkprogrammu](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Es nezinu, kā mainīt marķierierīces ilguma noklusējumus manā lietojumprogrammā](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Esmu apjucis, kā darbojas lietojumprogrammu piekrišana](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Es nezinu, kā piešķirt atļaujas manai lietojumprogrammai](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Nesaprotu atšķirību starp deleģētajām un lietojumprogrammas atļaujām](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Azure Active Directory autentifikācijas bibliotēkas (ADAL) un AZURE ad GRAPH API (AAD Graph) atbalsta beigas**

- Sākot no 30. jūnija, 2020 vairs nepievienosit jaunus līdzekļus Azure Active Directory autentifikācijas bibliotēkai (ADAL) un Azure AD Graph API (AAD Graph). Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, taču vairs nenodrošinās līdzekļu atjauninājumus.

- Sākot no 30. jūnija, 2022, mēs nodrošināsim atbalstu ADAL un AAD Graph un vairs nenodrošinās tehnisko atbalstu vai drošības atjauninājumus. Šī nosacījuma rezultātā ietekmēs tālāk norādītās darbības.

    - Programmas, kas, izmantojot ADAL, pēc šī laika turpinās darboties, bet nesaņem nekādu tehnisku atbalstu vai drošības atjauninājumus.

    - Lietojumprogrammas, kas izmanto AAD Graph pēc šī laika, var vairs nesaņemt atbildes no AAD Graph galapunkta

*PārADAL migrācija**

Ja izmantojat Microsoft apps, iesakām atjaunināt Microsoft autentifikācijas bibliotēkā (MSAL), kurā ir jaunākie līdzekļi un drošības atjauninājumi. Šis ieteikums ir paredzēts korporācijai Microsoft, kas uzsāk procesu, lai migrētu tās lietojumprogrammas uz MSAL pēc atbalsta termiņa beigām. 

Migrēšana, ko korporācija Microsoft ir MSAL, nodrošina, ka lietojumprogrammas izmanto MSAL drošības un līdzekļu uzlabojumus.

1. [ADAL bieži uzdoto jautājumu lasīšana](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Uzziniet, kā migrēt programmas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ja jums ir nepieciešama palīdzība, lai izprastu, kuras jūsu lietojumprogrammas izmanto ADAL, iesakām pārskatīt visu savu programmu avota kodu un, ja nepieciešams, sazināties ar visiem neatkarīgiem programmatūras piegādātājiem (ISV) vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsts var arī nodrošināt, ka jūsu nomniekā ir saraksts ar visām programmām, kas nav Microsoft ADAL.

**AAD Graph migrācija**

Attiecībā uz lietojumprogrammām, kas izmanto AAD Graph, izpildiet mūsu norādījumus par to, kā migrēt AAD Graph programmas uz Microsoft Graph:

1. [Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanas punktu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Jūsu Azure lietojumprogrammu reģistrācijas portālā ir parādīts, kuras lietojumprogrammas izmanto AAD Graph. Iesakām pārskatīt visu savu lietojumprogrammu avota kodu un, ja nepieciešams, sazināties ar visiem neatkarīgiem programmatūras piegādātājiem (ISV) vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsts var arī sniegt informāciju par AAD Graph lietošanu nomniekā.







