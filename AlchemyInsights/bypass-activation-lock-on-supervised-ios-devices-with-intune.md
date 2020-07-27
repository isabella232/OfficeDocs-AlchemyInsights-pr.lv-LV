---
title: Apiešanas aktivizēšanas bloķēšana pārraudzītās iOS ierīcēs ar Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/23/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1277"
- "6700008"
ms.openlocfilehash: 16be4e0cd2e47fe5d5888cbbe1380774f859e4d6
ms.sourcegitcommit: 07e56267dedfc4cec1143072c791670cbf81186b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/24/2020
ms.locfileid: "45424207"
---
# <a name="bypass-activation-lock-on-supervised-ios-devices-with-intune"></a><span data-ttu-id="24285-102">Apiešanas aktivizēšanas bloķēšana pārraudzītās iOS ierīcēs ar Intune</span><span class="sxs-lookup"><span data-stu-id="24285-102">Bypass activation lock on supervised iOS devices with Intune</span></span>

<span data-ttu-id="24285-103">Iespēja apiet aktivizācijas bloķēšanu iOS ierīcēs atvieglo atkopšanos no scenārija, kad lietotājs nodrošina aktivizēšanas bloķēšanu korporatīvā ierīcē un pēc tam atstāj uzņēmumu.</span><span class="sxs-lookup"><span data-stu-id="24285-103">The ability to bypass the activation lock on iOS devices makes it easier to recover from the scenario where a user enables activation lock on a corporate device, and then leaves the company.</span></span>

<span data-ttu-id="24285-104">Priekšnosacījumi aktivizācijas bloķēšanas apiešanai ir šādi:</span><span class="sxs-lookup"><span data-stu-id="24285-104">Pre-requisites to bypassing an activation lock include:</span></span>

- <span data-ttu-id="24285-105">Ierīce ir "pārraudzība".</span><span class="sxs-lookup"><span data-stu-id="24285-105">A device is that is "supervised."</span></span>
- <span data-ttu-id="24285-106">Aktivizēšanas bloķēšana ir veiksmīgi iespējota, izmantojot iOS ierīces ierobežojumu politiku Intune.</span><span class="sxs-lookup"><span data-stu-id="24285-106">The activation lock is successfully enabled using iOS Device restriction policy in Intune.</span></span>

<span data-ttu-id="24285-107">Turklāt, apejot aktivizācijas atslēgu, ir jāveic tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="24285-107">In addition, when bypassing an activation lock, you should:</span></span>

- <span data-ttu-id="24285-108">Fiziski ir jānoslauka ierīce.</span><span class="sxs-lookup"><span data-stu-id="24285-108">Physically possess the device being wiped.</span></span>
- <span data-ttu-id="24285-109">Kopējiet kodu pirms tīrīšanas izdošanas.</span><span class="sxs-lookup"><span data-stu-id="24285-109">Copy the code before you issue the wipe.</span></span>

<span data-ttu-id="24285-110">**Piezīme:** Tīrīšanas kods nav reģistrjutīgs, tāpēc "-" rakstzīmes nav vajadzīgas.</span><span class="sxs-lookup"><span data-stu-id="24285-110">**Note:** The wipe code is not case sensitive, so the "-" characters are not required.</span></span>

<span data-ttu-id="24285-111">Detalizētu informāciju skatiet rakstā [aktivizēšanas bloķēšanas apiešana Uzraudzītās iOS ierīcēs ar Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span><span class="sxs-lookup"><span data-stu-id="24285-111">For details, see [Bypass Activation Lock on Supervised iOS devices with Intune](https://docs.microsoft.com/intune/device-activation-lock-bypass).</span></span>

<span data-ttu-id="24285-112">**BUJ**</span><span class="sxs-lookup"><span data-stu-id="24285-112">**FAQ**</span></span>

<span data-ttu-id="24285-113">J: **es izdevu attālu darbību, lai noņemtu uzņēmuma datus no ierīces, un tagad tas ir iestrēdzis gaidīšanas stāvoklī.**</span><span class="sxs-lookup"><span data-stu-id="24285-113">Q: **I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.**</span></span>

<span data-ttu-id="24285-114">A: lai attāla darbība būtu sekmīga, mērķtiecīgai ierīcei jābūt tiešsaistē un veselīgai.</span><span class="sxs-lookup"><span data-stu-id="24285-114">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="24285-115">Tālāk norādītajās situācijās attālā darbība paliek gaidīšanas stāvoklī 30 dienas vai līdz brīdim, kad ierīce atpieņem komandu:</span><span class="sxs-lookup"><span data-stu-id="24285-115">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command when the device:</span></span>

- <span data-ttu-id="24285-116">Nav savienojamības.</span><span class="sxs-lookup"><span data-stu-id="24285-116">Does not have connectivity.</span></span>
- <span data-ttu-id="24285-117">Zaudē pārvaldības statusu ar Intune.</span><span class="sxs-lookup"><span data-stu-id="24285-117">Loses its management status with Intune.</span></span>

<span data-ttu-id="24285-118">Ja uzskatāt, ka ierīce vairs netiek pārbaudīta, un tā neizņems uzņēmuma datus, atlasiet Dzēst.</span><span class="sxs-lookup"><span data-stu-id="24285-118">If you think a device is no longer checking in, and that it won’t remove company data, select Delete.</span></span> <span data-ttu-id="24285-119">Dzēšot tiek noņemts ierīces ieraksts, un tas vairs netiek rādīts ierīču Intune sarakstā.</span><span class="sxs-lookup"><span data-stu-id="24285-119">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="24285-120">Lai ierīce atkal kļūtu aktīva, tās lietotājam ir atkārtoti jāpiesakās ierīcē.</span><span class="sxs-lookup"><span data-stu-id="24285-120">For the device to become active again, its user must re-enroll the device.</span></span>

<span data-ttu-id="24285-121">J: **Kāpēc noteiktas attālas darbības nav pieejamas lietošanai?**</span><span class="sxs-lookup"><span data-stu-id="24285-121">Q: **Why are certain remote actions not available for me to use?**</span></span>

<span data-ttu-id="24285-122">A: ne visas platformas atbalsta visas attālās ierīces darbības.</span><span class="sxs-lookup"><span data-stu-id="24285-122">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="24285-123">Tālāk norādītās attālās darbības ir Platform-specifiskas.</span><span class="sxs-lookup"><span data-stu-id="24285-123">The following remote actions are platform-specific.</span></span>

- <span data-ttu-id="24285-124">Apiešanas aktivizēšanas bloķēšana (tikai iOS)</span><span class="sxs-lookup"><span data-stu-id="24285-124">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="24285-125">Jauna startēšana (tikai Windows)</span><span class="sxs-lookup"><span data-stu-id="24285-125">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="24285-126">Pazaudēts režīms (tikai iOS)</span><span class="sxs-lookup"><span data-stu-id="24285-126">Lost mode (iOS only)</span></span>
- <span data-ttu-id="24285-127">Ierīces atrašana (tikai iOS)</span><span class="sxs-lookup"><span data-stu-id="24285-127">Locate device (iOS only)</span></span>
- <span data-ttu-id="24285-128">Restartēt (tikai operētājsistēmā Windows)</span><span class="sxs-lookup"><span data-stu-id="24285-128">Restart (Windows only)</span></span>

<span data-ttu-id="24285-129">Detalizētu informāciju par katru darbību skatiet rakstā [Pieejamās ierīces darbības](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="24285-129">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>