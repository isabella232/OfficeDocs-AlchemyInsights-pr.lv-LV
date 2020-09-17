---
title: Iesūtnes kārtulas darbību noteikšana audita žurnālos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1368"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 3de6fcde6dc649cb77077d469cc66d4003e0c890
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47779058"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="7e673-102">Iesūtnes kārtulas darbību noteikšana audita žurnālos</span><span class="sxs-lookup"><span data-stu-id="7e673-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="7e673-103">Varat izmantot audita žurnālu meklēšanu Microsoft 365 drošības & atbilstības centrā, lai skatītu iesūtnes kārtulu notikumus (izveidot, modificēt un dzēst iesūtnes kārtulas).</span><span class="sxs-lookup"><span data-stu-id="7e673-103">You can use audit log search in the Microsoft 365 Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="7e673-104">Piesakieties [Microsoft 365 drošības & atbilstības centrā](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="7e673-104">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="7e673-105">Dodieties **uz meklēšanas**  >  **audita žurnālu meklēšanas** lapā.</span><span class="sxs-lookup"><span data-stu-id="7e673-105">Go to the **Search** > **Audit log search** page.</span></span>

3. <span data-ttu-id="7e673-106">Atlasiet datumu diapazonu lauku **sākuma datums** un **beigšanas datums** .</span><span class="sxs-lookup"><span data-stu-id="7e673-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="7e673-107">Sadaļā **Exchange pastkastes darbības**pārbaudiet, vai laukā **aktivitātes** ir iestatīta opcija **Jauns-InboxRule izveidot/modificēt/iespējot/atspējot iesūtnes kārtulu**.</span><span class="sxs-lookup"><span data-stu-id="7e673-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="7e673-108">Noklikšķiniet uz **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="7e673-108">Click **Search**.</span></span>

<span data-ttu-id="7e673-109">Rezultātos atlasiet audita ierakstu.</span><span class="sxs-lookup"><span data-stu-id="7e673-109">In the results, select an audit record.</span></span> <span data-ttu-id="7e673-110">Detalizētas informācijas izlidošanas sarakstā noklikšķiniet uz **Papildinformācija**.</span><span class="sxs-lookup"><span data-stu-id="7e673-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="7e673-111">Informācija par iesūtnes kārtulas iestatījumiem tiek parādīta laukā **Parametri** .</span><span class="sxs-lookup"><span data-stu-id="7e673-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="7e673-112">Papildinformāciju skatiet rakstā kā [noteikt, vai lietotājs ir izveidojis iesūtnes kārtulu](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="7e673-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
