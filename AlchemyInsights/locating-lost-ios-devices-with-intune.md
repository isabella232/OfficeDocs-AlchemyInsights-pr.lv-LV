---
title: Pazudušu iOS ierīču atrašana ar Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1283"
- "6700008"
ms.openlocfilehash: faaea65c7edc345bb676d2fb266e20f85ba2cbe5
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439629"
---
# <a name="locating-lost-ios-devices-with-intune"></a><span data-ttu-id="1c328-102">Pazudušu iOS ierīču atrašana ar Intune</span><span class="sxs-lookup"><span data-stu-id="1c328-102">Locating lost iOS devices with Intune</span></span>

<span data-ttu-id="1c328-103">Ja iespējojat pazaudētu režīmu iOS ierīcē, administratoram ir parādīts ziņojums un kontaktpersonas tālruņa numurs bloķēšanas ekrānā.</span><span class="sxs-lookup"><span data-stu-id="1c328-103">Enabling lost mode on an iOS device allows an administrator to have a message and contact phone number displayed on the lock screen.</span></span>

<span data-ttu-id="1c328-104">Pēc tam, kad ir iespējots pazaudēts režīms, administrators var izmantot darbību atrast ierīci, lai noteiktu ierīces fizisko atrašanās vietu.</span><span class="sxs-lookup"><span data-stu-id="1c328-104">After lost mode is enabled the admin can use the Locate device action to identify the physical location of the device.</span></span>

<span data-ttu-id="1c328-105">Opcija atrast ierīces darbību Intune darbojas ar iOS ierīcēm, lai kartē rādītu noteiktas ierīces atrašanās vietu.</span><span class="sxs-lookup"><span data-stu-id="1c328-105">The Locate device action in Intune works with iOS devices to show the location of a specific device on a map.</span></span>

<span data-ttu-id="1c328-106">Šīs darbības veikšanai nepieciešama iOS ierīces lietošana:</span><span class="sxs-lookup"><span data-stu-id="1c328-106">Using this action requires the iOS device to be in:</span></span>

- <span data-ttu-id="1c328-107">Pārraudzīts režīms</span><span class="sxs-lookup"><span data-stu-id="1c328-107">Supervised mode</span></span>
- <span data-ttu-id="1c328-108">Zaudētais režīms</span><span class="sxs-lookup"><span data-stu-id="1c328-108">Lost mode</span></span>

