---
title: Izdzēsto notikumu audita žurnālu lasīšana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3100005"
- "7327"
ms.openlocfilehash: 9739fb1eb8e4f5adf81cd699c851a51176f0429e
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482265"
---
# <a name="read-the-audit-logs-for-deleted-events"></a><span data-ttu-id="02669-102">Izdzēsto notikumu audita žurnālu lasīšana</span><span class="sxs-lookup"><span data-stu-id="02669-102">Read the audit logs for deleted events</span></span>

<span data-ttu-id="02669-103">Tālāk ir aprakstīts, kā to paveikt.</span><span class="sxs-lookup"><span data-stu-id="02669-103">Here's how to do this:</span></span>

1. <span data-ttu-id="02669-104">Dodieties uz [Office 365 drošības & atbilstības centru](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span><span class="sxs-lookup"><span data-stu-id="02669-104">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143).</span></span>
1. <span data-ttu-id="02669-105">Atlasiet **meklēšanas**  >  [**audita žurnālu meklēšana**](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="02669-105">Select **Search** > [**Audit log search**](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>
    > [!NOTE]
    > <span data-ttu-id="02669-106">Ja redzat paziņojumu par to, ka šis līdzeklis ir jāieslēdz, turpiniet to ieslēgt tūlīt.</span><span class="sxs-lookup"><span data-stu-id="02669-106">If you see a notice that you need to turn on the feature, go ahead and turn it on now.</span></span> <span data-ttu-id="02669-107">Ja līdzeklis nav ieslēgts, meklēšanas rezultātos nevarēs paņemt datus no iepriekšējiem datumiem.</span><span class="sxs-lookup"><span data-stu-id="02669-107">If the feature isn't turned on, search results won't be able to pull data from previous dates.</span></span>
1. <span data-ttu-id="02669-108">Atlasiet **darbības** un pēc tam atrodiet **Exchange pastkastes darbības**.</span><span class="sxs-lookup"><span data-stu-id="02669-108">Select **Activities**, and then find **Exchange mailbox activities**.</span></span> <span data-ttu-id="02669-109">Atlasiet mapi Izdzēstie **vienumi** un **pārcēla ziņojumus uz mapes Izdzēstie vienumi** opcijām.</span><span class="sxs-lookup"><span data-stu-id="02669-109">Select the **Deleted messages from Deleted Items** folder and **Moved messages to Deleted Items** folder options.</span></span> <span data-ttu-id="02669-110">Kad tas ir paveikts, noklikšķiniet ārpus rūts, lai minimizētu rūti **aktivitātes** .</span><span class="sxs-lookup"><span data-stu-id="02669-110">When you're done, click outside of the pane to minimize the **Activities** pane.</span></span>
1. <span data-ttu-id="02669-111">Norādiet datumu diapazonu un pēc tam lodziņā **lietotāji** atlasiet tā lietotāja lietotājvārdu, kuru vēlaties izpētīt.</span><span class="sxs-lookup"><span data-stu-id="02669-111">Specify the date range, and then in the **Users** box, select the username for the user you want to investigate.</span></span> <span data-ttu-id="02669-112">Vienlaikus varat atlasīt vairākus lietotājus.</span><span class="sxs-lookup"><span data-stu-id="02669-112">You can select more than one user at a time.</span></span>
1. <span data-ttu-id="02669-113">Atlasiet **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="02669-113">Select **Search**.</span></span> <span data-ttu-id="02669-114">Darbības būs redzamas sadaļā **rezultāti**.</span><span class="sxs-lookup"><span data-stu-id="02669-114">The activities appear under **Results**.</span></span>
1. <span data-ttu-id="02669-115">Lai skatītu detalizētu informāciju, atlasiet aktivitāti un pēc tam atlasiet **Papildinformācija**.</span><span class="sxs-lookup"><span data-stu-id="02669-115">To view the details, select an activity, and then select **More Information**.</span></span> <span data-ttu-id="02669-116">Papildinformācija par izdzēsto vienumu, piemēram, tēmas rindiņu un vienuma atrašanās vietu pēc izdzēšanas, tiek parādīta laukā **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="02669-116">Additional information about the deleted item, such as the subject line and the location of the item when it was deleted, is displayed in the **AffectedItems** field.</span></span>
    > [!NOTE]
    > <span data-ttu-id="02669-117">Izdzēstos vienumus nevar atjaunot, izmantojot audita žurnālu līdzekli.</span><span class="sxs-lookup"><span data-stu-id="02669-117">You can't restore deleted items using the audit log feature.</span></span> <span data-ttu-id="02669-118">Lai atjaunotu izdzēstos vienumus, skatiet rakstu [izdzēsto vienumu atkopšana programmā Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span><span class="sxs-lookup"><span data-stu-id="02669-118">To restore deleted items, see [Recover deleted items or email in Outlook Web App](https://go.microsoft.com/fwlink/?linkid=2103759).</span></span>

<span data-ttu-id="02669-119">Lai uzzinātu vairāk, skatiet rakstu [meklēšana Office 365 audita žurnālu, lai novērstu raksturīgākos scenārijus](https://go.microsoft.com/fwlink/?linkid=2103944).</span><span class="sxs-lookup"><span data-stu-id="02669-119">To learn more, see [Search the Office 365 audit log to troubleshoot common scenarios](https://go.microsoft.com/fwlink/?linkid=2103944).</span></span>
