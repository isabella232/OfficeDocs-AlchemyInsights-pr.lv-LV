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
ms.openlocfilehash: aa1525c6d221dbcfe91da7abd3d094ae1c228ece
ms.sourcegitcommit: 0f42d1600b6845083f0273d14c1d9e59344e4371
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/30/2020
ms.locfileid: "49564617"
---
# <a name="delete-tenant"></a>Nomnieka dzēšana

Lai izdzēstu Azure AD, pārliecinieties, vai:
- Jūs esat globālais administrators direktorijā.
- Jūs neesat pierakstījies, izmantojot kontu, kuram ir noklusējuma direktorijs, piemēram, contoso.onmicrosoft.com parakstītajā kontā, piemēram, admin@contoso.onmicrosoft.com.
- Noņemiet visas aktīvās lietojumprogrammas direktorijā pirms dzēšanas. Lai noņemtu aktīvās lietojumprogrammas, atveriet lietojumprogrammu reģistrācijas un noņemiet esošās lietojumprogrammas.
- Nevienam Microsoft tiešsaistes pakalpojumam, piemēram, Microsoft Azure, Office 365 vai Azure AD Premium, kas ir saistīts ar direktoriju, nav neviena aktīva abonementa. Pārsūtiet savus abonementus vai Paātriniet aktīvo abonementu atcelšanu, izmantojot Azure atbalstu un norēķinus. Uzziniet vairāk par to, kā atcelt Office 365 un Azure abonementus. Norādījumus par to, kā nomniekam piesaistīt vai pievienot esošu abonementu, skatiet sadaļā [AZURE ad nomnieka saistīšana vai pievienošana](https://docs.microsoft.com/azure/active-directory/fundamentals/active-directory-how-subscriptions-associated-directory).
- Nav nevienas aktīvas licences. Lai noņemtu licences, skatiet rakstu [kā noņemt abonementu, lai noņemtu licenci](https://docs.microsoft.com/azure/active-directory/enterprise-users/directory-delete-howto#delete-a-subscription).
- Nav citu aktīvu lietotāju direktorijā bez sevis kā globālais administrators, mēģinot izdzēst Azure AD. Noņemiet visus pārējos aktīvos lietotājus, bet, ja vēlaties, ir jānoņem, piemēram, ar admin@contoso.com izveidotie lietotāji.

Detalizētāku informāciju par to, kā:
- Dzēst "Azure Active Directory" vai "abonementu", skatiet rakstu [Azure Active Directory dzēšana](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-delete-howto).
- Noņemot lietojumprogrammas direktorijā, skatiet rakstu [lietojumprogrammu noņemšana](https://docs.microsoft.com/azure/active-directory/develop/quickstart-remove-app). 
