---
title: IP adreses un klienta identificēšana audita žurnālos
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
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 295418f3c433df2ba1004f4bec4377c68e6bb155
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47668317"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="e3369-102">IP adreses un klienta identificēšana audita žurnālos</span><span class="sxs-lookup"><span data-stu-id="e3369-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="e3369-103">Audita žurnālos tiek rādīta IP adrese, kas atbilst aktivitātei, ko nodrošina Microsoft 365 lietotājs vai administrators.</span><span class="sxs-lookup"><span data-stu-id="e3369-103">The IP address that corresponds to an activity by a Microsoft 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="e3369-104">Tiek reģistrēta arī klienta informācija.</span><span class="sxs-lookup"><span data-stu-id="e3369-104">The client information is also logged.</span></span> <span data-ttu-id="e3369-105">Tālāk norādītas darbības, kas jāveic, lai noteiktu šādu informāciju</span><span class="sxs-lookup"><span data-stu-id="e3369-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="e3369-106">Piesakieties [Microsoft 365 drošības & atbilstības centrā](https://protection.office.com/).</span><span class="sxs-lookup"><span data-stu-id="e3369-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="e3369-107">Dodieties **uz meklēšanas**  >  **audita žurnālu meklēšanas** lapā.</span><span class="sxs-lookup"><span data-stu-id="e3369-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="e3369-108">Ja esat ieinteresēts noteiktā aktivitātē, atlasiet to sarakstā **aktivitātes** .</span><span class="sxs-lookup"><span data-stu-id="e3369-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="e3369-109">Ja tā nav, visi darbi tiks atgriezti atlasītajam lietotājam (noklusējuma iestatījums).</span><span class="sxs-lookup"><span data-stu-id="e3369-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="e3369-110">**Piezīme**: noteiktas darbības, iespējams, nav pieejamas izvēlnē **darbības** ; taču šie audita vienumi tiek atgriezti, ja ir atlasīts **Rādīt rezultātus visām darbībām** (noklusējuma iestatījums).</span><span class="sxs-lookup"><span data-stu-id="e3369-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="e3369-111">Laukā **lietotāji** norādiet lietotājvārdu, atlasiet atbilstīgo datumu diapazonu darbībai un pēc tam noklikšķiniet uz **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="e3369-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="e3369-112">Rezultātos varat redzēt šīs darbības IP adresi rezultātu rūtī.</span><span class="sxs-lookup"><span data-stu-id="e3369-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="e3369-113">Atlasiet audita ierakstu, **lai detalizētās** informācijas sadaļā skatītu detalizētu informāciju, piemēram, klients, lietotājs, kas veicis darbību utt.).</span><span class="sxs-lookup"><span data-stu-id="e3369-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="e3369-114">Papildinformāciju skatiet rakstā tā [datora IP adreses atrašana, ko izmanto, lai piekļūtu kompromitētajam kontam](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="e3369-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#find-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
