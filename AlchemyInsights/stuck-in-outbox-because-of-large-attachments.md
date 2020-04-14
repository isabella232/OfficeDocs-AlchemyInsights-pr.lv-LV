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
ms.openlocfilehash: 4f69de167dc51961fa7cf71b4d73ca7ee3ed4d55
ms.sourcegitcommit: 57fb994ddd3854d06faa67680c971b003b06bf83
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/13/2020
ms.locfileid: "43241259"
---
# <a name="fix-messages-that-are-stuck-in-the-outbox"></a><span data-ttu-id="b8742-102">Labot izsūtnē iestrēgušos ziņojumus</span><span class="sxs-lookup"><span data-stu-id="b8742-102">Fix messages that are stuck in the Outbox</span></span>

<span data-ttu-id="b8742-103">Ieteicams sākt, palaižot scenāriju ["man ir problēmas ar e-pasta ziņojumu sūtīšanu, saņemšanu vai atrašanu"](https://aka.ms/SaRA-OutlookSendReceive) no [Microsoft atbalsta un atkopšanas palīga](https://diagnostics.office.com/#/) rīka.</span><span class="sxs-lookup"><span data-stu-id="b8742-103">We recommend that you start by running the scenario ["I'm having problems sending, receiving, or finding email messages"](https://aka.ms/SaRA-OutlookSendReceive) from the [Microsoft Support and Recovery Assistant](https://diagnostics.office.com/#/) tool.</span></span>

<span data-ttu-id="b8742-104">Kad ziņojums tiek iestrēdzis izsūtnē, Visdrīzāk iemesls ir liels pielikumu vai opciju "nosūtīt uzreiz pēc savienojuma" nav iespējots.</span><span class="sxs-lookup"><span data-stu-id="b8742-104">When a message gets stuck in your Outbox, the most likely cause is a large attachment or the option "Send immediately when connected" is not enabled.</span></span>

<span data-ttu-id="b8742-105">**Noņemiet lielo pielikumu**</span><span class="sxs-lookup"><span data-stu-id="b8742-105">**Remove the large attachment**</span></span>

1. <span data-ttu-id="b8742-106">Programmā Outlook atlasiet **Nosūtīt/saņemt** > **darbu bezsaistē**.</span><span class="sxs-lookup"><span data-stu-id="b8742-106">In Outlook, select **Send / Receive** > **Work Offline**.</span></span> 
2. <span data-ttu-id="b8742-107">Navigācijas rūtī atlasiet **Izsūtne**.</span><span class="sxs-lookup"><span data-stu-id="b8742-107">In the navigation pane, select **Outbox**.</span></span> <span data-ttu-id="b8742-108">No šejienes jūs varat:</span><span class="sxs-lookup"><span data-stu-id="b8742-108">From here, you can:</span></span> 
    - <span data-ttu-id="b8742-109">Izdzēsiet ziņu (atlasiet to un pēc tam atlasiet **Dzēst**).</span><span class="sxs-lookup"><span data-stu-id="b8742-109">Delete the message (select it and then select **Delete**).</span></span>
    - <span data-ttu-id="b8742-110">Velciet ziņojumu uz melnrakstu mapi, veiciet dubultklikšķi, lai to atvērtu, un noņemiet pielikumu atlasiet to un pēc tam atlasiet **Dzēst**).</span><span class="sxs-lookup"><span data-stu-id="b8742-110">Drag the message to your Drafts folder, double-click to open it, and remove the attachment select it and then select **Delete**).</span></span>
3. <span data-ttu-id="b8742-111">Ja tiek parādīts kļūdas ziņojums, kurā teikts, ka programma Outlook mēģina pārraidīt ziņojumu, aizveriet programmu Outlook.</span><span class="sxs-lookup"><span data-stu-id="b8742-111">If you receive an error that says Outlook is trying to transmit the message, close Outlook.</span></span> <span data-ttu-id="b8742-112">Tas var aizņemt kādu brīdi, lai izietu.</span><span class="sxs-lookup"><span data-stu-id="b8742-112">It may take a few moments to exit.</span></span> <span data-ttu-id="b8742-113">Ja programma Outlook netiek aizvērta, nospiediet taustiņu kombināciju CTRL + ALT + DELETE un atlasiet **startēt uzdevumu pārvaldnieku**.</span><span class="sxs-lookup"><span data-stu-id="b8742-113">If Outlook doesn't close, press Ctrl+Alt+Delete and select **Start Task Manager**.</span></span> <span data-ttu-id="b8742-114">Uzdevumu pārvaldniekā atlasiet cilni **procesi** , ritiniet uz leju līdz Outlook. exe un atlasiet **Beigt procesu**.</span><span class="sxs-lookup"><span data-stu-id="b8742-114">In Task Manager, select the **Processes** tab, scroll down to outlook.exe, and select **End Process**.</span></span>
4. <span data-ttu-id="b8742-115">Kad programma Outlook tiek aizvērta, restartējiet to un atkārtojiet 2. un 3. darbību.</span><span class="sxs-lookup"><span data-stu-id="b8742-115">After Outlook closes, restart it and repeat steps 2 and 3.</span></span> 
5. <span data-ttu-id="b8742-116">Pēc pielikuma noņemšanas noklikšķiniet uz **Nosūtīt/saņemt** > **darbu bezsaistē** , lai atsāktu darbu tiešsaistē.</span><span class="sxs-lookup"><span data-stu-id="b8742-116">After you remove the attachment, click **Send / Receive** > **Work Offline** to resume working online.</span></span> 

