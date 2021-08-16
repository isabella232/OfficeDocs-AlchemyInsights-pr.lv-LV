---
title: Problēmas saistībā ar lietojumprogrammu izstrādi
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
ms.openlocfilehash: 065ff6d965063e44c4d1771821985058c9d020fbbabb0d381f30b6a11132c4ee
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54013431"
---
# <a name="issues-developing-applications"></a>Problēmas saistībā ar lietojumprogrammu izstrādi

Lai novērstu visbiežāk sastopamās problēmas, veidojot Azure Active Directory (AD) programmas, skatiet šos rakstus:

- [Tiek rādītas problēmas ar pierakstīšanos lietojumprogrammās, kas izmanto tikai pārlūkprogrammu Chrome](https://docs.microsoft.com/office365/troubleshoot/miscellaneous/chrome-behavior-affects-applications) 
- [Es nezinu, kā mainīt marķiera darbības laika noklusējumus savā lietojumprogrammā](https://docs.microsoft.com/azure/active-directory/develop/registration-config-change-token-lifetime-how-to) 
- [Es nesajauktu, kā darbojas lietojumprogrammas piekrišana](https://docs.microsoft.com/azure/active-directory/application-dev-consent-framework) 
- [Es nezinu, kā piešķirt atļaujas manai lietojumprogrammai](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent) 
- [Es nesaprotu atšķirību starp deleģētām un lietojumprogrammu atļaujām](https://docs.microsoft.com/azure/active-directory/develop/delegated-and-app-perms)

***Atbalsta beigas autentifikācijas Azure Active Directory bibliotēkai (ADAL) un Azure AD Graph API (AAD Graph)***

- Sākot ar 2020. gada 30. jūniju, mēs vairs nepievienosim jaunus līdzekļus Azure Active Directory autentifikācijas bibliotēkai (ADAL) un Azure AD Graph API (AAD Graph). Mēs turpināsim nodrošināt tehnisko atbalstu un drošības atjauninājumus, bet vairs nenodrošināsim līdzekļu atjauninājumus.

- Sākot ar 2022. gada 30. jūniju, mēs vairs nesniegsim ADAL un AAD Graph atbalstu un vairs nenodrošināsim tehnisko atbalstu vai drošības atjauninājumus. Šī nosacījuma rezultātā ir šādas sekas:

    - Lietojumprogrammas, kas izmanto ADAL esošajās OS versijās, turpinās darboties pēc šī datuma, taču nesaņems tehnisko atbalstu vai drošības atjauninājumus.

    - Programmas, kas izmanto AAD Graph šoreiz, iespējams, vairs nesaņems atbildes no AAD Graph galapunkta

**ADAL migrācija**

Ja izmantojat Microsoft programmas, iesakām atjaunināt uz Microsoft Authentication Library (MSAL) bibliotēku, kurā ir jaunākie līdzekļi un drošības atjauninājumi. Šis ieteikums ir Microsoft kontekstā uzsāciet programmu migrēšanas uz MSAL procesu līdz atbalsta beigu termiņam. 

Migrēšana no Microsoft uz MSAL nodrošina, ka lietojumprogrammas izmanto MSAL pastāvīgus drošības un līdzekļu uzlabojumus.

1. [Lasīt bieži uzdotos jautājumus par ADAL](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
2. [Uzziniet, kā migrēt lietojumprogrammas katrā platformā](https://docs.microsoft.com/azure/active-directory/develop/msal-migration#frequently-asked-questions-faq) 
3. Ja jums ir nepieciešama palīdzība, lai saprastu, kuras jūsu lietojumprogrammas izmanto ADAL, ieteicams pārskatīt visu jūsu lietojumprogrammu avota kodu un, ja nepieciešams, sazināties ar neatkarīgiem programmatūras piegādātājiem (ISV) vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsta dienests var jums sniegt sarakstu ar visām jūsu nomniekā esošajām lietojumprogrammām, kas nav Microsoft ADAL lietojumprogrammas.

**AAD Graph migrācija**

Lietojumprogrammām, kas izmanto AAD Graph, izpildiet mūsu norādījumus, lai migrētu AAD Graph uz Microsoft Graph:

1. [Mūsu migrācijas kontrolsaraksts nodrošina darba sākšanu](https://docs.microsoft.com/graph/migrate-azure-ad-graph-planning-checklist). 
2. Azure lietojumprogrammu reģistrācijas portālā tiek rādīts, kuras lietojumprogrammas izmanto AAD Graph. Iesakām pārskatīt visu savu lietojumprogrammu avota kodu un, ja nepieciešams, sazināties ar neatkarīgiem programmatūras piegādātājiem (ISV) vai lietojumprogrammu nodrošinātājiem. Microsoft atbalsts var sniegt jums arī informāciju par AAD Graph lietojumu jūsu nomniekā.







