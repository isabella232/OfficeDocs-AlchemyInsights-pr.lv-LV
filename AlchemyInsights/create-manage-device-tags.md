---
title: Ierīču atzīmju vai grupu izveide un pārvaldība
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11446"
- "9003537"
ms.openlocfilehash: 3a7d53beaaf830055904f0634f09a3e9e447006e
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731668"
---
# <a name="create-and-manage-device-tags-or-groups"></a><span data-ttu-id="ac3a4-102">Ierīču atzīmju vai grupu izveide un pārvaldība</span><span class="sxs-lookup"><span data-stu-id="ac3a4-102">Create and manage device tags or groups</span></span>

<span data-ttu-id="ac3a4-103">Pievienojiet atzīmes ierīcēm, lai izveidotu loģisku grupas piederības.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-103">Add tags on devices to create a logical group affiliation.</span></span> <span data-ttu-id="ac3a4-104">Ierīces tagi atbalsta pareizu tīkla kartēšanu, ļaujot pievienot dažādas atzīmes, lai tvertu kontekstu un iespējotu dinamisku sarakstu izveidi kā daļu no incidenta.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-104">Device tags support proper mapping of the network, enabling you to attach different tags to capture context and to enable dynamic list creation as part of an incident.</span></span> <span data-ttu-id="ac3a4-105">Atzīmes var izmantot kā filtru ierīču saraksta skatā vai ierīču grupēšanai.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-105">Tags can be used as a filter in Devices list view, or to group devices.</span></span> <span data-ttu-id="ac3a4-106">Papildinformāciju par ierīču grupēšanu skatiet rakstā [Ierīces atzīmju izveide un pārvaldība.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="ac3a4-106">For more information on device grouping, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>

<span data-ttu-id="ac3a4-107">Atzīmes ierīcēs varat pievienot, veicot tālākkās darbības.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-107">You can add tags on devices by:</span></span>

- <span data-ttu-id="ac3a4-108">Portāla izmantošana</span><span class="sxs-lookup"><span data-stu-id="ac3a4-108">Using the portal</span></span>

- <span data-ttu-id="ac3a4-109">Reģistra atslēgas vērtības iestatīšana</span><span class="sxs-lookup"><span data-stu-id="ac3a4-109">Setting a registry key value</span></span>
 
<span data-ttu-id="ac3a4-110">**Piezīme.** Starp laiku, kad atzīme tiek pievienota ierīcei, un tās pieejamību ierīču sarakstā un ierīces lapā var būt latentums.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-110">**Note:** There could be latency between the time a tag is added to a device and its availability in the devices list and device page.</span></span>

<span data-ttu-id="ac3a4-111">Lai pievienotu ierīces atzīmes, izmantojot API, skatiet [rakstu Ierīces atzīmju API pievienošana vai noņemšana.](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags)</span><span class="sxs-lookup"><span data-stu-id="ac3a4-111">To add device tags using API, see [Add or remove device tags API](/microsoft-365/security/defender-endpoint/add-or-remove-machine-tags).</span></span>

## <a name="add-and-manage-device-tags-using-the-portal"></a><span data-ttu-id="ac3a4-112">Ierīču atzīmju pievienošana un pārvaldība portālā</span><span class="sxs-lookup"><span data-stu-id="ac3a4-112">Add and manage device tags using the portal</span></span>

1. <span data-ttu-id="ac3a4-113">Atlasiet ierīci, kurā vēlaties pārvaldīt atzīmes.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-113">Select the device that you want to manage tags on.</span></span> <span data-ttu-id="ac3a4-114">Ierīci varat atlasīt vai meklēt jebkurā no šiem skatiem:</span><span class="sxs-lookup"><span data-stu-id="ac3a4-114">You can select or search for a device from any of the following views:</span></span>

    - <span data-ttu-id="ac3a4-115">**Drošības darbību informācijas panelis** Atlasiet ierīces nosaukumu sadaļā Populārākās ierīces ar aktīviem brīdinājumiem.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-115">**Security operations dashboard** Select the device name from the Top devices with active alerts section.</span></span>
    - <span data-ttu-id="ac3a4-116">**Brīdinājumu rinda** — atlasiet ierīces nosaukumu blakus ierīces ikonai brīdinājumu rindā.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-116">**Alerts queue** - Select the device name beside the device icon from the alerts queue.</span></span>
    - <span data-ttu-id="ac3a4-117">**Ierīču saraksts** — ierīču sarakstā atlasiet ierīces nosaukumu.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-117">**Devices list** - Select the device name from the list of devices.</span></span>
    - <span data-ttu-id="ac3a4-118">**Meklēšanas lodziņš** — nolaižamajā izvēlnē atlasiet Ierīce un ievadiet ierīces nosaukumu.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-118">**Search box** - Select Device from the drop-down menu and enter the device name.</span></span>

    <span data-ttu-id="ac3a4-119">Varat arī atvērt brīdinājuma lapu, izmantojot faila un IP skatu.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-119">You can also get to the alert page through the file and IP views.</span></span>

1. <span data-ttu-id="ac3a4-120">Rindā **Atbildes** darbības atlasiet Pārvaldīt atzīmes.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-120">Select **Manage Tags** from the row of Response actions.</span></span>

1. <span data-ttu-id="ac3a4-121">Rakstiet, lai atrastu vai izveidotu atzīmes.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-121">Type to find or create tags.</span></span>

<span data-ttu-id="ac3a4-122">Atzīmes tiek pievienotas ierīces skatam un atspoguļotas saraksta Ierīces skatā.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-122">Tags are added to the device view and are reflected on the Devices list view.</span></span> <span data-ttu-id="ac3a4-123">Pēc tam varat izmantot filtru Atzīmes, lai skatītu atbilstošo ierīču sarakstu.</span><span class="sxs-lookup"><span data-stu-id="ac3a4-123">You can then use the Tags filter to see the relevant list of devices.</span></span>

<span data-ttu-id="ac3a4-124">Papildinformāciju skatiet rakstā [Ierīces atzīmju izveide un pārvaldība.](/microsoft-365/security/defender-endpoint/machine-tags)</span><span class="sxs-lookup"><span data-stu-id="ac3a4-124">For more information, see [Create and manage device tags](/microsoft-365/security/defender-endpoint/machine-tags).</span></span>