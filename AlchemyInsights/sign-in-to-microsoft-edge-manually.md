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
# <a name="sign-in-to-microsoft-edge-manually"></a><span data-ttu-id="60ab6-102">Manuāla pierakstīšanās programmā Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="60ab6-102">Sign in to Microsoft Edge manually</span></span>

<span data-ttu-id="60ab6-103">Ja lietotājs netiek automātiski pierakstījies pirmās palaišanas laikā, lietotājs var manuāli pierakstīties pārlūkprogrammas iestatījumos vai identitātes izlidošanas logā.</span><span class="sxs-lookup"><span data-stu-id="60ab6-103">If a user isn't automatically signed in during a first-run experience, the user can manually sign in through the browser's settings or the identity flyout.</span></span> <span data-ttu-id="60ab6-104">Lai pārvaldītu pierakstī-ties, izmantojiet šādas politikas:</span><span class="sxs-lookup"><span data-stu-id="60ab6-104">To manage sign-in, use the following policies:</span></span>

1. <span data-ttu-id="60ab6-105">[Nav noņemamsProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) — lai nodrošinātu, ka lietotājam vienmēr ir darba profils programmā Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="60ab6-105">[NonRemovableProfileEnabled](https://docs.microsoft.com/deployedge/microsoft-edge-policies#nonremovableprofileenabled) - To ensure that a user always has a work profile in Microsoft Edge.</span></span>
2. <span data-ttu-id="60ab6-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) — lai ierobežotu pierakstīšanos uzticamu kontu kopā.</span><span class="sxs-lookup"><span data-stu-id="60ab6-106">[RestrictSigninToPattern](https://docs.microsoft.com/deployedge/microsoft-edge-policies#restrictsignintopattern) - To restrict sign-in to a set of trusted accounts.</span></span>
3. <span data-ttu-id="60ab6-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) — lai atspējotu pierakstīšanos vai liktu lietotājiem pierakstīties.</span><span class="sxs-lookup"><span data-stu-id="60ab6-107">[BrowserSignin](https://docs.microsoft.com/deployedge/microsoft-edge-policies#browsersignin) - To disable sign-in or to force users to sign in.</span></span>

