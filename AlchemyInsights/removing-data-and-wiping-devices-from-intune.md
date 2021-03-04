---
title: Datu un tīrīšanas ierīču noņemšana no Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/27/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1279"
- "6700008"
- "9004638"
- "8392"
ms.openlocfilehash: cada3c6f1e7d1dcd576baa1245fb5a62ed938613
ms.sourcegitcommit: 229bd519ec1c14c65a243226a94eee23e117a7fc
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/03/2021
ms.locfileid: "50416320"
---
# <a name="removing-data-and-wiping-devices-from-intune"></a><span data-ttu-id="83ca8-102">Datu un tīrīšanas ierīču noņemšana no Intune</span><span class="sxs-lookup"><span data-stu-id="83ca8-102">Removing data and wiping devices from Intune</span></span>

<span data-ttu-id="83ca8-103">Ierīces norakstīšanas un ierīces tīrīšanas attālās darbības var izmantot, lai noņemtu Intune pārvaldītos uzņēmuma datus vai veiktu rūpnīcas atiestatīšanu un atgrieztu ierīci noklusējuma iestatījumos.</span><span class="sxs-lookup"><span data-stu-id="83ca8-103">The Device Retire and Device Wipe remote actions can be used to remove company data managed by Intune or to perform a factory reset and return the device to its default settings.</span></span>

1. <span data-ttu-id="83ca8-104">Pierakstieties Microsoft 365 ierīču pārvaldībā un dodieties uz sadaļu **Ierīces** > **Visas ierīces**.</span><span class="sxs-lookup"><span data-stu-id="83ca8-104">Sign into Microsoft 365 Device Management, and go to **Devices** > **All Devices**.</span></span>
2. <span data-ttu-id="83ca8-105">Atlasiet ierīci, kuru vēlaties tīrīt.</span><span class="sxs-lookup"><span data-stu-id="83ca8-105">Select the device you want to wipe.</span></span>
3. <span data-ttu-id="83ca8-106">Atlasiet, kāda veida attālo tīrīšanu vēlaties veikt.</span><span class="sxs-lookup"><span data-stu-id="83ca8-106">Select the type of remote wipe you want to do.</span></span> <span data-ttu-id="83ca8-107">Norakstīšanā tiek izdzēsta tikai organizācijas informācija, bet pilna tīrīšana atjauno ierīces rūpnīcas iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="83ca8-107">Retire deletes only organizational information, while full wipes restore the device to its factory settings.</span></span>
4. <span data-ttu-id="83ca8-108">Atlasiet **Jā**, lai apstiprinātu.</span><span class="sxs-lookup"><span data-stu-id="83ca8-108">Select **Yes** to confirm.</span></span> <span data-ttu-id="83ca8-109">Līdz tīrīšana ir pabeigta, ierīces darbības statuss tiek rādīts kā *Gaida norakstīšanu*.</span><span class="sxs-lookup"><span data-stu-id="83ca8-109">Until the wipe finishes, the Device action status shows as *Retire Pending*.</span></span>
    <span data-ttu-id="83ca8-110">Kad darbība būs pabeigta, mobilo ierīci vairs neredzēsit pārvaldītās ierīces sarakstā.</span><span class="sxs-lookup"><span data-stu-id="83ca8-110">After the action is completed, you'll no longer see the mobile device in the list of managed device.</span></span>

> [!NOTE]
> <span data-ttu-id="83ca8-111">Uzņēmuma datus nevar noņemt no ierīcēm, kas PIEVIENOTAS Azure AD.</span><span class="sxs-lookup"><span data-stu-id="83ca8-111">Company data can't be removed from devices JOINED to Azure AD.</span></span> 

<span data-ttu-id="83ca8-112">Pilnu detalizētu informāciju par norakstīšanas un tīrīšanas darbībām, tostarp par to, kas tiek saglabāts un kas tiek izdzēsts, skatiet tālāk norādītajā dokumentācijā:</span><span class="sxs-lookup"><span data-stu-id="83ca8-112">For full details of the effect of the Retire and Wipe actions, including what is retained and what is deleted, see following documentation:</span></span>

- <span data-ttu-id="83ca8-113">[Noņemiet ierīces, izmantojot tīrīšanu, norakstīšanu vai manuāli atceliet ierīces reģistrāciju](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span><span class="sxs-lookup"><span data-stu-id="83ca8-113">[Remove devices by using wipe, retire, or manually unenrolling the device](https://docs.microsoft.com/mem/intune/remote-actions/devices-wipe).</span></span>
- [<span data-ttu-id="83ca8-114">Kā tīrīt tikai uzņēmuma datus no Intune pārvaldītām lietojumprogrammām</span><span class="sxs-lookup"><span data-stu-id="83ca8-114">How to wipe only corporate data from Intune-managed apps</span></span>](https://docs.microsoft.com/mem/intune/apps/apps-selective-wipe)
- <span data-ttu-id="83ca8-115">[Dzēsiet visus datus no MacOS ierīces](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span><span class="sxs-lookup"><span data-stu-id="83ca8-115">[Erase all data from a macOS device](https://docs.microsoft.com/mem/intune/remote-actions/device-erase).</span></span>