---
title: Noteiktu dzēšanas ziņu notikumiem audita žurnālos
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1370
ms.assetid: ''
ms.openlocfilehash: 93f8a192af6e689e2b2d04013f35b8da2b69e607
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909381"
---
# <a name="audit-logs-for-deleted-email-messages"></a><span data-ttu-id="de877-102">Audita žurnālos, dzēstie e-pasta ziņojumiem</span><span class="sxs-lookup"><span data-stu-id="de877-102">Audit logs for deleted email messages</span></span>

<span data-ttu-id="de877-103">Sākot ar janvāra 2019, Microsoft ir pagrieziena pastkastes audita pieteikšanās pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="de877-103">Starting in January 2019, Microsoft is turning on mailbox audit logging by default.</span></span> <span data-ttu-id="de877-104">Pretējā gadījumā pārskatīt dzēst ziņu notikumiem konkrētu lietotāju, ir jāiespējo manuāli dzēst darbības revīziju.</span><span class="sxs-lookup"><span data-stu-id="de877-104">Otherwise, to review delete message events for a specific user, you need to manually enable the delete actions for auditing.</span></span> <span data-ttu-id="de877-105">Ja pastkastes audita reģistrēšana ar operatora palīdzību jau bijusi iespējota jūsu uzņēmumam vai noteiktam lietotājam, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="de877-105">If mailbox audit logging is already enabled for your organization or for the specific user, follow the steps below.</span></span>

1. <span data-ttu-id="de877-106">[Office drošības 365 & atbilstību centra](https://protection.office.com/) pieteikties</span><span class="sxs-lookup"><span data-stu-id="de877-106">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="de877-107">Noklikšķiniet uz **meklēšanas un izmeklēšanas** un atlasiet **Audita žurnālu meklēšana**.</span><span class="sxs-lookup"><span data-stu-id="de877-107">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="de877-108">Atlasiet datumu diapazona **sākuma datums** un **beigu datums** laukos.</span><span class="sxs-lookup"><span data-stu-id="de877-108">Select the date range in the **Start date** and **End date** fields.</span></span> <span data-ttu-id="de877-109">Jānorāda lietotājvārds lietotājam, kuru vēlaties izpētīt (lietotājs, kurš Izdzēstie vienumi).</span><span class="sxs-lookup"><span data-stu-id="de877-109">Specify username for the user that you want to investigate (the user who deleted the items).</span></span> <span data-ttu-id="de877-110">**Darbības** lauks atlasiet **Izdzēstie ziņojumi no mapes Izdzēstie vienumi** un **Moved ziņojumus uz mapi Izdzēstie vienumi**.</span><span class="sxs-lookup"><span data-stu-id="de877-110">In the **Activities** field, select **Deleted messages from Deleted Items folder** and **Moved messages to Deleted Items folder**.</span></span>

4. <span data-ttu-id="de877-111">Noklikšķiniet uz **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="de877-111">Click **Search**.</span></span>

<span data-ttu-id="de877-112">Rezultātos atzīmējiet auditācijas ierakstu.</span><span class="sxs-lookup"><span data-stu-id="de877-112">In the results, select an audit record.</span></span> <span data-ttu-id="de877-113">Flyout detaļas, noklikšķiniet uz **Papildinformācija**.</span><span class="sxs-lookup"><span data-stu-id="de877-113">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="de877-114">Papildu informāciju par dzēsto vienumu (piemēram, tēmas rindu un vienums, kad to dzēsa atrašanās vieta) ir rādīts laukā **AffectedItems** .</span><span class="sxs-lookup"><span data-stu-id="de877-114">Additional information about the deleted item (for example, the subject line and the location of the item when it was deleted) is displayed in the **AffectedItems** field.</span></span> <span data-ttu-id="de877-115">**ClientInfoString** īpašuma rādīs, ja programmā Outlook, Outlook web (agrāk pazīstama kā Outlook Web App) vai kādu citu ierīci, radās dzēšanu.</span><span class="sxs-lookup"><span data-stu-id="de877-115">The **ClientInfoString** property will show if the deletion occurred in Outlook, Outlook on the web (formerly known as Outlook Web App), or any other device.</span></span>

<span data-ttu-id="de877-116">Plašāku informāciju skatiet [noteikšana, kas izveido e-pasta pāradresācija uz pastkasti](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span><span class="sxs-lookup"><span data-stu-id="de877-116">For more information, see [Determining who set up email forwarding for a mailbox](https://docs.microsoft.com/office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-deleted-email-items).</span></span>

<span data-ttu-id="de877-117">**Piezīme**: izmantojot funkciju audita žurnāla izdzēsto vienumu nevar izgūt.</span><span class="sxs-lookup"><span data-stu-id="de877-117">**Note**: You can't retrieve deleted items using the audit log feature.</span></span> <span data-ttu-id="de877-118">Lai izgūtu izdzēstos ziņojumus Outlook Web, skatiet [Atkopt izdzēstos vienumus programmā Outlook tīmekļa lietojumprogramma](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span><span class="sxs-lookup"><span data-stu-id="de877-118">To retrieve deleted messages in Outlook on the web, see [Recover deleted items in Outlook Web App](https://support.office.com/article/C3D8FC15-EEEF-4F1C-81DF-E27964B7EDD4).</span></span>
