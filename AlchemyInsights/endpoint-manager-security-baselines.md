---
title: EndPoint Manager — drošības bāzes
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
- "10064"
- "9003771"
ms.openlocfilehash: 36b480c7ed4715338fda056eafd69c511093e627
ms.sourcegitcommit: bef118c00aa397cd6d8941d403fe9cfa49dd8c73
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/30/2021
ms.locfileid: "51440891"
---
# <a name="endpoint-manager---security-baselines"></a><span data-ttu-id="c6907-102">EndPoint Manager — drošības bāzes</span><span class="sxs-lookup"><span data-stu-id="c6907-102">EndPoint Manager - Security baselines</span></span>

<span data-ttu-id="c6907-103">Drošības bāzes ir iepriekš konfigurētas Windows iestatījumu grupas, kas palīdz lietot atbilstošo drošības grupu ieteiktos drošības iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="c6907-103">Security baselines are pre-configured groups of Windows settings that help you apply the security settings recommended by the relevant security teams.</span></span> <span data-ttu-id="c6907-104">Šīs bāzes var pielāgot, lai nodrošinātu tikai vajadzīgos iestatījumus un vērtības.</span><span class="sxs-lookup"><span data-stu-id="c6907-104">These baselines can be customized to deliver only the settings and values desired.</span></span> <span data-ttu-id="c6907-105">Papildinformāciju par drošības bāzēm skatiet rakstā [Drošības bāžu izmantošana, lai konfigurētu Windows 10 ierīces Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span><span class="sxs-lookup"><span data-stu-id="c6907-105">For more information about security baselines, see [Use security baselines to configure Windows 10 devices in Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines).</span></span>

<span data-ttu-id="c6907-106">Pašlaik ir pieejamas bāzes šiem produktiem:</span><span class="sxs-lookup"><span data-stu-id="c6907-106">There are currently baselines for these products:</span></span>

- <span data-ttu-id="c6907-107">Windows MDM drošības iestatījumi</span><span class="sxs-lookup"><span data-stu-id="c6907-107">Windows MDM Security settings</span></span>
- <span data-ttu-id="c6907-108">Microsoft Defender galapunkta aizsardzībai</span><span class="sxs-lookup"><span data-stu-id="c6907-108">Microsoft Defender for EndPoint Security</span></span>
- <span data-ttu-id="c6907-109">Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="c6907-109">Microsoft Edge</span></span>

<span data-ttu-id="c6907-110">Katra bāze tiek periodiski atjaunināta un izlaista inkrementālās versijās.</span><span class="sxs-lookup"><span data-stu-id="c6907-110">Each of the baselines are updated periodically and released in incremental versions.</span></span> <span data-ttu-id="c6907-111">Katrā versijā tiek pievienoto vai noņemti iestatījumi no iepriekšējās versijas, lai nodrošinātu, ka bāze atbilst pašreizējiem norādījumiem.</span><span class="sxs-lookup"><span data-stu-id="c6907-111">Each version adds and or removes settings from the previous version to ensure that the baseline meets current guidance.</span></span> <span data-ttu-id="c6907-112">Drošības bāzes konsole Endpoint Security ļauj salīdzināt dažādas versijas, padarot redzamas izmaiņas no versijas uz versiju.</span><span class="sxs-lookup"><span data-stu-id="c6907-112">The Security baselines console in Endpoint Security allows different versions to be compared by making the changes from version to version visible.</span></span>

<span data-ttu-id="c6907-113">Norādījumus par to, kā efektīvāk mainīt to, kāda bāzes versija tiek izvietota, skatiet rakstā [Drošības bāzu profilu pārvaldība Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span><span class="sxs-lookup"><span data-stu-id="c6907-113">For guidance on how to most effectively change which version of baseline is deployed, see [Manage security baseline profiles in Microsoft Intune](https://docs.microsoft.com/mem/intune/protect/security-baselines-configure).</span></span>

<span data-ttu-id="c6907-114">Pēc drošības bāzes izvietošanas varat pārraudzīt izvietošanas stāvokli un pārskatīt iestatījumus katru ierīci atsevišķi.</span><span class="sxs-lookup"><span data-stu-id="c6907-114">After deploying a security baseline, you can monitor the state of deployment and review settings on a device-by-device basis.</span></span>

<span data-ttu-id="c6907-115">**Piezīme.** Bāzu atskaišu datu parādīšana var ilgt līdz pat 24 stundām no sākotnējās izvietošanas ierīcē un līdz pat 6 stundām papildu atjauninājumiem.</span><span class="sxs-lookup"><span data-stu-id="c6907-115">**Note:** The reporting data for baselines may take up to 24 hours to appear from the initial deployment to a device and up to 6 hours for further updates.</span></span> 

<span data-ttu-id="c6907-116">Visbiežāk bāzes iestatījums netiek lietots tāpēc, ka tāds pats iestatījums tiek izmantots citā profilā.</span><span class="sxs-lookup"><span data-stu-id="c6907-116">The most common cause of a baseline setting not applying is because the same setting being used in a different profile.</span></span> <span data-ttu-id="c6907-117">Šo scenāriju var izpētīt konkrētām ierīcēm, atlasot šo ierīci profila Drošības bāzes datu mezglā Ierīces statuss.</span><span class="sxs-lookup"><span data-stu-id="c6907-117">This scenario can be investigated for specific device by selecting that device from within the Device Status node of the Security Baseline profile.</span></span> <span data-ttu-id="c6907-118">Detalizētu informāciju skatiet rakstā [Konfliktu atrisināšana drošības bāzēm](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span><span class="sxs-lookup"><span data-stu-id="c6907-118">For details, see [Resolve conflicts for security baselines](https://docs.microsoft.com/mem/intune/protect/security-baselines-monitor#resolve-conflicts-for-security-baselines).</span></span>