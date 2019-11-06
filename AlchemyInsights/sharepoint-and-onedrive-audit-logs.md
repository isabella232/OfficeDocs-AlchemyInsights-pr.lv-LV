---
title: Klasiskās SharePoint audita žurnāla atskaites
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: ''
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: be95034bea3c58a4fde96cfb0f9ba525e810758e
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/05/2019
ms.locfileid: "37992625"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="27c4b-102">SharePoint un OneDrive audita žurnāli</span><span class="sxs-lookup"><span data-stu-id="27c4b-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="27c4b-103">SharePoint Classic audita žurnāli</span><span class="sxs-lookup"><span data-stu-id="27c4b-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="27c4b-104">SPO mantotā auditēšana tika migrēta uz vienoto audita žurnālu (UAL).</span><span class="sxs-lookup"><span data-stu-id="27c4b-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="27c4b-105">Visi SPO mantotie audita ziņojumi tagad tiks aprīkoti ar UAL, un mantotie audita signāli ir pārvietoti uz UAL.</span><span class="sxs-lookup"><span data-stu-id="27c4b-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="27c4b-106">Galvenās izmaiņas:</span><span class="sxs-lookup"><span data-stu-id="27c4b-106">Key changes:</span></span>

* <span data-ttu-id="27c4b-107">Apgriešana nav pieejama kā iespēja.</span><span class="sxs-lookup"><span data-stu-id="27c4b-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="27c4b-108">Konkrētu audita pasākumu izvēle nav pieejama.</span><span class="sxs-lookup"><span data-stu-id="27c4b-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="27c4b-109">Skatiet [šo dokumentu](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) , lai iegūtu pilnīgu sarakstu ar auditētajiem notikumiem, kas pieejami pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="27c4b-109">Refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="27c4b-110">Sadaļā **pielāgoti pārskati** opcija **atrašanās vieta** nav pieejama.</span><span class="sxs-lookup"><span data-stu-id="27c4b-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="27c4b-111">**Atverot vai lejupielādējot dokumentu** notikumu opcija nav pieejama.</span><span class="sxs-lookup"><span data-stu-id="27c4b-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="27c4b-112">Vietņu kolekcijas audita iestatījumu konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="27c4b-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="27c4b-113">SharePoint un OneDrive mūsdienu vienotā audita žurnālus no atbilstības</span><span class="sxs-lookup"><span data-stu-id="27c4b-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="27c4b-114">Ieslēgt/izslēgt vienoto audita reģistrēšanu</span><span class="sxs-lookup"><span data-stu-id="27c4b-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="27c4b-115">Nav nepieciešama papildu konfigurācija programmā SharePoint vai OneDrive.</span><span class="sxs-lookup"><span data-stu-id="27c4b-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="27c4b-116">Izmantojiet audita reģistrēšanas meklēšanu, lai pārbaudītu faila (-u), mapes (u), lietotāja (u) darbību, atļaujas:</span><span class="sxs-lookup"><span data-stu-id="27c4b-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="27c4b-117">Failu un lappušu darbības</span><span class="sxs-lookup"><span data-stu-id="27c4b-117">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="27c4b-118">Mapes darbības</span><span class="sxs-lookup"><span data-stu-id="27c4b-118">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="27c4b-119">Koplietošanas un piekļuves pieprasījumu darbības</span><span class="sxs-lookup"><span data-stu-id="27c4b-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="27c4b-120">Sinhronizēšanas darbības</span><span class="sxs-lookup"><span data-stu-id="27c4b-120">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="27c4b-121">Vietnes administrēšanas darbības</span><span class="sxs-lookup"><span data-stu-id="27c4b-121">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="27c4b-122">Lai iegūtu papildinformāciju par to, kā izgūt šos notikumus, skatiet [Meklēt audita žurnālā](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="27c4b-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