<span data-ttu-id="1c328-109">Papildinformāciju skatiet rakstā [pazaudēta režīma iespējošana iOS/iPadOS ierīcēs ar Intune](https://docs.microsoft.com/intune/device-lost-mode) un [atrodiet pazudušas vai nozagtas iOS/IPadOS ierīces ar Intune](https://docs.microsoft.com/intune/device-locate).</span><span class="sxs-lookup"><span data-stu-id="1c328-109">For more info, see [Enable lost mode on iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-lost-mode) and [Locate lost or stolen iOS/iPadOS devices with Intune](https://docs.microsoft.com/intune/device-locate).</span></span>

<span data-ttu-id="1c328-110">**BUJ**</span><span class="sxs-lookup"><span data-stu-id="1c328-110">**FAQ**</span></span>

<span data-ttu-id="1c328-111">J: es izdevu attālu darbību, lai noņemtu uzņēmuma datus no ierīces, un tagad tas ir iestrēdzis gaidīšanas stāvoklī.</span><span class="sxs-lookup"><span data-stu-id="1c328-111">Q: I issued a remote action to remove company data from a device, and now it’s stuck in a pending state.</span></span>

<span data-ttu-id="1c328-112">A: lai attāla darbība būtu sekmīga, mērķtiecīgai ierīcei jābūt tiešsaistē un veselīgai.</span><span class="sxs-lookup"><span data-stu-id="1c328-112">A: For a remote action to successfully complete, the targeted device must be online and healthy.</span></span> <span data-ttu-id="1c328-113">Tālāk norādītajās situācijās attālā darbība paliek gaidīšanas stāvoklī 30 dienas vai līdz brīdim, kad ierīce atpieņem komandu:</span><span class="sxs-lookup"><span data-stu-id="1c328-113">In the following situations, the remote action stays in a pending state for 30 days, or until the device acknowledges the command:</span></span>

- <span data-ttu-id="1c328-114">Ja ierīcei nav savienojamības</span><span class="sxs-lookup"><span data-stu-id="1c328-114">When the device does not have connectivity</span></span>
- <span data-ttu-id="1c328-115">Kad ierīce zaudē pārvaldības statusu ar Intune</span><span class="sxs-lookup"><span data-stu-id="1c328-115">When the device loses its management status with Intune</span></span>

<span data-ttu-id="1c328-116">Ja uzskatāt, ka ierīce vairs netiek pārbaudīta un nevarēs noņemt uzņēmuma datus, atlasiet Dzēst.</span><span class="sxs-lookup"><span data-stu-id="1c328-116">If you think a device is no longer checking in, and that it won’t be able to remove company data, select Delete.</span></span> <span data-ttu-id="1c328-117">Dzēšot tiek noņemts ierīces ieraksts, un tas vairs netiek rādīts ierīču Intune sarakstā.</span><span class="sxs-lookup"><span data-stu-id="1c328-117">Deleting removes the device record so that it no longer appears in the Intune list of devices.</span></span> <span data-ttu-id="1c328-118">Ja ierīce atkal kļūst aktīva, tās lietotājam tas būs atkārtoti jāreģistrē.</span><span class="sxs-lookup"><span data-stu-id="1c328-118">If the device becomes active again, its user will have to re-enroll it.</span></span>

<span data-ttu-id="1c328-119">J: Kāpēc noteiktas attālas darbības nav pieejamas lietošanai?</span><span class="sxs-lookup"><span data-stu-id="1c328-119">Q: Why are certain remote actions not available for me to use?</span></span>

<span data-ttu-id="1c328-120">A: ne visas platformas atbalsta visas attālās ierīces darbības.</span><span class="sxs-lookup"><span data-stu-id="1c328-120">A: Not all platforms support all remote device actions.</span></span> <span data-ttu-id="1c328-121">Tālāk norādītās attālās darbības ir platformas, tāpēc tās ir pieejamas tikai norādītajām platformām.</span><span class="sxs-lookup"><span data-stu-id="1c328-121">The following remote actions are platform-specific, so they are available only for the platforms noted.</span></span>

- <span data-ttu-id="1c328-122">Apiešanas aktivizēšanas bloķēšana (tikai iOS)</span><span class="sxs-lookup"><span data-stu-id="1c328-122">Bypass Activation Lock (iOS only)</span></span>
- <span data-ttu-id="1c328-123">Jauna startēšana (tikai Windows)</span><span class="sxs-lookup"><span data-stu-id="1c328-123">Fresh Start (Windows only)</span></span>
- <span data-ttu-id="1c328-124">Pazaudēts režīms (tikai iOS)</span><span class="sxs-lookup"><span data-stu-id="1c328-124">Lost mode (iOS only)</span></span>
- <span data-ttu-id="1c328-125">Ierīces atrašana (tikai iOS)</span><span class="sxs-lookup"><span data-stu-id="1c328-125">Locate device (iOS only)</span></span>
- <span data-ttu-id="1c328-126">Restartēt (tikai operētājsistēmā Windows)</span><span class="sxs-lookup"><span data-stu-id="1c328-126">Restart (Windows only)</span></span>

<span data-ttu-id="1c328-127">Detalizētu informāciju par katru darbību skatiet rakstā [Pieejamās ierīces darbības](https://docs.microsoft.com/intune/device-management#available-device-actions).</span><span class="sxs-lookup"><span data-stu-id="1c328-127">For more details about each action, see [Available device actions](https://docs.microsoft.com/intune/device-management#available-device-actions).</span></span>