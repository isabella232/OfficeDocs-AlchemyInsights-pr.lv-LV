---
title: Programmas starpniekservera konfigurācija
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
- "9004356"
- "7800"
ms.openlocfilehash: 835bfc59f77b31dc9a37c98db911505e2c7a758b37406dfc4da2d139afa61db5
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53951572"
---
# <a name="app-proxy-configuration"></a>Programmas starpniekservera konfigurācija

1. Lai izprastu, kā konfigurēt lietojumprogrammas starpniekservera lietojumprogrammu vidē Azure AD, lai atklātu lokālās lietojumprogrammas mākonī, skatiet rakstu Kā [konfigurēt lietojumprogrammas starpniekservera lietojumprogrammu.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to)
2. Vienotā pierakstīšanās (Single sign-on — SSO) sniedz lietotājiem iespēju piekļūt lietojumprogrammai, neveicot autentificēšanu vairākas reizes. Tādējādi viena autentifikācija tiek veikta mākonī, salīdzinot ar Azure Active Directory, un sniedz pakalpojumam vai savienotājam iespēju personificēt lietotāju, lai pabeigtu papildu autentifikācijas izaicinājumus no lietojumprogrammas. Papildinformāciju skatiet rakstā [Vienotās pierakstīšanās konfigurēšana lietojumprogrammas starpniekservera lietojumprogrammā.](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to)
3. Izmantojiet [šo rakstu,](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) lai novērstu biežāk sastopamās problēmas, ar ko saskaras lietotāji, veidojot jaunu lietojumprogrammu starpniekservera lietojumprogrammu.
4. Ja rodas problēmas, iestatot aizmugurgala autentifikāciju savā lietojumprogrammā, iespējams, ir jāatrisina [Kerberos](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) ierobežoto deleģēšanas konfigurāciju lietojumprogrammas starpniekserverī vai jāseko norādījumiem par lietojumprogrammas konfigurēšanu ar [PingAccess,](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) lai novērstu savu problēmu.
