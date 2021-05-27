---
title: Indikatori nedarbojas, izmantojot pārlūkprogrammu Edge
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11230"
- "9005470"
ms.openlocfilehash: df62d965e0dc2ddb656571af99b1e4c3cb52ea35
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676459"
---
# <a name="indicators-dont-work-using-edge-browser"></a><span data-ttu-id="4a9a1-102">Indikatori nedarbojas, izmantojot pārlūkprogrammu Edge</span><span class="sxs-lookup"><span data-stu-id="4a9a1-102">Indicators don't work using Edge browser</span></span>

<span data-ttu-id="4a9a1-103">Kad esat izveidojis indikatoru, tas netiek pagodēts edge (Smartscreen).</span><span class="sxs-lookup"><span data-stu-id="4a9a1-103">After you created an Indicator, it's not honored by Edge (Smartscreen).</span></span> <span data-ttu-id="4a9a1-104">Papildinformāciju skatiet rakstā [IP un vietrāžu URL/domēnu indikatoru izveide.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="4a9a1-104">For more information, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>

## <a name="step-1-ensure-the-following"></a><span data-ttu-id="4a9a1-105">1. darbība. Pārliecinieties, vai ir:</span><span class="sxs-lookup"><span data-stu-id="4a9a1-105">Step 1: Ensure the following</span></span>

- <span data-ttu-id="4a9a1-106">Pārliecinieties, vai indikators ir pareizs (IP/URL pārrakstīšanās kļūda, pareizās RBAC grupas).</span><span class="sxs-lookup"><span data-stu-id="4a9a1-106">Verify that the indicator is correct (no typos in IP/URL, correct action, the correct RBAC groups).</span></span>
- <span data-ttu-id="4a9a1-107">Uzgaidiet minimālās 2 stundas pēc indikatora izveides, lai ņem vērā iespējamo latentumu.</span><span class="sxs-lookup"><span data-stu-id="4a9a1-107">Wait the minimum 2 hours after creating the indicator to take into account any possible latency.</span></span>
- <span data-ttu-id="4a9a1-108">Pārliecinieties, vai sistēma(s) ir pievienota(s) programmatūrai Microsoft Defender galapunktam.</span><span class="sxs-lookup"><span data-stu-id="4a9a1-108">Confirm that the system(s) are onboarded to Microsoft Defender for Endpoint.</span></span>
- <span data-ttu-id="4a9a1-109">Pārbaudiet, vai sistēma(s) var sazināties ar mākoni.</span><span class="sxs-lookup"><span data-stu-id="4a9a1-109">Verify that system(s) can communicate with the Cloud.</span></span>
- <span data-ttu-id="4a9a1-110">Pārbaudiet, vai smartscreen ir iespējots un sasniedzams, dodoties uz [testa vietni.](https://demo.smartscreen.msft.net)</span><span class="sxs-lookup"><span data-stu-id="4a9a1-110">Verify that Smartscreen is enabled and reachable by going to the [test site](https://demo.smartscreen.msft.net).</span></span>

## <a name="step-2-troubleshoot-the-potential-issue"></a><span data-ttu-id="4a9a1-111">2. darbība. Potenciālās problēmas novēršana</span><span class="sxs-lookup"><span data-stu-id="4a9a1-111">Step 2: Troubleshoot the potential issue</span></span>

- <span data-ttu-id="4a9a1-112">Pārliecinieties, vai klients atbilst prasībām.</span><span class="sxs-lookup"><span data-stu-id="4a9a1-112">Make sure the client meets the requirements.</span></span> <span data-ttu-id="4a9a1-113">Detalizētu informāciju skatiet rakstā [IP un URL/domēnu indikatoru izveide.](/microsoft-365/security/defender-endpoint/indicator-ip-domain)</span><span class="sxs-lookup"><span data-stu-id="4a9a1-113">For details, see [Create indicators for IPs and URLs/domains](/microsoft-365/security/defender-endpoint/indicator-ip-domain).</span></span>
- <span data-ttu-id="4a9a1-114">Pārliecinieties, vai izmantojat jaunāko pārlūkprogrammas Edge versiju.</span><span class="sxs-lookup"><span data-stu-id="4a9a1-114">Make sure you're running the latest version of the Edge browser.</span></span> <span data-ttu-id="4a9a1-115">Lai uzzinātu jaunāko versiju, skatiet [rakstu Uzziniet, kura Microsoft Edge jūsu versija.](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb)</span><span class="sxs-lookup"><span data-stu-id="4a9a1-115">To find out the latest version, see [Find out which version of Microsoft Edge you have](https://support.microsoft.com/microsoft-edge/find-out-which-version-of-microsoft-edge-you-have-c726bee8-c42e-e472-e954-4cf5123497eb).</span></span>
- <span data-ttu-id="4a9a1-116">Restartējiet pārlūkprogrammu Edge.</span><span class="sxs-lookup"><span data-stu-id="4a9a1-116">Restart the Edge browser.</span></span>
- <span data-ttu-id="4a9a1-117">Naviģējiet uz vietni, kurai ir iestatīts indikators.</span><span class="sxs-lookup"><span data-stu-id="4a9a1-117">Navigate to the site for which you have setup an indicator.</span></span> <span data-ttu-id="4a9a1-118">Ja vietne netiek parādīta, kā paredzēts, pārejiet pie 3. darbības.</span><span class="sxs-lookup"><span data-stu-id="4a9a1-118">If the site does not appear as expected, continue to Step 3.</span></span> 

## <a name="step-3-collect-data"></a><span data-ttu-id="4a9a1-119">3. darbība. Datu apkopošana</span><span class="sxs-lookup"><span data-stu-id="4a9a1-119">Step 3: Collect data</span></span>

- <span data-ttu-id="4a9a1-120">Apkopojiet **MDEClientAnalyzer diagnostikas** datus.</span><span class="sxs-lookup"><span data-stu-id="4a9a1-120">Collect **MDEClientAnalyzer** diagnostic data.</span></span> <span data-ttu-id="4a9a1-121">Norādījumus skatiet rakstā Ar datoru [sēšanu saistītas problēmas līdz programmatūrai Microsoft Defender galapunktam.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="4a9a1-121">For instructions, see [Issues with onboarding machines to Microsoft Defender for Endpoint](issues-with-onboarding-machines.md).</span></span>
- <span data-ttu-id="4a9a1-122">Ja esat ērti instalējis un apkopojis Fiddler izsekošanas programmu, skatiet [sadaļu Telerik Fiddler](http://www.telerik.com/fiddler).</span><span class="sxs-lookup"><span data-stu-id="4a9a1-122">If you are comfortable installing and collecting a Fiddler trace, see [Telerik Fiddler](http://www.telerik.com/fiddler).</span></span>
- <span data-ttu-id="4a9a1-123">Ja vēlaties saņemt norādījumus no Microsoft atbalsta dienesta, tālāk atlasiet ikonu Atbalsts, lai atvērtu atbalsta gadījumu.</span><span class="sxs-lookup"><span data-stu-id="4a9a1-123">If you prefer guidance from Microsoft Support, select the Support icon below to open a support case.</span></span>
