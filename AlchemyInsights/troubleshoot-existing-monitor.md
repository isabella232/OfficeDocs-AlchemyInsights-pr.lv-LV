---
title: Esoša monitora problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: c4d2bb64b6b5ea79d4cd585e2be85c3c17e0f76f
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51824586"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="48436-102">Problēmu novēršana esošā monitorā</span><span class="sxs-lookup"><span data-stu-id="48436-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="48436-103">Izmēģiniet šos risinājumus, lai novērstu problēmas monitorā.</span><span class="sxs-lookup"><span data-stu-id="48436-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="48436-104">**Atsvaidziniet monitora displeju.**</span><span class="sxs-lookup"><span data-stu-id="48436-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="48436-105">Vienlaikus nospiediet šādus taustiņus: Windows taustiņš + Ctrl + Shift + B. Tādējādi tiks atsvaidzināta saziņa ar jūsu grafikas draiveri.</span><span class="sxs-lookup"><span data-stu-id="48436-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="48436-106">Jūsu monitori uz brīdi mirgos un atgriezīsies pēc dažām sekundēm.</span><span class="sxs-lookup"><span data-stu-id="48436-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="48436-107">**Problēmu novēršana saistībā ar monitora aparatūru:**</span><span class="sxs-lookup"><span data-stu-id="48436-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="48436-108">Atvienojiet kabeli, kas savieno datoru ar monitoru, un iespraudiet to atpakaļ.</span><span class="sxs-lookup"><span data-stu-id="48436-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="48436-109">Atvienojiet no datora visas svarīgākās ierīces (piemēram, adapterus vai dokos).</span><span class="sxs-lookup"><span data-stu-id="48436-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="48436-110">**Ja nesen instalējāt atjauninājumu savā datorā, varat atritiniet displeja draiveri:**</span><span class="sxs-lookup"><span data-stu-id="48436-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="48436-111">Atlasiet **Sākt**, ierakstiet **Ierīču pārvaldnieks** un **rezultātos** atlasiet Ierīču pārvaldnieks.</span><span class="sxs-lookup"><span data-stu-id="48436-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="48436-112">Izvērsiet **sadaļu Displeja adapteri,** ar peles labo pogu noklikšķiniet uz displeja adaptera un atlasiet **Rekvizīti**.</span><span class="sxs-lookup"><span data-stu-id="48436-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="48436-113">Naviģējiet **uz cilni** Draiveris un **atlasiet Atritiniet draiveri**.</span><span class="sxs-lookup"><span data-stu-id="48436-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="48436-114">Piezīme. Ja šī opcija nav pieejama vai  ir pelēkota, tālāk redzamajās opcijās atlasiet Nē, lai pārietu uz nākamo darbību.</span><span class="sxs-lookup"><span data-stu-id="48436-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="48436-115">Lai šīs izmaiņas stātos spēkā, iespējams, būs jārestartē dators.</span><span class="sxs-lookup"><span data-stu-id="48436-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="48436-116">**Atinstalējiet un atkārtoti instalējiet displeja draiveri.**</span><span class="sxs-lookup"><span data-stu-id="48436-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="48436-117">Atlasiet **Sākt**, ierakstiet **Ierīču pārvaldnieks** un **rezultātos** atlasiet Ierīču pārvaldnieks.</span><span class="sxs-lookup"><span data-stu-id="48436-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="48436-118">Izvērsiet **sadaļu Displeja adapteri,** ar peles labo pogu noklikšķiniet uz displeja adaptera un atlasiet **Atinstalēt ierīci**.</span><span class="sxs-lookup"><span data-stu-id="48436-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="48436-119">Atzīmējiet izvēles rūtiņu **blakus Dzēst šīs ierīces draivera programmatūru un** atlasiet **Atinstalēt**.</span><span class="sxs-lookup"><span data-stu-id="48436-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="48436-120">Piezīme. Iespējams, jums tiks lūgts restartēt datoru šajā posmā.</span><span class="sxs-lookup"><span data-stu-id="48436-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="48436-121">Pirms restartēšanas noteikti pierakstiet pārējos norādījumus.</span><span class="sxs-lookup"><span data-stu-id="48436-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="48436-122">Vēlreiz atveriet ierīču pārvaldnieku.</span><span class="sxs-lookup"><span data-stu-id="48436-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="48436-123">Izvērsiet **sadaļu Displeja adapteri,** ar peles labo pogu noklikšķiniet uz displeja adaptera un atlasiet **Atjaunināt draiveri**.</span><span class="sxs-lookup"><span data-stu-id="48436-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="48436-124">Atlasiet **Automātiski meklēt draivera programmatūras atjaunināšanu un** izpildiet instalēšanas norādījumus.</span><span class="sxs-lookup"><span data-stu-id="48436-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>