---
title: Noteiktu iesūtnes kārtulas darbību audita žurnālos
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1368
ms.assetid: ''
ms.openlocfilehash: 9339d9c58056f568dc994b75bffe39f2c8bbdd34
ms.sourcegitcommit: ffe2f489b1ac3aae62aa784c959da6a41c3261eb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/17/2019
ms.locfileid: "31909382"
---
# <a name="identify-inbox-rule-activity-in-audit-logs"></a><span data-ttu-id="fe8bf-102">Noteiktu iesūtnes kārtulas darbību audita žurnālos</span><span class="sxs-lookup"><span data-stu-id="fe8bf-102">Identify inbox rule activity in audit logs</span></span>

<span data-ttu-id="fe8bf-103">Audita žurnālu meklēšana, & drošības ievērošanu centrs var izmantot, lai skatītu iesūtnes kārtulu notikumi (izveidot, modificēt un dzēst iesūtnes kārtulas).</span><span class="sxs-lookup"><span data-stu-id="fe8bf-103">You can use audit log search in the Security & Compliance Center to view inbox rule events (creating, modifying, and deleting inbox rules).</span></span>

1. <span data-ttu-id="fe8bf-104">[Office drošības 365 & atbilstību centra](https://protection.office.com/) pieteikties</span><span class="sxs-lookup"><span data-stu-id="fe8bf-104">Log in to the [Office 365 Security & Compliance Center](https://protection.office.com/)</span></span>

2. <span data-ttu-id="fe8bf-105">Noklikšķiniet uz **meklēšanas un izmeklēšanas** un atlasiet **Audita žurnālu meklēšana**.</span><span class="sxs-lookup"><span data-stu-id="fe8bf-105">Click **Search and Investigation** and select **Audit Log Search**.</span></span>

3. <span data-ttu-id="fe8bf-106">Atlasiet datumu diapazona **sākuma datums** un **beigu datums** laukos.</span><span class="sxs-lookup"><span data-stu-id="fe8bf-106">Select the date range in the **Start date** and **End date** fields.</span></span>

4. <span data-ttu-id="fe8bf-107">**Exchange pastkastes darbību**, pārbaudīt **darbības** lauks ir iestatīts kā **Jauns-InboxRule izveidot/mainīt/iespējot/atspējot iesūtnes kārtulu**.</span><span class="sxs-lookup"><span data-stu-id="fe8bf-107">Under **Exchange Mailbox Activities**, verify the **Activities** field is set to **New-InboxRule Create/modify/enable/disable inbox rule**.</span></span>

5. <span data-ttu-id="fe8bf-108">Noklikšķiniet uz **Meklēt**.</span><span class="sxs-lookup"><span data-stu-id="fe8bf-108">Click **Search**.</span></span>

<span data-ttu-id="fe8bf-109">Rezultātos atzīmējiet auditācijas ierakstu.</span><span class="sxs-lookup"><span data-stu-id="fe8bf-109">In the results, select an audit record.</span></span> <span data-ttu-id="fe8bf-110">Flyout detaļas, noklikšķiniet uz **Papildinformācija**.</span><span class="sxs-lookup"><span data-stu-id="fe8bf-110">In the details flyout, click **More Information**.</span></span> <span data-ttu-id="fe8bf-111">Papildinformāciju par iesūtnes kārtulu iestatījumiem tiek rādīta laukā **Parametri** .</span><span class="sxs-lookup"><span data-stu-id="fe8bf-111">Information about the inbox rule settings is displayed in the **Parameters** field.</span></span>

<span data-ttu-id="fe8bf-112">Plašāku informāciju skatiet [noteikšana, ja lietotājs izveidojis iesūtnes kārtulu](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span><span class="sxs-lookup"><span data-stu-id="fe8bf-112">For more information, see [Determining if a user created an inbox rule](https://docs.microsoft.com//office365/securitycompliance/auditing-troubleshooting-scenarios#determining-if-a-user-created-an-inbox-rule)</span></span>
