---
title: Identificē IP adrese un klienta audita žurnālos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1367"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: e0119762d2a34bd2b0da827faf55c832e29d8a2b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36539036"
---
# <a name="identify-ip-address-and-client-in-audit-logs"></a><span data-ttu-id="91766-102">Identificē IP adrese un klienta audita žurnālos</span><span class="sxs-lookup"><span data-stu-id="91766-102">Identify IP address and client in audit logs</span></span>

<span data-ttu-id="91766-103">IP adrese, kas atbilst Office 365 lietotāja vai administratora darbība tiek rādīts audita žurnālus.</span><span class="sxs-lookup"><span data-stu-id="91766-103">The IP address that corresponds to an activity by an Office 365 user or administrator is shown in the Audit Logs.</span></span> <span data-ttu-id="91766-104">Klienta informācija arī pieteicies.</span><span class="sxs-lookup"><span data-stu-id="91766-104">The client information is also logged.</span></span> <span data-ttu-id="91766-105">Šeit ir soļi, lai apzinātu šādas informācijas</span><span class="sxs-lookup"><span data-stu-id="91766-105">Here are the steps to identifying such information</span></span>

1. <span data-ttu-id="91766-106">[Office drošības 365 & atbilstību centra](https://protection.office.com/)pieteikties.</span><span class="sxs-lookup"><span data-stu-id="91766-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/).</span></span>

2. <span data-ttu-id="91766-107">Iet uz **meklēšanas** > **audita žurnālu meklēšanas** lapu.</span><span class="sxs-lookup"><span data-stu-id="91766-107">Go to the **Search** > **Audit log search** page.</span></span>

   <span data-ttu-id="91766-108">Ja jūs interesē konkrētas aktivitātes, atlasiet to no **darbību** saraksta.</span><span class="sxs-lookup"><span data-stu-id="91766-108">If you're interested in a specific activity, select it from **Activities** list.</span></span> <span data-ttu-id="91766-109">Ja nav, tad visas darbības, kas tiks atgriezta atlasītā lietotāja (noklusētais uzstādījums).</span><span class="sxs-lookup"><span data-stu-id="91766-109">If not, all activities will be returned for the selected user (default setting).</span></span>

   <span data-ttu-id="91766-110">**Piezīme**: konkrētas darbības var nebūt pieejamas izvēlnē **darbības** ; Tomēr tiem audita vienumi tiks atgriezta, ja **Rādīt rezultātus visām darbībām** ir atlasītās (noklusējuma iestatījums).</span><span class="sxs-lookup"><span data-stu-id="91766-110">**Note**: Certain activities may not be available in the **Activities** menu; however, those audit items will be returned if **Show Results for all activities** is selected (default setting).</span></span>

3. <span data-ttu-id="91766-111">Jānorāda lietotājvārds **lietotāji** laukā, atlasiet atbilstošo datuma diapazonu darbības un pēc tam noklikšķiniet uz **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="91766-111">Specify the username in the **Users** field, select the appropriate date range for the activity, and then click **Search**.</span></span>

<span data-ttu-id="91766-112">Rezultātu, jūs varat redzēt IP adresi kādam šīs darbības rezultātu rūtī.</span><span class="sxs-lookup"><span data-stu-id="91766-112">In the results, you can see the IP address for that activity in the results pane.</span></span> <span data-ttu-id="91766-113">Atlasiet kontroles ierakstu, lai apskatītu detalizētu informāciju **detaļu** flyout (piemēram, klients, lietotāju, kas veic darbību, utt.).</span><span class="sxs-lookup"><span data-stu-id="91766-113">Select the audit record to see detailed information in the **Details** flyout (for example, Client, User that performed action, etc.).</span></span>

<span data-ttu-id="91766-114">Papildinformāciju skatiet sadaļā [atrast IP adresi datoram, ko izmanto, lai piekļūtu kompromitēta kontā](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span><span class="sxs-lookup"><span data-stu-id="91766-114">For more information, see [Finding the IP address of the computer used to access a compromised account](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#finding-the-ip-address-of-the-computer-used-to-access-a-compromised-account).</span></span>
