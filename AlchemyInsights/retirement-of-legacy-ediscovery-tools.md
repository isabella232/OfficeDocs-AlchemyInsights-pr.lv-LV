---
title: Veco e-datu atklāšanas rīku vecums
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001487"
- "3523"
ms.openlocfilehash: 94cd2127240be5faacd397ba6255fdb16e364308
ms.sourcegitcommit: d4fc2a03af69e28e96075812d040fdd34d2e23f0
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/26/2020
ms.locfileid: "46902627"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="d30e3-102">Veco e-datu atklāšanas rīku vecums</span><span class="sxs-lookup"><span data-stu-id="d30e3-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="d30e3-103">Jaunajā un uzlabotajā e-datu atklāšanas funkcionalitātē Microsoft 365 atbilstības centrā tālāk norādītie mantotie e-datu atklāšanas rīki un commandlets būs novecojuši.</span><span class="sxs-lookup"><span data-stu-id="d30e3-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="d30e3-104">Oriģinālu [e-datu atklāšanu](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) un [oriģinālu turēšanu](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="d30e3-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="d30e3-105">Exchange Online PowerShell cmdlet, kas atbalsta oriģinālu e-datu atklāšanu un oriģinālu turēšanu.</span><span class="sxs-lookup"><span data-stu-id="d30e3-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="d30e3-106">(Šīs cmdlet tiek kopīgi identificētas kā \*-MailboxSearch cmdlet.) Tas ietver šādas cmdlet:</span><span class="sxs-lookup"><span data-stu-id="d30e3-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="d30e3-107">New-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d30e3-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="d30e3-108">Sākums — MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d30e3-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="d30e3-109">Pārtraukt-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d30e3-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="d30e3-110">Set-MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="d30e3-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="d30e3-111">[Meklēšanas-pastkastes](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet pakalpojumā Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="d30e3-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="d30e3-112">Tālāk norādītās darbības Exchange tīmekļa pakalpojumu API.</span><span class="sxs-lookup"><span data-stu-id="d30e3-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="d30e3-113">GetSearchableMailboxes</span><span class="sxs-lookup"><span data-stu-id="d30e3-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="d30e3-114">SetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d30e3-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="d30e3-115">GetHoldOnMailboxes</span><span class="sxs-lookup"><span data-stu-id="d30e3-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="d30e3-116">Uzlabots e-datu atklāšanas v 1.0</span><span class="sxs-lookup"><span data-stu-id="d30e3-116">Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="d30e3-117">**Pensijas laika grafiks**:</span><span class="sxs-lookup"><span data-stu-id="d30e3-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="d30e3-118">**2020. gada 1. jūlijs** Jūs vairs nevarat izveidot jaunus meklēšanas un aizturēšanas, bet jūs pats varat veikt, rediģēt un dzēst esošos meklēšanas rezultātus.</span><span class="sxs-lookup"><span data-stu-id="d30e3-118">**July 1, 2020** You can no longer create new searches and holds, but you can run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="d30e3-119">Microsoft atbalsts vairs neatbalsta e-datu atklāšanu, & ir iekļauta EAC.</span><span class="sxs-lookup"><span data-stu-id="d30e3-119">Microsoft Support no longer supports In-Place eDiscovery & Holds in the EAC.</span></span>
    
- <span data-ttu-id="d30e3-120">**2020. gada 1. oktobris** Atrašanās vietas e-datu atklāšanas &ā EAC funkcionalitāte tiek iekļauta tikai lasīšanas režīmā, tāpēc varat noņemt tikai esošos meklēšanas rezultātus un aizturēšanas.</span><span class="sxs-lookup"><span data-stu-id="d30e3-120">**October 1, 2020** In-Place eDiscovery & Holds functionality in the EAC will be placed in read-only mode, so you can only remove existing searches and holds.</span></span>

<span data-ttu-id="d30e3-121">Papildinformāciju **skatiet rakstā**:</span><span class="sxs-lookup"><span data-stu-id="d30e3-121">**For more information, see**:</span></span>

 - [<span data-ttu-id="d30e3-122">Mantoto e-datu atklāšanas meklēšana un aizturēšana uz Microsoft 365 atbilstības centru</span><span class="sxs-lookup"><span data-stu-id="d30e3-122">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="d30e3-123">Veco e-datu atklāšanas rīku vecums</span><span class="sxs-lookup"><span data-stu-id="d30e3-123">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="d30e3-124">Bieži uzdotie jautājumi par oriģinālu e-datu atklāšanu un oriģinālu turēšanu</span><span class="sxs-lookup"><span data-stu-id="d30e3-124">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)



