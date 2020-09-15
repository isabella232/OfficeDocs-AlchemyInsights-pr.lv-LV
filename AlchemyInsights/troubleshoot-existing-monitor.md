---
title: Esošā monitora problēmu novēršana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: 2dc9a24c1d0d808e26733738cedbc32d513926a0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690718"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="a10f8-102">Esošā monitora problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="a10f8-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="a10f8-103">Izmēģiniet šos risinājumus, lai novērstu monitoru.</span><span class="sxs-lookup"><span data-stu-id="a10f8-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="a10f8-104">**Atsvaidzināt monitora displeju:**</span><span class="sxs-lookup"><span data-stu-id="a10f8-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="a10f8-105">Vienlaikus nospiediet šos taustiņus: Windows taustiņš + CTRL + SHIFT + B. Tādējādi tiks atsvaidzināta komunikācija ar jūsu grafikas draiveri.</span><span class="sxs-lookup"><span data-stu-id="a10f8-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="a10f8-106">Jūsu monitori acumirklī mirgos un atgriezīsies pēc dažām sekundēm.</span><span class="sxs-lookup"><span data-stu-id="a10f8-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="a10f8-107">**Monitora aparatūras problēmu novēršana:**</span><span class="sxs-lookup"><span data-stu-id="a10f8-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="a10f8-108">Atvienojiet kabeli, kas savieno jūsu datoru ar monitoru, un pievienojiet to atpakaļ.</span><span class="sxs-lookup"><span data-stu-id="a10f8-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="a10f8-109">Atvienojiet ierīces no datora (piemēram, adapterus vai dokus).</span><span class="sxs-lookup"><span data-stu-id="a10f8-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="a10f8-110">**Ja nesen instalējāt atjauninājumu savā datorā, varat atritināt savu interfeisa draiveri:**</span><span class="sxs-lookup"><span data-stu-id="a10f8-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="a10f8-111">Atlasiet **Sākt**, ierakstiet **ierīču pārvaldnieks**un pēc tam rezultātos atlasiet **ierīču pārvaldnieks** .</span><span class="sxs-lookup"><span data-stu-id="a10f8-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="a10f8-112">Izvērsiet sadaļu **parādāmie adapteri** , ar peles labo pogu noklikšķiniet uz parādāmā adaptera, rupjās daļas atlasiet **Rekvizīti**.</span><span class="sxs-lookup"><span data-stu-id="a10f8-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="a10f8-113">Pārejiet uz cilni **draiveris** un atlasiet **atritināt draiveri**.</span><span class="sxs-lookup"><span data-stu-id="a10f8-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="a10f8-114">Piezīme. Ja tas nav pieejams vai ir pelēkots, atlasiet **Nē** no tālāk norādītajām opcijām, lai pārietu uz nākamo darbību.</span><span class="sxs-lookup"><span data-stu-id="a10f8-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="a10f8-115">Lai šīs izmaiņas stātos spēkā, iespējams, būs jārestartē dators.</span><span class="sxs-lookup"><span data-stu-id="a10f8-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="a10f8-116">**Atinstalējiet un atkārtoti instalējiet savu interfeisa draiveri:**</span><span class="sxs-lookup"><span data-stu-id="a10f8-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="a10f8-117">Atlasiet **Sākt**, ierakstiet **ierīču pārvaldnieks**un pēc tam rezultātos atlasiet **ierīču pārvaldnieks** .</span><span class="sxs-lookup"><span data-stu-id="a10f8-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="a10f8-118">Izvērsiet sadaļu **parādāmie adapteri** , ar peles labo pogu noklikšķiniet uz jūsu parādāmā adaptera, rupjās atlasiet **atinstalēt ierīci**.</span><span class="sxs-lookup"><span data-stu-id="a10f8-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="a10f8-119">Atzīmējiet izvēles rūtiņu blakus **Dzēst draivera programmatūru šai ierīcei** un atlasiet **Atinstalēt**.</span><span class="sxs-lookup"><span data-stu-id="a10f8-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="a10f8-120">Piezīme. Šajā posmā jums, iespējams, būs jārestartē dators.</span><span class="sxs-lookup"><span data-stu-id="a10f8-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="a10f8-121">Pirms restartēšanas noteikti pierakstiet atlikušās instrukcijas.</span><span class="sxs-lookup"><span data-stu-id="a10f8-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="a10f8-122">Vēlreiz atveriet ierīču pārvaldnieku.</span><span class="sxs-lookup"><span data-stu-id="a10f8-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="a10f8-123">Izvērsiet sadaļu **parādāmie adapteri** , ar peles labo pogu noklikšķiniet uz jūsu parādāmā adaptera un atlasiet **Atjaunināt draiveri**.</span><span class="sxs-lookup"><span data-stu-id="a10f8-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="a10f8-124">**Lai atjauninātu draivera programmatūru, atlasiet automātiski meklēt** un izpildiet instalēšanas norādījumus.</span><span class="sxs-lookup"><span data-stu-id="a10f8-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>