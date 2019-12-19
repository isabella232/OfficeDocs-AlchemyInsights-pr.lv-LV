---
title: Esošā monitora problēmu novēršana
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3454"
- "9001450"
ms.openlocfilehash: d90baddd01bdf8508bd6289509c8399b8241887a
ms.sourcegitcommit: 42463e8d8869f36225a27388d83d37629c6b149e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/18/2019
ms.locfileid: "40738575"
---
# <a name="troubleshoot-an-existing-monitor"></a><span data-ttu-id="d02b1-102">Esoša monitora problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="d02b1-102">Troubleshoot an existing monitor</span></span>

<span data-ttu-id="d02b1-103">Izmēģiniet šos risinājumus, lai novērstu monitora problēmas.</span><span class="sxs-lookup"><span data-stu-id="d02b1-103">Try these solutions to troubleshoot a monitor.</span></span> 

<span data-ttu-id="d02b1-104">**Atsvaidzināt monitora displeju:**</span><span class="sxs-lookup"><span data-stu-id="d02b1-104">**Refresh your monitor's display:**</span></span>

<span data-ttu-id="d02b1-105">Vienlaikus nospiediet šādus taustiņus: Windows taustiņu + CTRL + SHIFT + B. Tas atsvaidzinās saziņu ar jūsu grafikas draiveri.</span><span class="sxs-lookup"><span data-stu-id="d02b1-105">Press the following keys at the same time: Windows Key  + Ctrl + Shift + B. This will refresh communication with your graphics driver.</span></span> <span data-ttu-id="d02b1-106">Monitori mirgos momentāni un atgriezīsies pēc dažām sekundēm.</span><span class="sxs-lookup"><span data-stu-id="d02b1-106">Your monitors will blink momentarily and come back after a few seconds.</span></span>

<span data-ttu-id="d02b1-107">**Monitora aparatūras problēmu novēršana:**</span><span class="sxs-lookup"><span data-stu-id="d02b1-107">**Troubleshoot monitor hardware:**</span></span>

1. <span data-ttu-id="d02b1-108">Atvienojiet kabeli, kas savieno datoru un monitoru, un pievienojiet to atpakaļ.</span><span class="sxs-lookup"><span data-stu-id="d02b1-108">Unplug the cable connecting your PC to your monitor, and plug it back in.</span></span>
2. <span data-ttu-id="d02b1-109">Atvienojiet visas ierīces, kas nav būtiskas, no datora (piemēram, adapteri vai dokus).</span><span class="sxs-lookup"><span data-stu-id="d02b1-109">Disconnect any non-essential devices from your PC (such as adapters or docks).</span></span>

<span data-ttu-id="d02b1-110">**Ja nesen datorā instalējāt atjauninājumu, varat atritināt displeja draiveri:**</span><span class="sxs-lookup"><span data-stu-id="d02b1-110">**If you recently installed an update on your PC, you can roll back your display driver:**</span></span>

1. <span data-ttu-id="d02b1-111">Atlasiet **Sākt**, ierakstiet **ierīču pārvaldnieks**un rezultātu sarakstā atlasiet **ierīču pārvaldnieks** .</span><span class="sxs-lookup"><span data-stu-id="d02b1-111">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="d02b1-112">Izvērsiet sadaļu **displeja adapteri** , ar peles labo pogu noklikšķiniet uz displeja adaptera, ANDS atlasiet **Rekvizīti**.</span><span class="sxs-lookup"><span data-stu-id="d02b1-112">Expand the **Display adapters** section, right-click your display adapter, ands select **Properties**.</span></span>
3. <span data-ttu-id="d02b1-113">Pārejiet uz cilni **draiveris** un atlasiet **Atrites draiveris**.</span><span class="sxs-lookup"><span data-stu-id="d02b1-113">Navigate to the **Driver** tab and select **Roll Back Driver**.</span></span> <br>
<span data-ttu-id="d02b1-114">Piezīme: ja tas nav pieejams vai ir pelēkota **, izvēlieties no** zemāk norādītajām iespējām, lai pārietu uz nākamo soli.</span><span class="sxs-lookup"><span data-stu-id="d02b1-114">Note: If this isn't available or is grayed out, select **No** from the options below to move to the next step.</span></span>
4. <span data-ttu-id="d02b1-115">Lai šīs izmaiņas stātos spēkā, iespējams, būs jārestartē dators.</span><span class="sxs-lookup"><span data-stu-id="d02b1-115">You may need to restart your PC before these changes take effect.</span></span>

<span data-ttu-id="d02b1-116">**Atinstalējiet un atkārtoti instalējiet displeja draiveri:**</span><span class="sxs-lookup"><span data-stu-id="d02b1-116">**Uninstall and reinstall your display driver:**</span></span>

1. <span data-ttu-id="d02b1-117">Atlasiet **Sākt**, ierakstiet **ierīču pārvaldnieks**un rezultātu sarakstā atlasiet **ierīču pārvaldnieks** .</span><span class="sxs-lookup"><span data-stu-id="d02b1-117">Select **Start**, type **device manager**, and select **Device Manager** from the results.</span></span>
2. <span data-ttu-id="d02b1-118">Izvērsiet sadaļu **displeja adapteri** , ar peles labo pogu noklikšķiniet uz displeja adaptera, ANDS atlasiet **atinstalēt ierīci**.</span><span class="sxs-lookup"><span data-stu-id="d02b1-118">Expand the **Display adapters** section, right-click your display adapter, ands select **Uninstall device**.</span></span> 
3. <span data-ttu-id="d02b1-119">Atzīmējiet izvēles rūtiņu blakus **dzēst šīs ierīces draivera programmatūru** un atlasiet **atinstalēt**.</span><span class="sxs-lookup"><span data-stu-id="d02b1-119">Select the box next to **Delete the driver software for this device** and select **Uninstall**.</span></span><br>
<span data-ttu-id="d02b1-120">Piezīme: šajā posmā var tikt lūgts restartēt datoru.</span><span class="sxs-lookup"><span data-stu-id="d02b1-120">Note: You may be asked to restart your computer at this stage.</span></span> <span data-ttu-id="d02b1-121">Pirms restartēšanas noteikti pierakstiet pārējos norādījumus.</span><span class="sxs-lookup"><span data-stu-id="d02b1-121">Make sure to write down the remaining instructions before you restart.</span></span>
4. <span data-ttu-id="d02b1-122">Vēlreiz atveriet ierīču pārvaldnieku.</span><span class="sxs-lookup"><span data-stu-id="d02b1-122">Open Device Manager again.</span></span>
5. <span data-ttu-id="d02b1-123">Izvērsiet sadaļu **displeja adapteri** , ar peles labo pogu noklikšķiniet uz displeja adaptera un atlasiet **Atjaunināt draiveri**.</span><span class="sxs-lookup"><span data-stu-id="d02b1-123">Expand the **Display adapters** section, right-click on your display adapter, and select **Update Driver**.</span></span>
6. <span data-ttu-id="d02b1-124">Atlasiet **automātiski meklēt, lai atjauninātu draivera programmatūru** , un izpildiet instalēšanas norādījumus.</span><span class="sxs-lookup"><span data-stu-id="d02b1-124">Select **Search automatically for update driver software** and follow the installation instructions.</span></span>