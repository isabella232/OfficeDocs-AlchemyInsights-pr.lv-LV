---
title: Nomnieka dzēšana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 11/23/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003256"
- "7297"
ms.openlocfilehash: 7377f77b7295e8134673c9a46fa7606842d4df949f535878d13986c6d39d0b5e
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53993900"
---
# <a name="delete-tenant"></a>Nomnieka dzēšana

Lai izdzēstu Azure AD, pārliecinieties, vai:
- Jūs esat globālais administrators direktorijā.
- Neesat pierakstījies ar kontu, kuram ir noklusējuma direktorijs, piemēram, contoso.onmicrosoft.com pierakstīšanās kontā, piemēram, admin@contoso.onmicrosoft.com.
- Pirms dzēšanas noņemiet direktorijā visas aktīvās lietojumprogrammas. Lai noņemtu aktīvās lietojumprogrammas, naviģējiet uz programmu reģistrācijām un noņemiet esošās lietojumprogrammas.
- Nav aktīvu Microsoft Online Services abonementu, piemēram, Microsoft Azure, Office 365 vai Azure AD Premium, kas saistīti ar šo direktoriju. Pārsūtiet savus abonementus vai paātrinātu aktīvo abonementu atcelšanu, izmantojot Azure atbalstu un norēķinus. Uzziniet vairāk par to, kā atcelt Office 365 Azure abonementus. Norādījumus par to, kā nomniekam piesaistīt vai pievienot esošu abonementu, skatiet rakstā Azure abonementa saistīšana vai pievienošana [Azure nomniekam.](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory)
- Nav aktīvas licences. Lai noņemtu licences, skatiet rakstu [Kā noņemt abonementu, lai noņemtu licenci](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Direktorijā nav citu aktīvu lietotāju, ne tikai jūs kā globālais administrators, kad mēģināt izdzēst Azure AD. Noņemiet visus pārējos aktīvos lietotājus, kā arī atkarību no nomnieka pielāgotā domēna nosaukuma, piemēram, lietotājus, kas izveidoti ar admin@contoso.com.

Lai iegūtu detalizētu informāciju par to, kā:
- Izdzēsiet "Azure Active Directory" vai "abonements", skatiet [rakstu Azure Active Directory.](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto)
- Noņemot lietojumprogrammas direktorijā, skatiet [sadaļu Lietojumprogrammu noņemšana](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
