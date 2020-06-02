---
title: Identificētu dzēst ziņojumu notikumus audita žurnālos
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: 641c0216491186aeb423a13854c6b39ee005e5df
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44508995"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="f4b2a-102">Audita žurnālus dzēstiem e-pasta ziņojumiem</span><span class="sxs-lookup"><span data-stu-id="f4b2a-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="f4b2a-103">Sākot ar 2019 janvārī, Microsoft ieslēdzot pastkastes audita reģistrēšanu pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="f4b2a-104">Pretējā gadījumā, lai pārskatītu dzēst ziņojumu notikumus noteiktam lietotājam, ir manuāli jāiespējo dzēšanas darbības auditēšanai.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="f4b2a-105">Ja pastkastes audita reģistrēšana jau ir iespējota jūsu organizācijai vai noteiktam lietotājam, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="f4b2a-106">Pieteikšanās [Microsoft 365 drošības & atbilstības centrs](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="f4b2a-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="f4b2a-107">Noklikšķiniet uz **meklēšana un izmeklēšana** un atlasiet **audita žurnāla meklēšana**.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="f4b2a-108">Laukā **sākuma datums** un **beigu datums** atlasiet datumu diapazonu.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="f4b2a-109">Norādiet tā lietotāja lietotājvārdu, kuru vēlaties izpētīt (lietotājs, kurš izdzēsis vienumus).</span><span class="sxs-lookup"><span data-stu-id="f4b2a-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="f4b2a-110">Laukā **darbības** atlasiet **Izdzēstie ziņojumi no mapes Izdzēstie vienumi** un **mapē ziņojumi pārvietoti uz mapi Izdzēstie vienumi**.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="f4b2a-111">Noklikšķiniet uz **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-111">Click **Search**.</span></span>

<span data-ttu-id="f4b2a-112">Rezultātos atlasiet audita ierakstu.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-112">In the results, select an audit record.</span></span> <span data-ttu-id="f4b2a-113">Detalizētās informācijas izlidošanas noklikšķiniet uz **Papildinformācija**.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="f4b2a-114">Laukā **Affecteditems** tiek parādīta papildinformācija par izdzēsto elementu (piemēram, tēmas rindiņa un vienuma atrašanās vieta, kad tā tika izdzēsta).</span><span class="sxs-lookup"><span data-stu-id="f4b2a-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="f4b2a-115">Rekvizītā **Clientinfostring** tiks parādīts, ja programmā Outlook, Outlook Web (iepriekš pazīstams kā Outlook Web App) vai jebkuras citas ierīces dzēšanu.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="f4b2a-116">Lai iegūtu papildinformāciju, skatiet [noteikt, kurš ir iestatījis e-pasta pārsūtīšanu pastkastei](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="f4b2a-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="f4b2a-117">**Piezīme**: nevar izgūt izdzēstos vienumus, izmantojot audita žurnāla līdzekli.</span><span class="sxs-lookup"><span data-stu-id="f4b2a-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="f4b2a-118">Lai izgūtu izdzēstos ziņojumus programmā Outlook tīmeklī, skatiet sadaļu [izdzēsto vienumu atkopšana programmā Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="f4b2a-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
