---
title: Radās kļūda, validējot piekļuves pilnvaru kļūdu desktop Analytics lietošanas laikā
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2536"
- "9000657"
ms.openlocfilehash: 12e5906ba8cbc76ba1fd99dde1cf76396c3a6942
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51813695"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Darbvirsmas analīzes instalēšanas laikā radās kļūda "Validējot piekļuves pilnvaru".

Šī kļūda parasti tiek novērota, kad beidzas autentifikācijas pilnvaras derīgums. Parasti lapas atsvaidzināšana atsvaidzina pilnvaru. Tomēr šī problēma var saglabāties, ja pastāv nosacījum piekļuves politikas, kas tiek lietotas kontam, kas tiek izmantots darbvirsmas analītikai. Varat pārskatīt Azure AD pierakstīšanās žurnālus Azure portālā, lai uzzinātu, vai nav pieteikšanās kļūmju kontā, kas tiek izmantots Desktop Analytics pievienošanai.

Lai iegūtu papildinformāciju par nosacījum piekļuvi, apmeklējiet [vietni Nosacījum piekļuves izvietošanas plānošana.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)