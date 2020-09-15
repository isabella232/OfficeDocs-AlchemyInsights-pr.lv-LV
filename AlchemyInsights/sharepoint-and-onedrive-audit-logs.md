---
title: Klasiskās SharePoint audita žurnālu atskaites
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
- "1372"
- "3100005"
ms.assetid: ''
ms.openlocfilehash: daf79f8d75ccdff8ad54f0f307648a5832a6bb71
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47662215"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="880de-102">SharePoint un OneDrive audita žurnāli</span><span class="sxs-lookup"><span data-stu-id="880de-102">SharePoint and OneDrive audit logs</span></span>

## <a name="sharepoint-classic-audit-logs"></a><span data-ttu-id="880de-103">SharePoint klasiskā audita žurnāli</span><span class="sxs-lookup"><span data-stu-id="880de-103">SharePoint classic Audit logs</span></span>

<span data-ttu-id="880de-104">SPO mantotā auditēšana ir migrēta uz vienotā audita žurnālu (UAL).</span><span class="sxs-lookup"><span data-stu-id="880de-104">SPO legacy auditing was migrated to Unified Audit Log (UAL).</span></span> <span data-ttu-id="880de-105">Visas SPO mantotās auditēšanas atskaites tagad tiks darbinātas, izmantojot UAL, un mantotie audita signāli ir migrēti uz UAL.</span><span class="sxs-lookup"><span data-stu-id="880de-105">All SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="880de-106">Galvenās izmaiņas:</span><span class="sxs-lookup"><span data-stu-id="880de-106">Key changes:</span></span>

* <span data-ttu-id="880de-107">Apgriešana nav pieejama kā iespēja.</span><span class="sxs-lookup"><span data-stu-id="880de-107">Trimming is NOT available as a capability.</span></span>
* <span data-ttu-id="880de-108">Konkrētu notikumu atlase auditam nav pieejama.</span><span class="sxs-lookup"><span data-stu-id="880de-108">Choosing specific events to audit is NOT available.</span></span> <span data-ttu-id="880de-109">[Šajā dokumentā](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) ir parādīts pilnīgs saraksts ar audita pasākumiem, kas pieejami pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="880de-109">Refer to [this document](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
* <span data-ttu-id="880de-110">Opcija **atrašanās vieta** sadaļā **pielāgotas atskaites** nav pieejama.</span><span class="sxs-lookup"><span data-stu-id="880de-110">The **Location** option under **Customized reports** is NOT available.</span></span>
* <span data-ttu-id="880de-111">Opcija **Atvērt vai lejupielādēt dokumentu** notikumus nav pieejama.</span><span class="sxs-lookup"><span data-stu-id="880de-111">The **Opening or downloading documents** events option is NOT available.</span></span>

[<span data-ttu-id="880de-112">Vietņu kolekcijas auditēšanas iestatījumu konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="880de-112">Configure Audit settings for a site collection</span></span>](https://support.office.com/article/Configure-audit-settings-for-a-site-collection-A9920C97-38C0-44F2-8BCB-4CF1E2AE22D2)

## <a name="sharepoint-and-onedrive-modern-unified-audit-logs-from-compliance"></a><span data-ttu-id="880de-113">SharePoint un OneDrive modernie vienotie audita žurnāli no atbilstības</span><span class="sxs-lookup"><span data-stu-id="880de-113">SharePoint and OneDrive Modern Unified Audit logs from compliance</span></span>

* [<span data-ttu-id="880de-114">Vienotās audita reģistrēšanas ieslēgšana/izslēgšana</span><span class="sxs-lookup"><span data-stu-id="880de-114">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="880de-115">Koplietošanas vidē SharePoint vai OneDrive papildu konfigurācija nav nepieciešama.</span><span class="sxs-lookup"><span data-stu-id="880de-115">No additional configuration is required within SharePoint or OneDrive.</span></span>

<span data-ttu-id="880de-116">Izmantojiet audita reģistrēšanas meklēšanu, lai pārbaudītu failu (-s), mapju (-u), lietotāju (u), atļauju:</span><span class="sxs-lookup"><span data-stu-id="880de-116">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

* [<span data-ttu-id="880de-117">Failu un lapu darbības</span><span class="sxs-lookup"><span data-stu-id="880de-117">File and page activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance)
* [<span data-ttu-id="880de-118">Mapju darbības</span><span class="sxs-lookup"><span data-stu-id="880de-118">Folder activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#folder-activities)
* [<span data-ttu-id="880de-119">Koplietošanas un piekļuves pieprasījumu darbības</span><span class="sxs-lookup"><span data-stu-id="880de-119">Sharing and access request activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
* [<span data-ttu-id="880de-120">Sinhronizēšanas darbības</span><span class="sxs-lookup"><span data-stu-id="880de-120">Synchronization activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
* [<span data-ttu-id="880de-121">Vietnes administrēšanas darbības</span><span class="sxs-lookup"><span data-stu-id="880de-121">Site administration activities</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)

<span data-ttu-id="880de-122">Papildinformāciju par to, kā izgūt šos notikumus, skatiet rakstā [meklēšana audita žurnālu](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="880de-122">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/microsoft-365/compliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>
