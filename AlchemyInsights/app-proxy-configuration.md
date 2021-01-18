---
title: Lietojumprogrammas starpniekservera konfigurācija
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
ms.openlocfilehash: 0b782705afa8eab338687590baff90de4e17ccb9
ms.sourcegitcommit: 83fe2a8d060794fdf58445b469b30a3294b7a9b6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2021
ms.locfileid: "49885136"
---
# <a name="app-proxy-configuration"></a>Lietojumprogrammas starpniekservera konfigurācija

1. Lai izprastu, kā konfigurēt lietojumprogrammas starpniekservera lietojumprogrammu Azure AD, lai lokālās lietojumprogrammas atklātu mākonī, skatiet rakstu [kā konfigurēt lietojumprogrammas starpniekservera lietojumprogrammu](https://docs.microsoft.com/azure/active-directory/application-proxy-config-how-to).
2. Vienotā pierakstīšanās (SSO) ļauj lietotājiem piekļūt lietojumprogrammai, neveicot autentificēšanas vairākas reizes. Tas ļauj vienai autentifikācijai notikt mākonī, izmantojot Azure Active Directory, un ļauj pakalpojumam vai savienotājam personificēt lietotāju, lai pabeigtu jebkādas papildu autentifikācijas problēmas no lietojumprogrammas. Papildinformāciju skatiet rakstā [vienotās pierakstīšanās konfigurācija lietojumprogrammas starpniekservera lietojumprogrammai](https://docs.microsoft.com/azure/active-directory/application-proxy-config-sso-how-to).
3. Izmantojiet [šo rakstu](https://docs.microsoft.com/azure/active-directory/application-proxy-config-problem) , lai novērstu bieži sastopamas problēmas, ar kurām saskaras lietotāji, veidojot jaunu lietojumprogrammas starpniekservera lietojumprogrammu.
4. Ja rodas problēmas, iestatot servera autentifikācijas autentifikāciju savā lietojumprogrammā, iespējams, ir [jānovērš Kerberos ierobežotās deleģēšanas konfigurācijas lietojumprogrammas starpniekserverim](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-kerberos-constrained-delegation-how-to) vai jāievēro norādījumi par [lietojumprogrammas konfigurēšanu ar PingAccess](https://docs.microsoft.com/azure/active-directory/application-proxy-back-end-ping-access-how-to) , lai atrisinātu problēmu.
