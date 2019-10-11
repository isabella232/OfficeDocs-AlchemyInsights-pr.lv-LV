---
title: Iestrēdzis izsūtnē lielu pielikumu dēļ
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2713"
- "9000768"
ms.openlocfilehash: d5fb20fcc146be67c5a04de0640ed4efd625311a
ms.sourcegitcommit: 8004ee243b5c68ff9532224a2e6c69dda0abbd0b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 10/10/2019
ms.locfileid: "37441312"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="62a51-102">Labot izsūtnē iestrēgušos ziņojumus</span><span class="sxs-lookup"><span data-stu-id="62a51-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="62a51-103">Ieteicams sākt, palaižot scenāriju ["man ir problēmas ar e-pasta ziņojumu sūtīšanu, saņemšanu vai atrašanu"](https://aka.ms/SaRA-OutlookSendReceive) no [Microsoft atbalsta un atkopšanas palīga](https://diagnostics.office.com/#/) rīka.</span><span class="sxs-lookup"><span data-stu-id="62a51-103">We recommend that you start by running the scenario ["I’m having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="62a51-104">Kad ziņojums iestrēgst Izsūtnē, iespējamie cēloņi ir:</span><span class="sxs-lookup"><span data-stu-id="62a51-104">When a message gets stuck in your Outbox, the most likely causes are:</span></span>
- <span data-ttu-id="62a51-105">Lieliem pielikumiem.</span><span class="sxs-lookup"><span data-stu-id="62a51-105">Large attachments.</span></span>
- <span data-ttu-id="62a51-106">Nav iespējota opcija **Nosūtīt tūlīt pēc savienojuma** .</span><span class="sxs-lookup"><span data-stu-id="62a51-106">The **Send immediately when connected** option is not enabled.</span></span>

<span data-ttu-id="62a51-107">Lai noņemtu lielus pielikumus:</span><span class="sxs-lookup"><span data-stu-id="62a51-107">To remove large attachments:</span></span> 

1. <span data-ttu-id="62a51-108">Programmā Outlook atlasiet **Nosūtīt/saņemt** > **darbu bezsaistē**.</span><span class="sxs-lookup"><span data-stu-id="62a51-108">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="62a51-109">Navigācijas rūtī atlasiet **Izsūtne**.</span><span class="sxs-lookup"><span data-stu-id="62a51-109">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="62a51-110">No šejienes jūs varat:</span><span class="sxs-lookup"><span data-stu-id="62a51-110">From here, you can:</span></span> 
    - <span data-ttu-id="62a51-111">Izdzēsiet ziņu (atlasiet to un pēc tam atlasiet **Dzēst**).</span><span class="sxs-lookup"><span data-stu-id="62a51-111">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="62a51-112">Velciet ziņojumu uz melnrakstu mapi, veiciet dubultklikšķi, lai to atvērtu, un noņemiet pielikumu atlasiet to un pēc tam atlasiet **Dzēst**).</span><span class="sxs-lookup"><span data-stu-id="62a51-112">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="62a51-113">Ja tiek parādīts kļūdas ziņojums, kurā teikts, ka programma Outlook mēģina pārraidīt ziņojumu, aizveriet programmu Outlook.</span><span class="sxs-lookup"><span data-stu-id="62a51-113">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="62a51-114">Tas var aizņemt kādu brīdi, lai izietu.</span><span class="sxs-lookup"><span data-stu-id="62a51-114">It may take a few moments to exit.</span></span> <span data-ttu-id="62a51-115">Ja programma Outlook netiek aizvērta, nospiediet taustiņu kombināciju CTRL + ALT + DELETE un atlasiet **startēt uzdevumu pārvaldnieku**.</span><span class="sxs-lookup"><span data-stu-id="62a51-115">If Outlook doesn’t close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="62a51-116">Uzdevumu pārvaldniekā atlasiet cilni **procesi** , ritiniet uz leju līdz Outlook. exe un atlasiet **Beigt procesu**.</span><span class="sxs-lookup"><span data-stu-id="62a51-116">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="62a51-117">Kad programma Outlook tiek aizvērta, restartējiet to un atkārtojiet 2. un 3. darbību.</span><span class="sxs-lookup"><span data-stu-id="62a51-117">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="62a51-118">Pēc pielikuma noņemšanas noklikšķiniet uz **Nosūtīt/saņemt** > **darbu bezsaistē** , lai atsāktu darbu tiešsaistē.</span><span class="sxs-lookup"><span data-stu-id="62a51-118">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="62a51-119">Ziņojumi tiek iestrēguši arī izsūtnē, kad noklikšķināt uz **nosūtīt**, bet nav izveidots savienojums.</span><span class="sxs-lookup"><span data-stu-id="62a51-119">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="62a51-120">Noklikšķiniet uz **Nosūtīt/saņemt** un paskatieties uz pogu **strādāt bezsaistē** .</span><span class="sxs-lookup"><span data-stu-id="62a51-120">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="62a51-121">Ja tas ir zils, jūs esat atvienots.</span><span class="sxs-lookup"><span data-stu-id="62a51-121">If it's blue, you're disconnected.</span></span> <span data-ttu-id="62a51-122">Atlasiet to, lai izveidotu savienojumu (poga kļūst balta) un noklikšķiniet uz **Sūtīt visu**.</span><span class="sxs-lookup"><span data-stu-id="62a51-122">Select it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="62a51-123">Lai iespējotu **nosūtīšanu tūlīt pēc savienojuma**:</span><span class="sxs-lookup"><span data-stu-id="62a51-123">To enable **Send immediately when connected**:</span></span>
 
- <span data-ttu-id="62a51-124">Atlasiet **failu** > **Opcijas** >  **papildu**.</span><span class="sxs-lookup"><span data-stu-id="62a51-124">Select **File** > **Options** >  **Advanced**.</span></span>
<span data-ttu-id="62a51-125">Sadaļā **sūtīt un saņemt** atlasiet **nosūtīt uzreiz pēc savienojuma**, un pēc tam izvēlieties **Labi**.</span><span class="sxs-lookup"><span data-stu-id="62a51-125">In the **Send and receive** section, select **Send immediately when connected**, and then choose **OK**.</span></span>
 
<span data-ttu-id="62a51-126">Lai iegūtu pilnīgu informāciju, skatīt:</span><span class="sxs-lookup"><span data-stu-id="62a51-126">For full details see:</span></span>
- [<span data-ttu-id="62a51-127">Video: sūtīt vai izdzēst iestrēdzis e-pastu</span><span class="sxs-lookup"><span data-stu-id="62a51-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="62a51-128">E-pasts paliek mapē Izsūtne līdz jūs manuāli uzsākt sūtīšanas/saņemšanas operāciju programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="62a51-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
