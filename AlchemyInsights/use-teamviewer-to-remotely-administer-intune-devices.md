---
title: TeamViewer izmantošana, lai attāli administrētu Intune ierīces
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/28/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1284"
- "6700008"
ms.openlocfilehash: 63e7f068f3c53240ad13d1679df460c97a1a94f4
ms.sourcegitcommit: 0e50dfcdb3f6aa72368279e23b83efecb9dc9c3f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "46555241"
---
# <a name="use-teamviewer-to-remotely-administer-intune-devices"></a><span data-ttu-id="cee34-102">TeamViewer izmantošana, lai attāli administrētu Intune ierīces</span><span class="sxs-lookup"><span data-stu-id="cee34-102">Use TeamViewer to remotely administer Intune devices</span></span>

<span data-ttu-id="cee34-103">Intune pārvaldītās ierīces var lietot attāli, izmantojot [TeamViewer](https://www.teamviewer.com/).</span><span class="sxs-lookup"><span data-stu-id="cee34-103">Devices managed by Intune can be administered remotely by using [TeamViewer](https://www.teamviewer.com/).</span></span>

<span data-ttu-id="cee34-104">Lai administrētu Intune, izmantojot TeamViewer, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="cee34-104">To administer Intune by using TeamViewer, use these steps:</span></span> 

<span data-ttu-id="cee34-105">Sāciet ar akreditācijas datu saņemšanu no TeamViewer, lai iestatītu TeamViewer savienotāju pakalpojumā Intune.</span><span class="sxs-lookup"><span data-stu-id="cee34-105">Begin by obtaining credentials from TeamViewer to set up the TeamViewer Connector on Intune.</span></span> <span data-ttu-id="cee34-106">Tādējādi administrators var ievadīt akreditācijas datus TeamViewer Connector UI sadaļā ierīces — vienreizēja darbība, lai izveidotu saiti starp Intune un TeamViewer pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="cee34-106">This allows the admin to enter credentials in the TeamViewer Connector UI under Devices, a one-time operation to establish the link between Intune and the TeamViewer service.</span></span>

<span data-ttu-id="cee34-107">**1. daļa: sesijas sākšana ar attālo ierīci**</span><span class="sxs-lookup"><span data-stu-id="cee34-107">**Part 1: Start a session with a remote device**</span></span>

1. <span data-ttu-id="cee34-108">Sadaļā **visas ierīces**atlasiet ierīci, ar kuru vēlaties sākt attālo sesiju.</span><span class="sxs-lookup"><span data-stu-id="cee34-108">Under **All devices**, select the device you want to start a remote session with.</span></span>
2. <span data-ttu-id="cee34-109">No **... Papildu**atlasiet **Jauna attālās palīdzības sesija**.</span><span class="sxs-lookup"><span data-stu-id="cee34-109">From  **…More**, select **New remote assistance session**.</span></span>
3. <span data-ttu-id="cee34-110">Atlasiet **Jā** , lai apstiprinātu, ka vēlaties izveidot attālo sesiju.</span><span class="sxs-lookup"><span data-stu-id="cee34-110">Select **Yes** to acknowledge you want to establish a remote session.</span></span>
    <span data-ttu-id="cee34-111">Pēc tam, kad TeamViewer pakalpojums ir atzinis pieprasījumu "jauna Attālā sesija", tiks parādīta opcija **palaist attālo palīdzību** atbilstoši ierīces pārskata (vai Essentials) rūtij.</span><span class="sxs-lookup"><span data-stu-id="cee34-111">After the "Initiating a new remote session" request is acknowledged by the TeamViewer service, you'll see an option to **Start remote assistance** under the details of the Overview (or, Essentials) pane for the device.</span></span> <span data-ttu-id="cee34-112">Atlasiet **Skatīt vairāk** , lai izvērstu rūti un rādītu attālās palīdzības statusu.</span><span class="sxs-lookup"><span data-stu-id="cee34-112">Select **See More** to expand the pane and show the Remote Assistance status.</span></span>
4. <span data-ttu-id="cee34-113">Atlasiet **Sākt attālo sesiju** , lai sāktu sesiju administratora pusē.</span><span class="sxs-lookup"><span data-stu-id="cee34-113">Select **Start remote session** to initiate the session on the admin side.</span></span>
5. <span data-ttu-id="cee34-114">Izvēlieties lejupielādēt TeamViewer bināro failu (Windows) un pēc tam atlasiet **palaist**.</span><span class="sxs-lookup"><span data-stu-id="cee34-114">Choose to download the TeamViewer binary (Windows), and select **Run**.</span></span><br/>
    <span data-ttu-id="cee34-115">**Piezīmes** Varat ignorēt jebkuru tīmekļa pārlūkprogrammas lapu, kas atvērta TeamViewer tīmekļa vietnē.</span><span class="sxs-lookup"><span data-stu-id="cee34-115">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

6. <span data-ttu-id="cee34-116">Apstipriniet TeamViewer lietojumprogrammas pieprasījumu veikt izmaiņas ierīcē (tikai sistēmā Windows).</span><span class="sxs-lookup"><span data-stu-id="cee34-116">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
7. <span data-ttu-id="cee34-117">Tiek palaista programma TeamViewer, kurā ir iekļauts sesijas kods, lai autentificētu savienojumu ar attālo ierīci.</span><span class="sxs-lookup"><span data-stu-id="cee34-117">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>

<span data-ttu-id="cee34-118">**2. daļa: ierīcē, kas paredzēta attālai sesijai**</span><span class="sxs-lookup"><span data-stu-id="cee34-118">**Part 2: On the device being targeted for a remote session**</span></span>

1. <span data-ttu-id="cee34-119">Atveriet Intune uzņēmuma portālu.</span><span class="sxs-lookup"><span data-stu-id="cee34-119">Open the Intune company portal.</span></span>
2. <span data-ttu-id="cee34-120">Meklējiet paziņojuma karodziņu: "jūsu IT administrators pieprasa šīs ierīces vadību attālās palīdzības sesijai" un pēc tam atlasiet paziņojumu.</span><span class="sxs-lookup"><span data-stu-id="cee34-120">Look for a notification flag: "Your IT administrator is requesting control of this device for a remote assistance session," and select the notification.</span></span>
3. <span data-ttu-id="cee34-121">Izvēlieties lejupielādēt lietojumprogrammu TeamViewer vai apstiprināt programmas TeamViewer lejupielādi no lietojumprogrammu veikala un atlasiet **palaist**.</span><span class="sxs-lookup"><span data-stu-id="cee34-121">Choose to download the TeamViewer application, or acknowledge download of the TeamViewer app from the app store, and select **Run**.</span></span>
    <span data-ttu-id="cee34-122">**Piezīmes** Varat ignorēt jebkuru tīmekļa pārlūkprogrammas lapu, kas atvērta TeamViewer tīmekļa vietnē.</span><span class="sxs-lookup"><span data-stu-id="cee34-122">**Note** You can ignore any web browser page opened to the TeamViewer web site.</span></span>

4. <span data-ttu-id="cee34-123">Apstipriniet TeamViewer lietojumprogrammas pieprasījumu veikt izmaiņas ierīcē (tikai sistēmā Windows).</span><span class="sxs-lookup"><span data-stu-id="cee34-123">Acknowledge the request for the TeamViewer app to make changes on the device (Windows only).</span></span>
5. <span data-ttu-id="cee34-124">Tiek palaista programma TeamViewer, kurā ir iekļauts sesijas kods, lai autentificētu savienojumu ar attālo ierīci.</span><span class="sxs-lookup"><span data-stu-id="cee34-124">The TeamViewer app starts and includes the session code to authenticate the connection with the remote device.</span></span>
6. <span data-ttu-id="cee34-125">Uznirstošais jautājums, vai vēlaties atļaut sesijas sākšanu.</span><span class="sxs-lookup"><span data-stu-id="cee34-125">A popup asks if you want to allow the session to start.</span></span>

<span data-ttu-id="cee34-126">**Piezīmes** TeamViewer pakalpojuma ģenerētie sesijas kodi ir tikai vienreizēja izmantošana.</span><span class="sxs-lookup"><span data-stu-id="cee34-126">**Note** The session codes generated by the TeamViewer service are one-time use only.</span></span> <span data-ttu-id="cee34-127">Ja pazaudējat savienojumu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="cee34-127">If you lose the connection, you must:</span></span>

1. <span data-ttu-id="cee34-128">Attālajā ierīcē un administrēšanas darbstacijā izvērsiet lietojumprogrammas TeamViewer instanci.</span><span class="sxs-lookup"><span data-stu-id="cee34-128">Close the instance of the TeamViewer app on the remote device and on the admin workstation.</span></span>
2. <span data-ttu-id="cee34-129">Attālajā ierīcē izvērsiet uzņēmuma portālu.</span><span class="sxs-lookup"><span data-stu-id="cee34-129">Close the company portal on the remote device.</span></span>
3. <span data-ttu-id="cee34-130">Administrēšanas portālā sāciet jaunu attālās palīdzības sesiju.</span><span class="sxs-lookup"><span data-stu-id="cee34-130">Initiate a new "New remote Assistance session" from the admin portal.</span></span>
4. <span data-ttu-id="cee34-131">Atkārtoti atveriet uzņēmuma portālu attālajā ierīcē, lai saņemtu jauno paziņojumu.</span><span class="sxs-lookup"><span data-stu-id="cee34-131">Re-open the company portal on the remote device to receive the new notification.</span></span>
5. <span data-ttu-id="cee34-132">Lejupielādējiet un atveriet programmu TeamViewer gan attālajā ierīcē, gan administratora darbstacijā, kā iepriekš.</span><span class="sxs-lookup"><span data-stu-id="cee34-132">Download and open the TeamViewer app on both the remote device and the admin workstation, as before.</span></span>