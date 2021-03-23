---
title: Diska vietas atbrīvošana operētājsistēmā Windows 10
ms.author: pebaum
author: pebaum
manager: dansimp
ms.date: 03/16/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9771"
- "9005403"
ms.openlocfilehash: 3838f3db3bc5f54bcb1a2558484056f3194b76e1
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036589"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="a03f6-102">Diska vietas atbrīvošana operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="a03f6-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="a03f6-103">Tālāk ir divas iespējas, kā atbrīvot vietu diskā operētājsistēmā Windows.</span><span class="sxs-lookup"><span data-stu-id="a03f6-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="a03f6-104">Atbrīvojiet vietu diskā operētājsistēmā Windows 10.</span><span class="sxs-lookup"><span data-stu-id="a03f6-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="a03f6-105">Atbrīvojiet vietu Windows 10 atjauninājumiem ar ārējās krātuves ierīci.</span><span class="sxs-lookup"><span data-stu-id="a03f6-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="a03f6-106">Ja pēc diska tīrīšanas joprojām ir maz brīvas vietas, iespējams, ka jūsu Temp mape ir ātri piepildīta ar lietojumprogrammu (. Appx) failiem, ko izmanto Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="a03f6-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="a03f6-107">Lai novērstu šo problēmu, atiestatiet veikalu, notīriet veikala kešatmiņu un pēc tam palaidiet Windows Update problēmu risinātāju.</span><span class="sxs-lookup"><span data-stu-id="a03f6-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="a03f6-108">Pirms turpināt šīs darbības, pārliecinieties, vai Microsoft veikals ir aizvērts.</span><span class="sxs-lookup"><span data-stu-id="a03f6-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="a03f6-109">**1. darbība: Microsoft Store atiestatīšana**</span><span class="sxs-lookup"><span data-stu-id="a03f6-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="a03f6-110">**Piezīmes** Šī darbība neatgriezeniski izdzēš lietojumprogrammas datus ierīcē, ieskaitot jūsu preferences un pierakstīšanās informāciju.</span><span class="sxs-lookup"><span data-stu-id="a03f6-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="a03f6-111">Atlasiet **Sākt**  >  **iestatījumu**  >  **programmu**  >  **programmas & līdzekļus**.</span><span class="sxs-lookup"><span data-stu-id="a03f6-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="a03f6-112">Programmu sarakstā atrodiet un atlasiet Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="a03f6-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="a03f6-113">Atlasiet **Papildu opcijas**.</span><span class="sxs-lookup"><span data-stu-id="a03f6-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="a03f6-114">Ritiniet uz leju un atlasiet **Atiestatīt** un pēc tam **apstipriniet atiestatīšanu**.</span><span class="sxs-lookup"><span data-stu-id="a03f6-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="a03f6-115">**2. darbība: Microsoft Store kešatmiņas notīrīšana**</span><span class="sxs-lookup"><span data-stu-id="a03f6-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="a03f6-116">Nospiediet Windows logotipa taustiņu + R, lai atvērtu palaišanas dialoglodziņu.</span><span class="sxs-lookup"><span data-stu-id="a03f6-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="a03f6-117">Ierakstiet wsreset.exe un atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="a03f6-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="a03f6-118">Tiek atvērts tukšs komandu uzvednes logs.</span><span class="sxs-lookup"><span data-stu-id="a03f6-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="a03f6-119">Pēc aptuveni 10 sekundēm logs tiek aizvērts, un krātuve tiek atvērta automātiski.</span><span class="sxs-lookup"><span data-stu-id="a03f6-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="a03f6-120">**3. darbība: atiestatiet Windows Update**</span><span class="sxs-lookup"><span data-stu-id="a03f6-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="a03f6-121">Atlasiet **Sākt**  >  **iestatījumu**  >  **atjaunināšanu & drošības**  >  **problēmu novēršana**.</span><span class="sxs-lookup"><span data-stu-id="a03f6-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="a03f6-122">Ritiniet uz leju un sarakstā atlasiet **Windows Update** un atlasiet **palaist problēmu risinātāju**.</span><span class="sxs-lookup"><span data-stu-id="a03f6-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="a03f6-123">Restartējiet datoru un pārbaudiet, vai joprojām rodas problēma.</span><span class="sxs-lookup"><span data-stu-id="a03f6-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

