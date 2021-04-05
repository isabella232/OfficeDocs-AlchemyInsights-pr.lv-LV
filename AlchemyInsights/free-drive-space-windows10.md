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
- "9774"
- "9005390"
- "9005403"
ms.openlocfilehash: 2313636307bfddce2810c2d4c4ce9e3b407a7bdf
ms.sourcegitcommit: 7b2e5078dd65f11af6650e692a7ea48e91f544e0
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/02/2021
ms.locfileid: "51505363"
---
# <a name="free-up-drive-space-in-windows-10"></a><span data-ttu-id="0e5d3-102">Diska vietas atbrīvošana operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="0e5d3-102">Free up drive space in Windows 10</span></span>

<span data-ttu-id="0e5d3-103">Šeit ir divas opcijas, lai atbrīvotu diska vietu operētājsistēmā Windows 10:</span><span class="sxs-lookup"><span data-stu-id="0e5d3-103">Here are two options to free up drive space in Windows:</span></span>

- <span data-ttu-id="0e5d3-104">Diska vietas atbrīvošana operētājsistēmā Windows 10.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-104">Free up drive space in Windows 10.</span></span>
- <span data-ttu-id="0e5d3-105">Atbrīvojiet vietu operētājsistēmas Windows 10 atjauninājumiem, izmantojot ārējo krātuves ierīci.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-105">Free up space for Windows 10 updates with external storage device.</span></span>

<span data-ttu-id="0e5d3-106">Ja pēc diska tīrīšanas izmantošanas vēl joprojām ir maz vietas diskā, iespējams, ka mape Temp ātri tiek piepildīta ar programmas (.appx) failiem, kurus izmanto Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-106">If you still have low disk space after using Disk Cleanup, it’s possible that your Temp folder is quickly filling up with application (.appx) files used by Microsoft Store.</span></span> <span data-ttu-id="0e5d3-107">Lai novērstu šo problēmu, atiestatiet Microsoft Store, iztīriet tā kešatmiņu un pēc tam palaidiet Windows Update problēmu risinātāju.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-107">To fix this problem, reset the Store, clear the Store cache, and then run the Windows Update troubleshooter.</span></span> <span data-ttu-id="0e5d3-108">Pirms šo darbību veikšanas pārliecinieties, vai Microsoft Store ir aizvērts.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-108">Make sure Microsoft Store is closed before you proceed with these steps.</span></span>

<span data-ttu-id="0e5d3-109">**1. darbība: Microsoft Store atiestatīšana**</span><span class="sxs-lookup"><span data-stu-id="0e5d3-109">**Step 1: Reset Microsoft Store**</span></span>

<span data-ttu-id="0e5d3-110">**Piezīme** Tādējādi ierīcē tiks neatgriezeniski izdzēsti programmas dati, tostarp jūsu preferences un pierakstīšanās dati.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-110">**Note** This permanently deletes the app data on the device, including your preferences and sign-in details.</span></span>

1. <span data-ttu-id="0e5d3-111">Atlasiet **Sākt** > **, Iestatījumi** > **, Programmas** > **,Programmas un līdzekļi**.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-111">Select **Start** > **Settings** > **Apps** > **Apps & features**.</span></span>

1. <span data-ttu-id="0e5d3-112">Programmu sarakstā atrodiet un atlasiet Microsoft Store.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-112">In the list of apps, locate and select Microsoft Store.</span></span>

1. <span data-ttu-id="0e5d3-113">Atlasiet **Papildu opcijas**.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-113">Select **Advanced options**.</span></span>

1. <span data-ttu-id="0e5d3-114">Ritiniet uz leju un atlasiet **Atiestatīt** un pēc tam **Apstiprināt atiestatīšanu**.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-114">Scroll down and select **Reset**, and then **Confirm Reset**.</span></span>

<span data-ttu-id="0e5d3-115">**2. darbība: Microsoft Store kešatmiņas notīrīšana**</span><span class="sxs-lookup"><span data-stu-id="0e5d3-115">**Step 2: Clear the Microsoft Store cache**</span></span>

1. <span data-ttu-id="0e5d3-116">Nospiediet taustiņu kombināciju Windows logotipa taustiņš+R, lai atvērtu un palaistu dialoglodziņu.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-116">Press the Windows Logo Key + R to open the Run dialog box.</span></span>

1. <span data-ttu-id="0e5d3-117">Ierakstiet wsreset.exe un atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-117">Type wsreset.exe and select **OK**.</span></span>

1. <span data-ttu-id="0e5d3-118">Atveras tukšs komandu uzvednes logs.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-118">A blank Command Prompt window opens.</span></span> <span data-ttu-id="0e5d3-119">Pēc aptuveni 10 sekundēm logs aizveras un Microsoft Store atveras automātiski.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-119">After about 10 seconds, the window closes and the Store opens automatically.</span></span>

<span data-ttu-id="0e5d3-120">**3. darbība: Windows Update atiestatīšana**</span><span class="sxs-lookup"><span data-stu-id="0e5d3-120">**Step 3: Reset Windows Update**</span></span>

1. <span data-ttu-id="0e5d3-121">Atlasiet **Sākt** > **, Iestatījumi** > **, Atjauninājumi un drošība** > **, Problēmu novēršana**.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-121">Select **Start** > **Settings** > **Update & Security** > **Troubleshoot**.</span></span>

1. <span data-ttu-id="0e5d3-122">Ritiniet uz leju un sarakstā atlasiet **Windows Update** un pēc tam atlasiet **Palaist problēmu risinātāju**.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-122">Scroll down and select **Windows Update** from the list, and select **Run the troubleshooter**.</span></span>

1. <span data-ttu-id="0e5d3-123">Restartējiet datoru un pārbaudiet, vai problēma joprojām pastāv.</span><span class="sxs-lookup"><span data-stu-id="0e5d3-123">Reboot your computer and check whether you're still experiencing the issue.</span></span>

