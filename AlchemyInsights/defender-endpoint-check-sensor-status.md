---
title: Defender galapunktu pārbaudes sensora statuss
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 05/21/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11084"
- "9003537"
ms.openlocfilehash: a53a0109c3b974806d04135dd2c102de81ec560f
ms.sourcegitcommit: ded29f44e5019b1929218b02733b390899843680
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/24/2021
ms.locfileid: "52676344"
---
# <a name="defender-endpoint-check-sensor-status"></a><span data-ttu-id="e53a3-102">Defender galapunktu pārbaudes sensora statuss</span><span class="sxs-lookup"><span data-stu-id="e53a3-102">Defender Endpoint check sensor status</span></span>

<span data-ttu-id="e53a3-103">Elements **Ierīces ar sensora** problēmām atrodas informācijas panelī Drošības operācijas.</span><span class="sxs-lookup"><span data-stu-id="e53a3-103">The **Devices with sensor issues** tile is located on the Security Operations dashboard.</span></span> <span data-ttu-id="e53a3-104">Šis elements sniedz informāciju par atsevišķas ierīces iespēju nodrošināt sensora datus un sazināties ar Defender galapunktu pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="e53a3-104">This tile provides information on the individual device’s ability to provide sensor data and communicate with the Defender for Endpoint service.</span></span> <span data-ttu-id="e53a3-105">Tā ziņo, cik ierīcēm jāpievērš uzmanība un palīdz noteikt problemātiskās ierīces un rīkoties, lai novērstu zināmās problēmas.</span><span class="sxs-lookup"><span data-stu-id="e53a3-105">It reports how many devices require attention and helps you identify problematic devices and take action to correct known issues.</span></span>

<span data-ttu-id="e53a3-106">Divi statusa indikatori elementā sniedz informāciju par to ierīču skaitu, par kuru nav pareizi ziņots pakalpojumam:</span><span class="sxs-lookup"><span data-stu-id="e53a3-106">Two status indicators on the tile provide information on the number of devices not reporting properly to the service:</span></span>

- <span data-ttu-id="e53a3-107">**Nepareizi konfigurēts** Ierīces, kas var daļēji būt atskaišu sensora dati pakalpojumam Defender for Endpoint, un kurās var būt konfigurācijas kļūdas, kas ir jāizlabo.</span><span class="sxs-lookup"><span data-stu-id="e53a3-107">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service and might have configuration errors that need to be corrected.</span></span>
- <span data-ttu-id="e53a3-108">**Inactive** Ierīces, kuras pēdējā mēnesī ir pārtraukuši atskaišu rādīšanu pakalpojumam Defender for Endpoint vairāk nekā septiņas dienas.</span><span class="sxs-lookup"><span data-stu-id="e53a3-108">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service for more than seven days in the past month.</span></span>

<span data-ttu-id="e53a3-109">Noklikšķinot uz jebkuras grupas, tiks iet novirzīts uz sarakstu Ierīces, kas filtrēts atbilstoši jūsu izvēlei.</span><span class="sxs-lookup"><span data-stu-id="e53a3-109">Clicking any of the groups directs you to Devices list, filtered according to your choices.</span></span> <span data-ttu-id="e53a3-110">Sarakstā Ierīces varat filtrēt darbspējas stāvokļa sarakstu pēc šāda statusa:</span><span class="sxs-lookup"><span data-stu-id="e53a3-110">On the Devices list, you can filter the health state list by the following status:</span></span>

- <span data-ttu-id="e53a3-111">**Aktīvs** Ierīces, kas aktīvi ziņo Par pakalpojumu Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="e53a3-111">**Active** Devices that are actively reporting to the Defender for Endpoint service.</span></span>
- <span data-ttu-id="e53a3-112">**Nepareizi konfigurēts** Ierīces, kas var daļēji būt atskaišu sensora dati Defender galapunktu pakalpojumam, bet kurās ir konfigurācijas kļūdas, kas ir jāizlabo.</span><span class="sxs-lookup"><span data-stu-id="e53a3-112">**Misconfigured** Devices that might partially be reporting sensor data to the Defender for Endpoint service but have configuration errors that need to be corrected.</span></span> <span data-ttu-id="e53a3-113">Nepareizi konfigurētām ierīcēm var būt viena vai vairākas tālāk minētās problēmas.</span><span class="sxs-lookup"><span data-stu-id="e53a3-113">Misconfigured devices can have either one or a combination of the following issues:</span></span>

    - <span data-ttu-id="e53a3-114">Bez sensora datiem — ierīces apturēs sensora datu sūtīšanu.</span><span class="sxs-lookup"><span data-stu-id="e53a3-114">No sensor data - Devices has stopped sending sensor data.</span></span> <span data-ttu-id="e53a3-115">No ierīces var tikt aktivizēti ierobežoti brīdinājumi.</span><span class="sxs-lookup"><span data-stu-id="e53a3-115">Limited alerts can be triggered from the device.</span></span>
    - <span data-ttu-id="e53a3-116">Sakaru traucējumi — spējām sazināties ar ierīci ir traucējumi.</span><span class="sxs-lookup"><span data-stu-id="e53a3-116">Impaired communications - Ability to communicate with device is impaired.</span></span> <span data-ttu-id="e53a3-117">Failu sūtīšana padziļinātai analīzei, failu bloķēšanai, ierīču izbrīvošana no tīkla un citas darbības, kam nepieciešama saziņa ar ierīci, var nedarboties.</span><span class="sxs-lookup"><span data-stu-id="e53a3-117">Sending files for deep analysis, blocking files, isolating device from network and other actions that require communication with the device may not work.</span></span>
- <span data-ttu-id="e53a3-118">**Inactive** Ierīces, kuras pārtrauca atskaišu rādīšanu pakalpojumam Defender for Endpoint.</span><span class="sxs-lookup"><span data-stu-id="e53a3-118">**Inactive** Devices that have stopped reporting to the Defender for Endpoint service.</span></span>

<span data-ttu-id="e53a3-119">Varat lejupielādēt visu sarakstu CSV formātā, izmantojot eksportēšanas līdzekli.</span><span class="sxs-lookup"><span data-stu-id="e53a3-119">You can download the entire list in CSV format using the Export feature.</span></span>

<span data-ttu-id="e53a3-120">Papildinformāciju skatiet rakstā [Sensora darbspējas stāvokļa pārbaude programmatūrā Microsoft Defender galapunktam](/microsoft-365/security/defender-endpoint/check-sensor-status).</span><span class="sxs-lookup"><span data-stu-id="e53a3-120">For more information, see [Check sensor health state in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/check-sensor-status).</span></span>

<span data-ttu-id="e53a3-121">Papildinformāciju par to, kas izraisīja ierīces neaktīvu vai nepareizi konfigurētu, skatiet rakstā Neaktīviem sensoriem labošana [programmatūrā Microsoft Defender galapunktam.](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors)</span><span class="sxs-lookup"><span data-stu-id="e53a3-121">For more information about what caused a device to be inactive or misconfigured, see [Fix unhealthy sensors in Microsoft Defender for Endpoint](/microsoft-365/security/defender-endpoint/fix-unhealthy-sensors).</span></span>
