---
title: Manuāla pierakstīšanās programmā Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
ms.date: 12/03/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 686e8f18-b871-4dd2-864f-8562947ab583
ms.collection: Adm_O365
ms.custom:
- "9003844"
- "6893"
- "8332"
- "9004625"
ms.openlocfilehash: f380d09dc14788205638cdee6aebe0b084ecab2f
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398664"
---
# <a name="sign-in-to-microsoft-edge-manually"></a>Manuāla pierakstīšanās programmā Microsoft Edge

Ja lietotājs netiek automātiski pierakstījies pirmās palaišanas laikā, lietotājs var manuāli pierakstīties pārlūkprogrammas iestatījumos vai identitātes izlidošanas logā. Lai pārvaldītu pierakstī-ties, izmantojiet šādas politikas:

1. [Nav noņemamsProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) — lai nodrošinātu, ka lietotājam vienmēr ir darba profils programmā Microsoft Edge.
2. [RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) — lai ierobežotu pierakstīšanos uzticamu kontu kopā.
3. [BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) — lai atspējotu pierakstīšanos vai liktu lietotājiem pierakstīties.

