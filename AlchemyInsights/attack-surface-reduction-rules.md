---
title: Uzbrukumu trūkšanas samazināšanas kārtulas
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
- "11228"
- "9005470"
ms.openlocfilehash: 99feaa5c3f35a0bb78b99f47ac2be88cf3e1b62a
ms.sourcegitcommit: 4b504650e11adb9894c37b6d8608b53f9d5fc13d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/25/2021
ms.locfileid: "52676435"
---
# <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c0cfc-102">Uzbrukumu trūkšanas samazināšanas kārtulas</span><span class="sxs-lookup"><span data-stu-id="c0cfc-102">Attack surface reduction rules</span></span>

<span data-ttu-id="c0cfc-103">Izslēdzot failus vai mapes, var ievērojami samazināt uzbrukumu virsmas samazināšanas kārtulu nodrošināto aizsardzību.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-103">Excluding files or folders can severely reduce the protection provided by attack surface reduction rules.</span></span> <span data-ttu-id="c0cfc-104">Failus, kurus kārtula būtu bloķējusi, ir atļauts palaist, un atskaite vai notikums netiek ierakstīts.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-104">Files that would have been blocked by a rule are allowed to run, and no report or event is recorded.</span></span> <span data-ttu-id="c0cfc-105">Izņēmumi attiecas uz visām kārtulām, kas atļauj izņēmumus.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-105">An exclusion applies to all rules that allow exclusions.</span></span>

<span data-ttu-id="c0cfc-106">ASR izņēmumiem ir jāizmanto tā pati sintakse, kas pretvīrusu programmatūra Microsoft Defender izslēgšanai.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-106">ASR exclusions use the same syntax as Microsoft Defender Antivirus exclusions.</span></span> <span data-ttu-id="c0cfc-107">Detalizētu informāciju skatiet rakstā [Izņēmumu konfigurēšana un pārbaude, lai pretvīrusu programmatūra Microsoft Defender skenēšanu.](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="c0cfc-107">For details, see [Configure and validate exclusions for Microsoft Defender Antivirus scans](/microsoft-365/security/defender-endpoint/configure-exclusions-microsoft-defender-antivirus).</span></span> <span data-ttu-id="c0cfc-108">Lai izvairītos no problēmām, [pārskatiet biežāk sastopamās kļūdas, kas rodas, definējot izņēmumus.](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus)</span><span class="sxs-lookup"><span data-stu-id="c0cfc-108">To avoid problems, review [Common mistakes to avoid when defining exclusions](/microsoft-365/security/defender-endpoint/common-exclusion-mistakes-microsoft-defender-antivirus).</span></span>

<span data-ttu-id="c0cfc-109">Ne visas ASR kārtulas atbalsta izņēmumus.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-109">Not all ASR rules support exclusions.</span></span> <span data-ttu-id="c0cfc-110">Lai pārbaudītu, vai jūsu kārtula atbalsta izņēmumus, skatiet tabulu [Uzbrukumu trūkšanas kārtulas.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="c0cfc-110">To validate if your rule supports exclusions, see the table [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

## <a name="attack-surface-reduction-rules"></a><span data-ttu-id="c0cfc-111">Uzbrukumu trūkšanas samazināšanas kārtulas</span><span class="sxs-lookup"><span data-stu-id="c0cfc-111">Attack surface reduction rules</span></span>

<span data-ttu-id="c0cfc-112">Jūsu organizācijas uzbrukuma virsma ietver visas vietas, kur uzbrucējs var uz apdraudējumēt organizācijas ierīces vai tīklus.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-112">Your organization attack surface includes all the places where an attacker could compromise organization devices or networks.</span></span> <span data-ttu-id="c0cfc-113">Samazinot uzbrukumu virsmu, tiek aizsargātas organizācijas ierīces un tīkls, kas uzbrukumiem atstāj mazāk veidu, kā veikt uzbrukumus.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-113">Reducing your attack surface means protecting the organization devices and network, which leaves attackers with fewer ways to perform attacks.</span></span> <span data-ttu-id="c0cfc-114">Varat konfigurēt uzbrukumu surface samazināšanas kārtulas programmatūrā Microsoft Defender galapunktam.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-114">Configuring attack surface reduction rules in Microsoft Defender for Endpoint can help.</span></span>

<span data-ttu-id="c0cfc-115">Papildinformāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="c0cfc-115">For more information, see:</span></span>

