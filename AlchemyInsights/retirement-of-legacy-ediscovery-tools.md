---
title: Mantoto e-datu atklāšanas rīku norakstīšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 986c78f20e7b8c303c302913d63d817a56ce2896
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51798556"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="17ebf-102">Mantoto e-datu atklāšanas rīku norakstīšana</span><span class="sxs-lookup"><span data-stu-id="17ebf-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="17ebf-103">Ņemot vērā jauno un uzlaboto e-datu atklāšanas funkcionalitāti Microsoft 365 atbilstības centrā, nākamo mēnešu laikā tiks izņemti šādi mantoti e-datu atklāšanas rīki un komandlietotņi:</span><span class="sxs-lookup"><span data-stu-id="17ebf-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="17ebf-104">[Ievietojiet e-datu atklāšanu](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) [un izteiksmju](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) glabāšanu Exchange administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="17ebf-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="17ebf-105">Exchange Online PowerShell cmdlet, kas atbalsta In-Place e-datu atklāšanu un glabāšanuIn-Place aizturēšanas.</span><span class="sxs-lookup"><span data-stu-id="17ebf-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="17ebf-106">(Šīs cmdlet kopā tiek identificētas kā \*-MailboxSearch cmdlet.) Tas ietver šādas cmdlet:</span><span class="sxs-lookup"><span data-stu-id="17ebf-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="17ebf-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="17ebf-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="17ebf-108">Start-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="17ebf-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="17ebf-109">Stop-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="17ebf-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="17ebf-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="17ebf-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="17ebf-111">Meklēšanas [pastkastes](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet meklētājprogrammā Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="17ebf-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="17ebf-112">Tālāk norādītās darbības Exchange tīmekļa pakalpojumu API:</span><span class="sxs-lookup"><span data-stu-id="17ebf-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="17ebf-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="17ebf-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="17ebf-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="17ebf-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="17ebf-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="17ebf-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="17ebf-116">Advanced eDiscovery v1.0</span><span class="sxs-lookup"><span data-stu-id="17ebf-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="17ebf-117">**Pensijas laika grafiks:**</span><span class="sxs-lookup"><span data-stu-id="17ebf-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="17ebf-118">**2020. gada 1. jūlijs** Jūs vairs nevarat izveidot jaunus meklējumus un aizturēšanu, tomēr jūs varat veikt, rediģēt un dzēst esošos meklēšanas vaicājumus uz savu risku.</span><span class="sxs-lookup"><span data-stu-id="17ebf-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="17ebf-119">Microsoft atbalsta dienests vairs neatbalsta In-Place e-& glabāšanu EAC.</span><span class="sxs-lookup"><span data-stu-id="17ebf-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="17ebf-120">In-Place. gada **1.** oktobris & e-datu atklāšanas līdz ar & aizturēšanas funkcionalitāti EAC tiks novietota tikai lasīšanas režīmā, tāpēc varat noņemt tikai esošās meklēšanas un aizturēšanas.</span><span class="sxs-lookup"><span data-stu-id="17ebf-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="17ebf-121">**Papildinformāciju skatiet rakstā:**</span><span class="sxs-lookup"><span data-stu-id="17ebf-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="17ebf-122">Mantoto e-datu atklāšanas meklējumu migrēšana uz Microsoft 365 atbilstības centru</span><span class="sxs-lookup"><span data-stu-id="17ebf-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="17ebf-123">Mantoto e-datu atklāšanas rīku norakstīšana</span><span class="sxs-lookup"><span data-stu-id="17ebf-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="17ebf-124">Bieži uzdotie jautājumi In-Place e-datu atklāšanu In-Place aizturēšanu</span><span class="sxs-lookup"><span data-stu-id="17ebf-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



