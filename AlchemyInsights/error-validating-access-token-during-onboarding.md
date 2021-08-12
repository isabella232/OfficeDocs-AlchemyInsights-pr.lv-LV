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
ms.openlocfilehash: 1d6b840e731eaff537d8f74f9ce0af29af13bd390e701fb2835e8718b4521158
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "53946622"
---
# <a name="there-was-an-error-validating-access-token-error-during-desktop-analytics-onboarding"></a>Darbvirsmas analīzes instalēšanas laikā radās kļūda "Validējot piekļuves pilnvaru".

Šī kļūda parasti tiek novērota, kad beidzas autentifikācijas pilnvaras derīgums. Parasti lapas atsvaidzināšana atsvaidzina pilnvaru. Tomēr šī problēma var saglabāties, ja pastāv nosacījum piekļuves politikas, kas tiek lietotas kontam, kas tiek izmantots darbvirsmas analītikai. Varat pārskatīt Azure AD pierakstīšanās žurnālus Azure portālā, lai uzzinātu, vai nav pieteikšanās kļūmju kontā, kas tiek izmantots Desktop Analytics pievienošanai.

Lai iegūtu papildinformāciju par nosacījum piekļuvi, apmeklējiet [vietni Nosacījum piekļuves izvietošanas plānošana.](https://docs.microsoft.com/azure/active-directory/conditional-access/plan-conditional-access)