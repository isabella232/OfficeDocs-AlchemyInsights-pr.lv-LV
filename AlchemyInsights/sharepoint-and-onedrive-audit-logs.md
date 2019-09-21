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
ms.openlocfilehash: af5b3c76b82db13bc89c917247e41fa1d8779b68
ms.sourcegitcommit: d5bf97a0bf0547f36b6da9684ce9f16a13a7749e
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/20/2019
ms.locfileid: "37068030"
---
# <a name="sharepoint-and-onedrive-audit-logs"></a><span data-ttu-id="58096-102">SharePoint un OneDrive audita žurnāli</span><span class="sxs-lookup"><span data-stu-id="58096-102">SharePoint and OneDrive audit logs</span></span>

<span data-ttu-id="58096-103">**SharePoint un OneDrive mūsdienu vienotā audita žurnālus no atbilstības**</span><span class="sxs-lookup"><span data-stu-id="58096-103">**SharePoint and OneDrive Modern Unified Audit logs from compliance**</span></span>

- [<span data-ttu-id="58096-104">Ieslēgt/izslēgt vienoto audita reģistrēšanu</span><span class="sxs-lookup"><span data-stu-id="58096-104">Turn on/off Unified Audit Logging</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off) 

<span data-ttu-id="58096-105">Nav nepieciešama papildu konfigurācija programmā SharePoint vai OneDrive.</span><span class="sxs-lookup"><span data-stu-id="58096-105">No additional configuration is required within SharePoint or OneDrive.</span></span>

- <span data-ttu-id="58096-106">Izmantojiet audita reģistrēšanas meklēšanu, lai pārbaudītu faila (-u), mapes (u), lietotāja (u) darbību, atļaujas:</span><span class="sxs-lookup"><span data-stu-id="58096-106">Use audit logging search to check activity of the file(s), folder(s), user(s), permissions:</span></span>

    - [<span data-ttu-id="58096-107">Failu un lappušu darbības</span><span class="sxs-lookup"><span data-stu-id="58096-107">File and page activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance)
    - [<span data-ttu-id="58096-108">Mapes darbības</span><span class="sxs-lookup"><span data-stu-id="58096-108">Folder activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#folder-activities)
    - [<span data-ttu-id="58096-109">Koplietošanas un piekļuves pieprasījumu darbības</span><span class="sxs-lookup"><span data-stu-id="58096-109">Sharing and access request activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#sharing-and-access-request-activities)
    - [<span data-ttu-id="58096-110">Sinhronizēšanas darbības</span><span class="sxs-lookup"><span data-stu-id="58096-110">Synchronization activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#synchronization-activities)
    - [<span data-ttu-id="58096-111">Vietnes administrēšanas darbības</span><span class="sxs-lookup"><span data-stu-id="58096-111">Site administration activities</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#site-administration-activities)
- <span data-ttu-id="58096-112">Lai iegūtu papildinformāciju par to, kā izgūt šos notikumus, skatiet [Meklēt audita žurnālā](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span><span class="sxs-lookup"><span data-stu-id="58096-112">For more information about how to retrieve these events, see [Search the audit log](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance#search-the-audit-log).</span></span>

<span data-ttu-id="58096-113">**SharePoint Classic audita žurnāli**</span><span class="sxs-lookup"><span data-stu-id="58096-113">**SharePoint classic Audit logs**</span></span>

<span data-ttu-id="58096-114">Mēs migrējuši SPO, veicot auditēšanu vienotā audita žurnālā (UAL).</span><span class="sxs-lookup"><span data-stu-id="58096-114">We migrated SPO legacy auditing to Unified Audit Log (UAL).</span></span> <span data-ttu-id="58096-115">Tas būtībā nozīmē, ka visi SPO mantotie audita ziņojumi tagad tiks aprīkoti ar UAL un mantotie audita signāli ir pārvietoti uz UAL.</span><span class="sxs-lookup"><span data-stu-id="58096-115">This essentially means that all SPO legacy audit reports will now be powered through UAL, and the legacy audit signals have been migrated to UAL.</span></span>

<span data-ttu-id="58096-116">Galvenās izmaiņas:</span><span class="sxs-lookup"><span data-stu-id="58096-116">Key changes:</span></span>

- <span data-ttu-id="58096-117">Apgriešana kā iespēja nav pieejama.</span><span class="sxs-lookup"><span data-stu-id="58096-117">Trimming as a capability is NOT available.</span></span>
- <span data-ttu-id="58096-118">Sadaļa, kurā izvēlaties konkrētus auditācijas notikumus, nav pieejama.</span><span class="sxs-lookup"><span data-stu-id="58096-118">The section where you choose specific events to audit is NOT available.</span></span> <span data-ttu-id="58096-119">Lūdzu, skatiet [šo dokumentu](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) , lai iegūtu pilnu sarakstu ar auditētajiem notikumiem, kas pieejami pēc noklusējuma.</span><span class="sxs-lookup"><span data-stu-id="58096-119">Please refer to [this document](https://docs.microsoft.com/office365/securitycompliance/search-the-audit-log-in-security-and-compliance) for a complete list of audited events available by default.</span></span>
- <span data-ttu-id="58096-120">Opcija "atrašanās vieta" sadaļā **pielāgoti pārskati** nav pieejama.</span><span class="sxs-lookup"><span data-stu-id="58096-120">The "Location" option under **Customized reports** is NOT available.</span></span> 
- <span data-ttu-id="58096-121">"Dokumentu atvēršana vai lejupielāde" pasākumi nav pieejami.</span><span class="sxs-lookup"><span data-stu-id="58096-121">“Opening or downloading documents” events is NOT available.</span></span> 

