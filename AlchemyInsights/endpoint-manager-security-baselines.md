---
title: EndPoint pārvaldnieks — drošības bāzes rādītāji
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
- "10084"
- "6700005"
ms.openlocfilehash: d2a063fdc4929cbee5fef71bfb47ace8f2ba458f
ms.sourcegitcommit: 430d247cb5dd5dc5d1f82d977456558dfd514277
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51421083"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="63b39-102">EndPoint pārvaldnieks — drošības bāzes rādītāji</span><span class="sxs-lookup"><span data-stu-id="63b39-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="63b39-103">Drošības bāzes datu bāzes ir iepriekš konfigurētas Windows iestatījumu grupas, kas palīdz lietot atbilstošo drošības grupu ieteiktos drošības iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="63b39-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="63b39-104">Šos bāzes datu laukus var pielāgot, lai nodrošinātu tikai vajadzīgos iestatījumus un vērtības.</span><span class="sxs-lookup"><span data-stu-id="63b39-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="63b39-105">Papildinformāciju par drošības bāzes datu bāzes datu skatiet rakstā Drošības bāzes datu [izmantošana Windows 10 ierīču konfigurēšanai intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="63b39-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="63b39-106">Šiem produktiem pašlaik ir pieejami bāzes dati:</span><span class="sxs-lookup"><span data-stu-id="63b39-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="63b39-107">Windows MDM drošības iestatījumi</span><span class="sxs-lookup"><span data-stu-id="63b39-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="63b39-108">Microsoft Defender lietotājam EndPoint drošība</span><span class="sxs-lookup"><span data-stu-id="63b39-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="63b39-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="63b39-109">Microsoft Edge</span></span>

<span data-ttu-id="63b39-110">Katrs bāzes datu objekts tiek periodiski atjaunināts un izlaists inkrementālajās versijās.</span><span class="sxs-lookup"><span data-stu-id="63b39-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="63b39-111">Katra versija pievieno un vai noņem iestatījumus no iepriekšējās versijas, lai nodrošinātu, ka bāzes datus atbilst pašreizējiem norādījumiem.</span><span class="sxs-lookup"><span data-stu-id="63b39-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="63b39-112">Galapunkta drošības drošības konsolē var salīdzināt dažādas versijas, tādējādi kļūstot redzamas izmaiņas no versijas uz versiju.</span><span class="sxs-lookup"><span data-stu-id="63b39-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="63b39-113">Norādījumus par to, kā efektīvāk mainīt bāzes datu versiju, skatiet rakstā Drošības bāzlīniju profilu pārvaldība [programmā Microsoft Intune.](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure)</span><span class="sxs-lookup"><span data-stu-id="63b39-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="63b39-114">Pēc drošības bāzes datu izvietošanas varat pārraudzīt izvietošanas stāvokli un pārskatīt iestatījumus pa ierīcēm.</span><span class="sxs-lookup"><span data-stu-id="63b39-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="63b39-115">**Piezīme.** Var paiet līdz pat 24 stundām, līdz bāzes datu atskaites dati tiek parādīti no sākotnējās izvietošanas ierīcē, un var būt nepieciešamas līdz pat 6 stundām, lai iegūtu atjauninājumus.</span><span class="sxs-lookup"><span data-stu-id="63b39-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="63b39-116">Visbiežākais bāzlīniju iestatījuma cēlonis, kas netiek lietots, ir tas pats iestatījums, kas tiek izmantots citā profilā.</span><span class="sxs-lookup"><span data-stu-id="63b39-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="63b39-117">Šo scenāriju var izpētīt konkrētām ierīcēm, atlasot šo ierīci profila Drošības bāzlīnija mezglā Ierīces statuss.</span><span class="sxs-lookup"><span data-stu-id="63b39-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="63b39-118">Detalizētu informāciju skatiet rakstā [Drošības bāzes datu konfliktu atrise.](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines)</span><span class="sxs-lookup"><span data-stu-id="63b39-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>