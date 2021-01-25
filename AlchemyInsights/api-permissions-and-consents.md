---
title: API atļaujas un piekrišana
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
- "7756"
ms.openlocfilehash: c99e5e2e8fb9bcc88e5221890ed9c28ed9e7d0c8
ms.sourcegitcommit: 605a73b159d30634b064c1b63b0e734ceb3fdec8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/25/2021
ms.locfileid: "49974608"
---
# <a name="api-permissions-and-consent"></a>API atļaujas un piekrišana

Lietojumprogrammas, kas ir integrētas ar Microsoft identitātes platformu, atbilst autorizācijas modelim, kas sniedz lietotājiem un administratoriem iespēju kontrolēt datu piekļuves iespējas. Autorizācijas modeļa ieviešana ir atjaunināta Microsoft identitātes platformas galapunktā. Tas maina, kā lietojumprogrammai ir jāmijiedarbojas ar Microsoft identitātes platformu. [Atļaujas un piekrišana Microsoft identitātes platformas galapunktā](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) attiecas uz šī autorizācijas modeļa pamatjēdzieniem, tostarp tvērumiem, atļaujām un piekrišanu.

[Azure Active Directory (AZURE AD) piekrišanas struktūra](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) ļauj viegli izveidot vairāku nomnieku tīmekļa un vietējo klientu lietojumprogrammas. Šīs lietojumprogrammas ļauj pierakstīties lietotāju kontos no Azure AD nomnieka, kas atšķiras no tās, kurā ir reģistrēta lietojumprogramma. Tiem, iespējams, būs jāpiekļūst arī tīmekļa API, piemēram, Microsoft Graph API (lai piekļūtu Azure AD, Intune un pakalpojumiem pakalpojumā Microsoft 365) un citos Microsoft pakalpojumu API papildus savam tīmekļa API.

