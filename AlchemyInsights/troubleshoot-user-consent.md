---
title: Lietotāja piekrišanas problēmu novēršana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/18/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004353"
- "7785"
ms.openlocfilehash: db784c133fec554604ad09f5b27941879d97ff238f926ff6338d0f3b7c3c4105
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007905"
---
# <a name="troubleshoot-user-consent"></a>Lietotāja piekrišanas problēmu novēršana

1. Varat konfigurēt lietotāju piekrišanu lietojumprogrammām, izmantojot Azure Portal vai PowerShell. [Papildinformāciju skatiet rakstā Lietotāja](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) piekrišanas iestatījumi.
1. Administrators var arī izmantot [Microsoft Graph API,](https://docs.microsoft.com/azure/active-directory/manage-apps/configure-user-consent?tabs=azure-portal#user-consent-settings) lai piešķirtu piekrišanu deleģētām atļaujām atsevišķa lietotāja vārdā. Lai iegūtu papildinformāciju, [skatiet rakstu Piekļuves iegūste lietotāja vārdā.](https://docs.microsoft.com/graph/auth-v2-user)
1. [Lietotāja piekrišanas](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)kļūdas: šajā rakstā ir aplūkotas kļūdas, kas var rasties, kad lietotājs piekrīt lietojumprogrammai. Ja novērst neparedzētas piekrišanas uzvednes, kurās nav kļūdu ziņojumu, skatiet rakstu [Azure AD autentifikācijas scenāriji.](https://docs.microsoft.com/azure/active-directory/manage-apps/application-sign-in-unexpected-user-consent-error)