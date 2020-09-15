---
title: Dzēst ziņojuma notikumu noskaidrošana audita žurnālos
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
- "1370"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: bc78076706aee15a3133c4b1a89064591f790b58
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47696520"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="d50fb-102">Izdzēsto e-pasta ziņojumu audita žurnāli</span><span class="sxs-lookup"><span data-stu-id="d50fb-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="d50fb-103">Sākot ar 2019. janvāri, Microsoft pēc noklusējuma ieslēdz pastkastes audita reģistrēšanu.</span><span class="sxs-lookup"><span data-stu-id="d50fb-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="d50fb-104">Pretējā gadījumā, lai pārskatītu dzēst ziņojuma notikumus konkrētam lietotājam, ir manuāli jāiespējo dzēšanas darbības auditēšanai.</span><span class="sxs-lookup"><span data-stu-id="d50fb-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="d50fb-105">Ja jums jau ir iespējota pastkastes audita reģistrēšana jūsu organizācijai vai konkrētam lietotājam, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="d50fb-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="d50fb-106">Piesakieties [Microsoft 365 drošības & atbilstības centrā](https://protection.office.com/)</span><span class="sxs-lookup"><span data-stu-id="d50fb-106">Log in to the [Microsoft 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="d50fb-107">Noklikšķiniet uz **meklēšana un izpēte** un atlasiet **audita žurnālu meklēšana**.</span><span class="sxs-lookup"><span data-stu-id="d50fb-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="d50fb-108">Atlasiet datumu diapazonu lauku **sākuma datums** un **beigšanas datums** .</span><span class="sxs-lookup"><span data-stu-id="d50fb-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="d50fb-109">Norādiet tā lietotāja lietotājvārdu, kuru vēlaties izpētīt (lietotāju, kurš izdzēsis šos vienumus).</span><span class="sxs-lookup"><span data-stu-id="d50fb-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="d50fb-110">Laukā **aktivitātes** atlasiet **Izdzēstie ziņojumi no mapes** Izdzēstie vienumi un **pārvietoti ziņojumi uz mapi Izdzēstie vienumi**.</span><span class="sxs-lookup"><span data-stu-id="d50fb-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="d50fb-111">Noklikšķiniet uz **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="d50fb-111">Click **Search**.</span></span>

<span data-ttu-id="d50fb-112">Rezultātos atlasiet audita ierakstu.</span><span class="sxs-lookup"><span data-stu-id="d50fb-112">In the results, select an audit record.</span></span> <span data-ttu-id="d50fb-113">Detalizētas informācijas izlidošanas sarakstā noklikšķiniet uz **Papildinformācija**.</span><span class="sxs-lookup"><span data-stu-id="d50fb-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="d50fb-114">Papildinformāciju par izdzēsto vienumu (piemēram, tēmas rindiņu un vienuma atrašanās vietu, kad tas tika izdzēsts) tiek parādīta laukā **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="d50fb-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="d50fb-115">Rekvizīts **ClientInfoString** tiek parādīts, ja dzēšana notiek programmā Outlook, Outlook tīmeklī (iepriekš zināma kā Outlook Web App) vai jebkura cita ierīce.</span><span class="sxs-lookup"><span data-stu-id="d50fb-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="d50fb-116">Papildinformāciju skatiet rakstā [e-pasta pārsūtīšanas iestatīšana pastkastei](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="d50fb-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/microsoft-365/compliance/auditing-troubleshooting-scenarios#determine-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="d50fb-117">**Piezīme**. jūs nevarat izgūt izdzēstos vienumus, izmantojot audita žurnālu līdzekli.</span><span class="sxs-lookup"><span data-stu-id="d50fb-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="d50fb-118">Lai izdzēstos ziņojumus izgūtu programmā Outlook tīmeklī, skatiet rakstu [izdzēsto vienumu atkopšana programmā Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="d50fb-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