- [<span data-ttu-id="c0cfc-116">Kartēt ASR kārtulas GUID uz nosaukumu</span><span class="sxs-lookup"><span data-stu-id="c0cfc-116">Map ASR rule GUID to name</span></span>](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)
- <span data-ttu-id="c0cfc-117">ASR noteikumu prasības:</span><span class="sxs-lookup"><span data-stu-id="c0cfc-117">ASR rules requirements:</span></span>
    - [<span data-ttu-id="c0cfc-118">Windows 10 Pro, versija 1709 vai jaunāka</span><span class="sxs-lookup"><span data-stu-id="c0cfc-118">Windows 10 Pro, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c0cfc-119">Windows 10 Enterprise, versija 1709 vai jaunāka</span><span class="sxs-lookup"><span data-stu-id="c0cfc-119">Windows 10 Enterprise, version 1709 or later</span></span>](/windows/whats-new/whats-new-windows-10-version-1709)
    - [<span data-ttu-id="c0cfc-120">Windows Server, versija 1803 (pusgada kanāls) vai jaunāka versija</span><span class="sxs-lookup"><span data-stu-id="c0cfc-120">Windows Server, version 1803 (Semi-Annual Channel) or later</span></span>](/windows-server/get-started/whats-new-in-windows-server-1803)

## <a name="identify-the-correct-exclusion-to-apply"></a><span data-ttu-id="c0cfc-121">Pareizas izslēgšanas identificēšana, ko vēlaties lietot</span><span class="sxs-lookup"><span data-stu-id="c0cfc-121">Identify the correct exclusion to apply</span></span>

1. <span data-ttu-id="c0cfc-122">Meklējiet eventID 1121 vai 1122 Microsoft-Windows-Windows Defender/darbības žurnālā.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-122">Look for eventID 1121 or 1122 in the Microsoft-Windows-Windows Defender/Operational log.</span></span>

1. <span data-ttu-id="c0cfc-123">Novērtējiet bloka scenāriju un kontekstu un apstipriniet, ka šo scenāriju nepieciešams atbloķēt.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-123">Evaluate the block scenario and context and confirm that this scenario needs to be unblocked.</span></span>

1. <span data-ttu-id="c0cfc-124">Notikuma detalizētās informācijas sadaļā izlasiet ceļa vērtību, kas ir vērtība, kas definē izņēmumu.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-124">Read the Path value in the event details, which is the value that defines the exclusion.</span></span>
    - <span data-ttu-id="c0cfc-125">Pēc iespējas precīzāk noteikt izņēmumus.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-125">Make the exclusion as strict as possible.</span></span>
    - <span data-ttu-id="c0cfc-126">Lietojiet aizstājējzīmi, ja nepieciešams (piemēram, aizstājiet mainīgo Lietotājs).</span><span class="sxs-lookup"><span data-stu-id="c0cfc-126">Apply a wildcard where needed (for example, replace User variable).</span></span>

1. <span data-ttu-id="c0cfc-127">Lietojiet izņēmumus atbilstoši izvietošanas vajadzībām.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-127">Apply the exclusion according to your deployment needs.</span></span> <span data-ttu-id="c0cfc-128">Detalizētu informāciju skatiet rakstā [Uzbrukuma virsmas samazināšanas kārtulu pielāgošana.](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction)</span><span class="sxs-lookup"><span data-stu-id="c0cfc-128">For details, see [Customize attack surface reduction rules](/microsoft-365/security/defender-endpoint/customize-attack-surface-reduction).</span></span>

## <a name="exclusion-is-not-honored"></a><span data-ttu-id="c0cfc-129">Izņēmumi netiek paturēti</span><span class="sxs-lookup"><span data-stu-id="c0cfc-129">Exclusion is not honored</span></span>

1. <span data-ttu-id="c0cfc-130">Nosakiet, vai kārtula atbalsta izņēmumus.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-130">Determine whether the rule support exclusions.</span></span> <span data-ttu-id="c0cfc-131">Detalizētu informāciju skatiet rakstā [Uzbrukuma virsmas samazināšanas kārtulas.](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules)</span><span class="sxs-lookup"><span data-stu-id="c0cfc-131">For details, see [Attack surface reduction rules](/microsoft-365/security/defender-endpoint/attack-surface-reduction#attack-surface-reduction-rules).</span></span>

1. <span data-ttu-id="c0cfc-132">Pārskatiet lietotos izņēmumus un pārbaudiet, vai ir ievadīti drukas kļūdu vai nepareizi interpretētu aizstājējzīmju dati.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-132">Review the exclusions applied and verify with the event data for typos or misinterpreted wildcards.</span></span> <span data-ttu-id="c0cfc-133">Papildinformāciju skatiet rakstā [Atbalstītie izņēmumu tipi.](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span><span class="sxs-lookup"><span data-stu-id="c0cfc-133">For more info, see [Supported exclusion types](/microsoft-365/security/defender-endpoint/mac-exclusions#supported-exclusion-types)</span></span>

1. <span data-ttu-id="c0cfc-134">ja kārtulas ietekme ir pārāk augsta, apsveriet iespēju pārvietot kārtulu (atpakaļ) uz audita režīmu, lai veiktu papildu validāciju.</span><span class="sxs-lookup"><span data-stu-id="c0cfc-134">if the impact of the rule it too high, consider moving the rule (back) to Audit mode to perform further validation.</span></span> <span data-ttu-id="c0cfc-135">Detalizētu informāciju skatiet rakstā [Pārbaudiet, kā Microsoft Defender galapunkta līdzekļiem darbojas audita režīmā.](/microsoft-365/security/defender-endpoint/audit-windows-defender)</span><span class="sxs-lookup"><span data-stu-id="c0cfc-135">For details, see [Test how Microsoft Defender for Endpoint features work in audit mode](/microsoft-365/security/defender-endpoint/audit-windows-defender).</span></span>

1. <span data-ttu-id="c0cfc-136">Apkopojiet atbalsta datus, lai atvērtu atbalsta gadījumu, izmantojot šo komandu:</span><span class="sxs-lookup"><span data-stu-id="c0cfc-136">Collect support data to open a support case by using this command:</span></span>
    
   <span data-ttu-id="c0cfc-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span><span class="sxs-lookup"><span data-stu-id="c0cfc-137">\*\* MDEClientAnalyzer.cmd -v\*\*</span></span>

    <span data-ttu-id="c0cfc-138">Lai iegūtu papildinformāciju, skatiet rakstu Ar datoru [sēšanu saistītie jautājumi līdz programmatūrai Microsoft Defender galapunktiem.](issues-with-onboarding-machines.md)</span><span class="sxs-lookup"><span data-stu-id="c0cfc-138">For more information, see [Issues with onboarding machines to Microsoft Defender for Endpoints](issues-with-onboarding-machines.md).</span></span>
