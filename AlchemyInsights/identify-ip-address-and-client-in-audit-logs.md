---
title: Identificēt IP adresi un klientu audita žurnālos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 80b652eb65612093252dee226a19ec74bc035faa
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508923"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="3f6e1-102">Identificēt IP adresi un klientu audita žurnālos</span><span class="sxs-lookup"><span data-stu-id="3f6e1-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="3f6e1-103">IP adrese, kas atbilst Microsoft 365 lietotāja vai administratora darbībai, tiek rādīta audita žurnālos.</span><span class="sxs-lookup"><span data-stu-id="3f6e1-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="3f6e1-104">Klienta informācija arī tiek reģistrēta.</span><span class="sxs-lookup"><span data-stu-id="3f6e1-104">The client information is also logged.</span></span> <span data-ttu-id="3f6e1-105">Tālāk ir norādītas šādas informācijas identificēšanas darbības.</span><span class="sxs-lookup"><span data-stu-id="3f6e1-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="3f6e1-106">Piesakieties [Microsoft 365 drošības & atbilstības centrā](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="3f6e1-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="3f6e1-107">Pārejiet **uz meklēšanas**  >  **audita žurnāla meklēšanas** lapu.</span><span class="sxs-lookup"><span data-stu-id="3f6e1-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="3f6e1-108">Ja jūs interesē konkrēta aktivitāte, atlasiet to sarakstā **aktivitātes** .</span><span class="sxs-lookup"><span data-stu-id="3f6e1-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="3f6e1-109">Ja tā nav, visas darbības tiks atgrieztas atlasītajam lietotājam (noklusējuma iestatījums).</span><span class="sxs-lookup"><span data-stu-id="3f6e1-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="3f6e1-110">**Piezīme**: dažas darbības var nebūt pieejamas izvēlnē **aktivitātes** ; Tomēr šie audita vienumi tiks atgriezti, ja ir atlasīts **Rādīt rezultātus visām darbībām** (noklusējuma iestatījums).</span><span class="sxs-lookup"><span data-stu-id="3f6e1-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="3f6e1-111">Norādiet lietotājvārdu laukā **lietotāji** , atlasiet darbībai atbilstošo datumu diapazonu un pēc tam noklikšķiniet uz **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="3f6e1-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="3f6e1-112">Rezultātu rūtī varat redzēt minētās aktivitātes IP adresi.</span><span class="sxs-lookup"><span data-stu-id="3f6e1-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="3f6e1-113">Atlasiet audita ierakstu, **lai detalizēti skatītu detalizētu informāciju izlidošanas vietā** (piemēram, klients, lietotājs, kas veicis darbību utt.).</span><span class="sxs-lookup"><span data-stu-id="3f6e1-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="3f6e1-114">Papildinformāciju skatiet sadaļā [tā datora IP adreses atrašana, kas tika izmantots, lai piekļūtu apdraudējumam izmantotam kontam](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="3f6e1-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
