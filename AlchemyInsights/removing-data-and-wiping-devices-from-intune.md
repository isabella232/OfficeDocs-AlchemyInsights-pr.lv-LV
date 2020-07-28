---
title: Datu noņemšana un ierīču tīrīšana no Intune
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
- "1279"
- "6700008"
ms.openlocfilehash: efaf111f694ab57d0435b141a6d4baad58658ed2
ms.sourcegitcommit: e34bb95fb93250f1dc7aec6a13578bb3bb355935
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439646"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="1b8e8-102">Datu noņemšana un ierīču tīrīšana no Intune</span><span class="sxs-lookup"><span data-stu-id="1b8e8-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="1b8e8-103">Ierīces pārtraukšanas un ierīces tīrīšanas attālās darbības var izmantot, lai noņemtu uzņēmuma datus, kurus pārvalda Intune, vai lai veiktu rūpnīcas atiestatīšanu un atgrieztu ierīces noklusējuma iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="1b8e8-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="1b8e8-104">Pierakstieties Microsoft 365 ierīču pārvaldībā un dodieties uz **ierīces**  >  **visas ierīces**.</span><span class="sxs-lookup"><span data-stu-id="1b8e8-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="1b8e8-105">Atlasiet ierīci, kuru vēlaties izdzēst.</span><span class="sxs-lookup"><span data-stu-id="1b8e8-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="1b8e8-106">Atlasiet, kāda veida attālo tīrīšanu vēlaties veikt.</span><span class="sxs-lookup"><span data-stu-id="1b8e8-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="1b8e8-107">Pensionējoties dzēš tikai organizācijas informāciju, bet pilna tīrīšana atjauno ierīces rūpnīcas iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="1b8e8-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="1b8e8-108">Atlasiet **Jā** , lai apstiprinātu.</span><span class="sxs-lookup"><span data-stu-id="1b8e8-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="1b8e8-109">Līdz brīdim, kad tīrīšana ir pabeigta, ierīces darbības statuss tiek rādīts kā pensija gaida.</span><span class="sxs-lookup"><span data-stu-id="1b8e8-109">Until the wipe finishes, the Device action status shows as Retire Pending.</span></span></br>
    <span data-ttu-id="1b8e8-110">Kad darbība ir pabeigta, jūs vairs neredzat mobilo ierīci pārvaldītās ierīces sarakstā.</span><span class="sxs-lookup"><span data-stu-id="1b8e8-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

<span data-ttu-id="1b8e8-111">**Piezīmes** Uzņēmuma datus nevar noņemt no ierīcēm, kas SAVIENOTas ar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="1b8e8-111">**Note** Company data can't be removed from devices JOINED to Azure AD.</span></span>

<span data-ttu-id="1b8e8-112">Lai iegūtu pilnu informāciju par atkāpju un tīrīšanas darbību sekām, tostarp par to, kas tiek paturēts un kas tiek izdzēsts, skatiet rakstu [Ierīču noņemšana, izmantojot notīrīšanu, pensionēju vai manuāli](https://docs.microsoft.com/intune/devices-wipe)atsaucot ierīci.</span><span class="sxs-lookup"><span data-stu-id="1b8e8-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see [Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/intune/devices-wipe).</span></span>

<span data-ttu-id="1b8e8-113">Informāciju par visu datu izdzēšanu no macOS ierīces skatiet rakstā [visu datu dzēšana no MacOS ierīces](https://docs.microsoft.com/intune/device-erase).</span><span class="sxs-lookup"><span data-stu-id="1b8e8-113">To erase all data from a macOS device, see [Erase all data from a macOS device](https://docs.microsoft.com/intune/device-erase).</span></span>