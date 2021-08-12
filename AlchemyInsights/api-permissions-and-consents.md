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
ms.openlocfilehash: c45bab67d414c8f0f2ca1c5275084d4ecce538c5256154292302080ba5bd8175
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53932104"
---
# <a name="api-permissions-and-consent"></a>API atļaujas un piekrišana

Lietojumprogrammas, kas Microsoft indentitāšu platforma ar autorizācijas modeli, kas sniedz lietotājiem un administratoriem iespēju kontrolēt datu piekļuvi. Autorizācijas modeļa ieviešana ir atjaunināta e-Microsoft indentitāšu platforma galapunktā. Tas maina, kā lietojumprogrammai ir jāveic mijiedarbība ar Microsoft indentitāšu platforma. [Atļaujas un piekrišana galapunktā Microsoft indentitāšu platforma](https://docs.microsoft.com/azure/active-directory/develop/v2-permissions-and-consent) aptver šī autorizācijas modeļa pamatjēdzienos, tostarp tvērumus, atļaujas un piekrišanu.

Windows [Azure Active Directory (Azure AD) piekrišanas struktūra](https://docs.microsoft.com/azure/active-directory/develop/consent-framework) atvieglo vairāku nomnieku tīmekļa un vietējo klientu lietojumprogrammu izstrādāšanu. Šīs lietojumprogrammas ļauj pierakstīties lietotāju kontos no Azure AD nomnieka, kas atšķiras no tā, kurā ir reģistrēta programma. Viņiem var būt nepieciešama arī piekļuve tīmekļa API, piemēram, Microsoft Graph API (lai piekļūtu Azure AD, Intune un pakalpojumiem Microsoft 365) un citiem Microsoft pakalpojumi API papildus saviem tīmekļa API.

