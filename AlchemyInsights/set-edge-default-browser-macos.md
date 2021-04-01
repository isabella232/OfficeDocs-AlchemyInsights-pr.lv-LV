---
title: Microsoft Edge iestatīšana par noklusējuma pārlūkprogrammu macOS ierīcē
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 03/29/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "10362"
- "9006005"
ms.openlocfilehash: 5318c7d20ee7091e162e566cd2b4ebf5d255915b
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/30/2021
ms.locfileid: "51491557"
---
# <a name="set-microsoft-edge-as-the-default-browser-on-a-macos-device"></a><span data-ttu-id="21e46-102">Microsoft Edge iestatīšana par noklusējuma pārlūkprogrammu macOS ierīcē</span><span class="sxs-lookup"><span data-stu-id="21e46-102">Set Microsoft Edge as the default browser on a macOS device</span></span>

<span data-ttu-id="21e46-103">Izmantojiet vienu no šīm divām metodēm, lai iestatītu Microsoft Edge kā noklusējuma pārlūkprogrammu.</span><span class="sxs-lookup"><span data-stu-id="21e46-103">Use one of these two methods to set Microsoft Edge as the default browser:</span></span>

<span data-ttu-id="21e46-104">1. metode. Mirgo ierīce ar macOS attēlu, kurā Microsoft Edge jau ir iestatīta kā noklusējuma pārlūkprogramma.</span><span class="sxs-lookup"><span data-stu-id="21e46-104">Method 1: Flash the device with an image of macOS where Microsoft Edge has already been set as the default browser.</span></span>

<span data-ttu-id="21e46-105">2. metode. Iestatiet politiku DefaultBrowserSettingEnabled, lai piedāvātu lietotājam iestatīt Microsoft Edge kā noklusējuma pārlūkprogrammu.</span><span class="sxs-lookup"><span data-stu-id="21e46-105">Method 2: Set the DefaultBrowserSettingEnabled policy to prompt the user to set Microsoft Edge as the default browser.</span></span>

<span data-ttu-id="21e46-106">Jebkura no metodēm sniedz lietotājam iespēju mainīt noklusējuma pārlūkprogrammu.</span><span class="sxs-lookup"><span data-stu-id="21e46-106">Either method allows a user to change the default browser.</span></span> <span data-ttu-id="21e46-107">Šī iemesla dēļ mēs iesakām izvietot politiku DefaultBrowserSettingEnabled pat tad, ja izmantojat 1. metodi.</span><span class="sxs-lookup"><span data-stu-id="21e46-107">For this reason, we recommend that you deploy the DefaultBrowserSettingEnabled policy even if you used method 1.</span></span> <span data-ttu-id="21e46-108">Ja lietotājs maina noklusējuma pārlūkprogrammu pēc politikas izvietošanas, politika aicina lietotāju iestatīt noklusējuma pārlūkprogrammu atpakaļ uz Microsoft Edge.</span><span class="sxs-lookup"><span data-stu-id="21e46-108">If a user changes the default browser after the policy is deployed, the policy prompts the user to set the default browser back to Microsoft Edge.</span></span>