<span data-ttu-id="b8742-117">Ziņojumi tiek iestrēguši arī izsūtnē, kad noklikšķināt uz **nosūtīt**, bet nav izveidots savienojums.</span><span class="sxs-lookup"><span data-stu-id="b8742-117">Messages also get stuck in the Outbox when you click **Send**, but you are not connected.</span></span> <span data-ttu-id="b8742-118">Noklikšķiniet uz **Nosūtīt/saņemt** un paskatieties uz pogu **strādāt bezsaistē** .</span><span class="sxs-lookup"><span data-stu-id="b8742-118">Click **Send / Receive** and look at the **Work Offline** button.</span></span> <span data-ttu-id="b8742-119">Ja tas ir zils, jūs esat atvienots.</span><span class="sxs-lookup"><span data-stu-id="b8742-119">If it's blue, you're disconnected.</span></span> <span data-ttu-id="b8742-120">Noklikšķiniet uz tās, lai savienotu (poga kļūst balta) un noklikšķiniet uz **Sūtīt visu**.</span><span class="sxs-lookup"><span data-stu-id="b8742-120">Click it to connect (the button turns white) and click **Send All**.</span></span>
 
<span data-ttu-id="b8742-121">**Iespējot nosūtīšanu uzreiz pēc savienojuma**</span><span class="sxs-lookup"><span data-stu-id="b8742-121">**Enable Send immediately when connected**</span></span>
 
1. <span data-ttu-id="b8742-122">Cilni failu, noklikšķiniet uz **Opcijas**.</span><span class="sxs-lookup"><span data-stu-id="b8742-122">On the File tab, click **Options**.</span></span>

2. <span data-ttu-id="b8742-123">Outlook opcijas dialoglodziņā noklikšķiniet uz **papildu**.</span><span class="sxs-lookup"><span data-stu-id="b8742-123">In the Outlook Options dialog box, click **Advanced**.</span></span>

3. <span data-ttu-id="b8742-124">Sadaļā nosūtīt un saņemt noklikšķiniet, lai iespējotu **nosūtīt uzreiz pēc savienojuma**.</span><span class="sxs-lookup"><span data-stu-id="b8742-124">In the Send and receive section, click to enable **Send immediately when connected**.</span></span> <span data-ttu-id="b8742-125">Noklikšķiniet uz **Labi**.</span><span class="sxs-lookup"><span data-stu-id="b8742-125">Click **OK**.</span></span>
 
<span data-ttu-id="b8742-126">Lai iegūtu pilnīgu informāciju, skatiet:</span><span class="sxs-lookup"><span data-stu-id="b8742-126">For full details, see:</span></span>
- [<span data-ttu-id="b8742-127">Video: sūtīt vai izdzēst iestrēdzis e-pastu</span><span class="sxs-lookup"><span data-stu-id="b8742-127">Video: Send or delete a stuck email</span></span>](https://support.office.com/article/Video-Send-or-delete-an-email-stuck-in-your-outbox-26d5d34a-4e5f-444a-a9e8-44db04a94dec) 
- [<span data-ttu-id="b8742-128">E-pasts paliek mapē Izsūtne līdz jūs manuāli uzsākt sūtīšanas/saņemšanas operāciju programmā Outlook</span><span class="sxs-lookup"><span data-stu-id="b8742-128">Email stays in the Outbox folder until you manually initiate a send/receive operation in Outlook</span></span>](https://support.microsoft.com/help/2797572/email-stays-in-the-outbox-folder-until-you-manually-initiate-a-send-re)
