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
- "9002385"
- "4645"
ms.openlocfilehash: 35fe9ae76ca77faa43796b288af09be8525cb6df
ms.sourcegitcommit: 929f8accdca2b8e5be170e0fc8edd527581453d4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/12/2020
ms.locfileid: "43232637"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="9e610-102">Labot izsūtnē iestrēgušos ziņojumus</span><span class="sxs-lookup"><span data-stu-id="9e610-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="9e610-103">Ieteicams sākt, palaižot scenāriju ["man ir problēmas, nosūtot, saņemot vai atrodot e-pasta ziņojumus"](https://aka.ms/SaRA-OutlookSendReceive) no [Microsoft Support un atkopšanas palīgs](https://diagnostics.office.com/#/) rīks attiecīgajā datorā.</span><span class="sxs-lookup"><span data-stu-id="9e610-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool on the affected machine.</span></span>

<span data-ttu-id="9e610-104">Kad ziņojums tiek iestrēdzis izsūtnē, Visdrīzāk iemesls ir liels pielikumu vai opciju "nosūtīt uzreiz pēc savienojuma" nav iespējots.</span><span class="sxs-lookup"><span data-stu-id="9e610-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="9e610-105">**Noņemiet lielo pielikumu**</span><span class="sxs-lookup"><span data-stu-id="9e610-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="9e610-106">Noklikšķiniet uz **Nosūtīt/saņemt** > **darbu bezsaistē**.</span><span class="sxs-lookup"><span data-stu-id="9e610-106">Click **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="9e610-107">Navigācijas rūtī noklikšķiniet uz **Izsūtne**.</span><span class="sxs-lookup"><span data-stu-id="9e610-107">In the navigation pane, click **Outbox**.</span></span> <span data-ttu-id="9e610-108">No šejienes jūs varat:</span><span class="sxs-lookup"><span data-stu-id="9e610-108">From here, you can:</span></span> 
    - <span data-ttu-id="9e610-109">Izdzēsiet ziņu.</span><span class="sxs-lookup"><span data-stu-id="9e610-109">Delete the message.</span></span> <span data-ttu-id="9e610-110">Vienkārši atlasiet to un noklikšķiniet uz **Dzēst**.</span><span class="sxs-lookup"><span data-stu-id="9e610-110">Just select it and click **Delete**.</span></span>
    - <span data-ttu-id="9e610-111">Velciet ziņojumu uz **melnrakstu mapi**, veiciet dubultklikšķi, lai atvērtu ziņojumu, un izdzēsiet pielikumu (noklikšķiniet uz tā un noklikšķiniet uz **Dzēst**).</span><span class="sxs-lookup"><span data-stu-id="9e610-111">Drag the message to your **drafts folder**, double-click to open the message, and delete the attachment (click it and click **Delete**).</span></span>
3. <span data-ttu-id="9e610-112">Ja tiek parādīts kļūdas ziņojums programma Outlook mēģina nosūtīt ziņojumu, aizveriet programmu Outlook.</span><span class="sxs-lookup"><span data-stu-id="9e610-112">If an error tells you Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="9e610-113">Tas var aizņemt kādu brīdi, lai izietu.</span><span class="sxs-lookup"><span data-stu-id="9e610-113">It may take a few moments to exit.</span></span> <span data-ttu-id="9e610-114">Ja programma Outlook netiek aizvērta, nospiediet taustiņu **kombināciju CTRL + ALT + DELETE** un noklikšķiniet uz **startēt uzdevumu pārvaldnieku**.</span><span class="sxs-lookup"><span data-stu-id="9e610-114">If Outlook doesn't close, press **Ctrl+Alt+Delete** and click **Start Task Manager**.</span></span> <span data-ttu-id="9e610-115">Uzdevumu pārvaldniekā atlasiet cilni **procesi** , ritiniet uz leju līdz Outlook. exe un noklikšķiniet uz **Beigt procesu**.</span><span class="sxs-lookup"><span data-stu-id="9e610-115">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and click **End Process**.</span></span>
4. <span data-ttu-id="9e610-116">Pēc Outlook aizvēršanas restartējiet Outlook un atkārtojiet 2-3.</span><span class="sxs-lookup"><span data-stu-id="9e610-116">After Outlook closes, restart Outlook and repeat steps 2-3.</span></span> 
5. <span data-ttu-id="9e610-117">Pēc pielikuma noņemšanas noklikšķiniet uz **Nosūtīt/saņemt** > **darbu bezsaistē** , lai atceltu pogas atlasi un atsāktu darbu tiešsaistē.</span><span class="sxs-lookup"><span data-stu-id="9e610-117">After you remove the attachment, click **Send / Receive** > **Work Offline** to deselect the button and to resume working online.</span></span> 

<span data-ttu-id="9e610-118">Ziņojumi tiek iestrēguši arī izsūtnē, kad noklikšķināt uz **nosūtīt**, bet nav izveidots savienojums.</span><span class="sxs-lookup"><span data-stu-id="9e610-118">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="9e610-119">Noklikšķiniet uz **Nosūtīt/saņemt** un paskatieties uz pogu **strādāt bezsaistē** .</span><span class="sxs-lookup"><span data-stu-id="9e610-119">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="9e610-120">Ja tas ir zils, jūs esat atvienots.</span><span class="sxs-lookup"><span data-stu-id="9e610-120">If it's blue, you're disconnected.</span></span> <span data-ttu-id="9e610-121">Noklikšķiniet uz tās, lai savienotu (poga kļūst balta) un noklikšķiniet uz **Sūtīt visu**.</span><span class="sxs-lookup"><span data-stu-id="9e610-121">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="9e610-122">**Iespējot nosūtīšanu uzreiz pēc savienojuma**</span><span class="sxs-lookup"><span data-stu-id="9e610-122">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="9e610-123">Cilni failu, noklikšķiniet uz **Opcijas**.</span><span class="sxs-lookup"><span data-stu-id="9e610-123">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="9e610-124">Outlook opcijas dialoglodziņā noklikšķiniet uz **papildu**.</span><span class="sxs-lookup"><span data-stu-id="9e610-124">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="9e610-125">Sadaļā nosūtīt un saņemt noklikšķiniet, lai iespējotu **nosūtīt uzreiz pēc savienojuma**.</span><span class="sxs-lookup"><span data-stu-id="9e610-125">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="9e610-126">Noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="9e610-126">Click **OK**.</span></span>
 
<span data-ttu-id="9e610-127">Lai iegūtu pilnīgu informāciju, skatiet:</span><span class="sxs-lookup"><span data-stu-id="9e610-127">For full details, see:</span></span>
- [<span data-ttu-id="9e610-128">Video: sūtīt vai izdzēst iestrēdzis e-pastu</span><span class="sxs-lookup"><span data-stu-id="9e610-128">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="9e610-129">E-pasts paliek mapē Izsūtne līdz jūs manuāli uzsākt sūtīšanas/saņemšanas operāciju programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="9e610-129">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
