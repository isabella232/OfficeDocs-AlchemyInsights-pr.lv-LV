---
title: Iepriekšējās paaudzes eDiscovery rīku norakstīšanas
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
ms.openlocfilehash: af9a0bd8ff4294575ac68f37d4997bb50b132ce7
ms.sourcegitcommit: 9ab422063e5a474c92ed956d42d222b90336fecb
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/11/2020
ms.locfileid: "42600383"
---
# <a name="retirement-of-legacy-ediscovery-tools"></a><span data-ttu-id="20f87-102">Iepriekšējās paaudzes eDiscovery rīku norakstīšanas</span><span class="sxs-lookup"><span data-stu-id="20f87-102">Retirement of Legacy eDiscovery Tools</span></span>

<span data-ttu-id="20f87-103">Jaunā un uzlabotā e-datu atklāšanas funkcionalitātes rezultātā Microsoft 365 atbilstības centrā šādas mantotās eDiscovery rīki un commandlets tiks pensijā nākamajos mēnešos:</span><span class="sxs-lookup"><span data-stu-id="20f87-103">As a result of the new and improved eDiscovery functionality in Microsoft 365 Compliance center, the following legacy eDiscovery tools and commandlets will be retired in the coming months:</span></span>

- <span data-ttu-id="20f87-104">[In-place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) un [oriģinālu tur](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) Exchange administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="20f87-104">[In-Place eDiscovery](https://docs.microsoft.com/exchange/security-and-compliance/in-place-ediscovery/in-place-ediscovery) and [In-Place Holds](https://docs.microsoft.com/exchange/security-and-compliance/create-or-remove-in-place-holds) in the Exchange admin center.</span></span>

- <span data-ttu-id="20f87-105">Exchange Online PowerShell cmdlet, kas atbalsta in-place eDiscovery un oriģinālu tur.</span><span class="sxs-lookup"><span data-stu-id="20f87-105">The Exchange Online PowerShell cmdlets that support In-Place eDiscovery and In-Place Holds.</span></span> <span data-ttu-id="20f87-106">(Šie cmdlets kopīgi identificē kā \* MailboxSearch cmdlet.) Tas ietver šādu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="20f87-106">(These cmdlets are collectively identified as \*-MailboxSearch cmdlets.) This includes the following cmdlets:</span></span>

    - [<span data-ttu-id="20f87-107">Jauns MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="20f87-107">New-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/new-mailboxsearch)
    - [<span data-ttu-id="20f87-108">Sākuma MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="20f87-108">Start-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/start-mailboxsearch)
    - [<span data-ttu-id="20f87-109">Stop MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="20f87-109">Stop-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/stop-mailboxsearch)
    - [<span data-ttu-id="20f87-110">Kopa MailboxSearch</span><span class="sxs-lookup"><span data-stu-id="20f87-110">Set-MailboxSearch</span></span>](https://docs.microsoft.com/powershell/module/exchange/policy-and-compliance-content-search/set-mailboxsearch)

- <span data-ttu-id="20f87-111">[Meklēšanas pastkasti](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet Exchange Online PowerShell.</span><span class="sxs-lookup"><span data-stu-id="20f87-111">The [Search-Mailbox](https://docs.microsoft.com/powershell/module/exchange/mailboxes/search-mailbox?view=exchange-ps) cmdlet in Exchange Online PowerShell.</span></span>
- <span data-ttu-id="20f87-112">Exchange tīmekļa pakalpojumos API šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="20f87-112">The following operations in the Exchange Web Services API:</span></span>
    - [<span data-ttu-id="20f87-113">Getsearchablepastkastēm</span><span class="sxs-lookup"><span data-stu-id="20f87-113">GetSearchableMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getsearchablemailboxes-operation)
    - [<span data-ttu-id="20f87-114">Setholdonpastkastēm</span><span class="sxs-lookup"><span data-stu-id="20f87-114">SetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/setholdonmailboxes-operation)
    - [<span data-ttu-id="20f87-115">Getholdonpastkastēm</span><span class="sxs-lookup"><span data-stu-id="20f87-115">GetHoldOnMailboxes</span></span>](https://docs.microsoft.com/exchange/client-developer/web-service-reference/getholdonmailboxes-operation)

- [<span data-ttu-id="20f87-116">Office 365 Advanced eDiscovery v 1.0</span><span class="sxs-lookup"><span data-stu-id="20f87-116">Office 365 Advanced eDiscovery v1.0</span></span>](https://docs.microsoft.com/microsoft-365/compliance/office-365-advanced-ediscovery)

<span data-ttu-id="20f87-117">**Pensionēšanās grafiks**:</span><span class="sxs-lookup"><span data-stu-id="20f87-117">**Timeline for retirement**:</span></span>
- <span data-ttu-id="20f87-118">April 1, 2020: jūs nevarēsiet izveidot jaunu meklēšanu un tilpnēs, bet jūs joprojām varat palaist, rediģēt un dzēst esošo meklēšanu uz savu risku.</span><span class="sxs-lookup"><span data-stu-id="20f87-118">April 1, 2020: You won't be able to create new searches and holds, but you can still run, edit, and delete existing searches at your own risk.</span></span> <span data-ttu-id="20f87-119">Microsoft Support vairs neatbalsta in-place eDiscovery & pieder EAC.</span><span class="sxs-lookup"><span data-stu-id="20f87-119">Microsoft Support will no longer support In-Place eDiscovery & Holds in the EAC.</span></span>

- <span data-ttu-id="20f87-120">Jūlijs 1, 2020: In-Place eDiscovery & tur funkcionalitāti EAC tiks ievietots tikai lasīšanas režīmā.</span><span class="sxs-lookup"><span data-stu-id="20f87-120">July 1, 2020: The In-Place eDiscovery & Holds functionality in the EAC will be placed in a read-only mode.</span></span> <span data-ttu-id="20f87-121">Tas nozīmē, ka varēsit noņemt tikai esošos meklēšanas vaicājumus un aizturēšanas.</span><span class="sxs-lookup"><span data-stu-id="20f87-121">This means you'll only be able to remove existing searches and holds.</span></span>

<span data-ttu-id="20f87-122">Papildinformāciju **skatiet**:</span><span class="sxs-lookup"><span data-stu-id="20f87-122">**For more information, see**:</span></span>

 - [<span data-ttu-id="20f87-123">Mantotā eDiscovery meklēšanas un aizturēšanas migrēt uz Microsoft 365 atbilstības centrs</span><span class="sxs-lookup"><span data-stu-id="20f87-123">Migrate legacy eDiscovery searches and holds to the Microsoft 365 compliance center</span></span>](https://docs.microsoft.com/microsoft-365/compliance/migrate-legacy-ediscovery-searches-and-holds)
 - [<span data-ttu-id="20f87-124">Iepriekšējās paaudzes eDiscovery rīku norakstīšanas</span><span class="sxs-lookup"><span data-stu-id="20f87-124">Retirement of legacy eDiscovery tools</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement)
 - [<span data-ttu-id="20f87-125">BUJ par in-place eDiscovery un oriģinālu tur</span><span class="sxs-lookup"><span data-stu-id="20f87-125">FAQs about In-Place eDiscovery and In-Place Holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/legacy-ediscovery-retirement#faqs-about-in-place-ediscovery-and-in-place-holds)


