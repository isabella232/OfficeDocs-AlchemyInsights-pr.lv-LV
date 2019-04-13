---
title: 1336 RecoverableItems mape ir pilna
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 1336
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 14d46980caf7dac90e73c34482a3aee34382fa1f
ms.sourcegitcommit: 1a4b8fa9e38a95ca811085af516edb81caf2018c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/13/2019
ms.locfileid: "31859003"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="a89b0-102">Atkopt vienumus mape ir pilna</span><span class="sxs-lookup"><span data-stu-id="a89b0-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="a89b0-103">Exchange Online pastkastēm Office 365, atkopt vienumus mapē noklusējuma glabāšanas limits ir 30 GB.</span><span class="sxs-lookup"><span data-stu-id="a89b0-103">For Exchange Online mailboxes in Office 365, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="a89b0-104">Atkopt vienumus mapē krātuves ierobežojums automātiski palielina līdz 100GB ja pastkaste tiek likts uz tiesāšanos turiet eDiscovery aizturēšana, vai ir piešķirta biroja 365 saglabāšanas politiku.</span><span class="sxs-lookup"><span data-stu-id="a89b0-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to an Office 365 retention policy.</span></span>

<span data-ttu-id="a89b0-105">Atkopt vienumus mapē sasniedz krātuves limits, funkcionalitāti pastkastes tiek ietekmētas šādos veidos:</span><span class="sxs-lookup"><span data-stu-id="a89b0-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="a89b0-106">Lietotājs nevar dzēst vienumus no pastkastes.</span><span class="sxs-lookup"><span data-stu-id="a89b0-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="a89b0-107">Pārvaldītas mapes palīgu nevar dzēst vienumus, pamatojoties uz aiztures tag vai pārvaldītās mapes iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="a89b0-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="a89b0-108">Pastkastēm ir iespējota vienotā vienumu atkopšana vai tiek aizturēta, lapas kopiju rakstīšanas aizsardzības procesā nevar uzturēt elementu rediģēt lietotājs versijām.</span><span class="sxs-lookup"><span data-stu-id="a89b0-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="a89b0-109">Pastkastēm, kuriem ir pastkaste, audita iespējotu reģistrēšanu, pastkastes audita žurnāla ieraksti var tikt saglabāti revīziju apakšmapei mapē atkopt vienumus.</span><span class="sxs-lookup"><span data-stu-id="a89b0-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="a89b0-110">Pastkastēm, kas nav aizturēts, varat izmantot admins `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komandu Exchange Online PowerShell, lai izdzēstu vienumus atkopt vienumu mapē.</span><span class="sxs-lookup"><span data-stu-id="a89b0-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="a89b0-111">Papildinformāciju skatiet tālāk sniegtajās tēmās.</span><span class="sxs-lookup"><span data-stu-id="a89b0-111">For more information, see the following topics:</span></span> 

- [<span data-ttu-id="a89b0-112">Meklēt un dzēst ziņojumus</span><span class="sxs-lookup"><span data-stu-id="a89b0-112">Search for and delete messages</span></span>](https://docs.microsoft.com/office365/securitycompliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="a89b0-113">Meklēšanas pastkasti</span><span class="sxs-lookup"><span data-stu-id="a89b0-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="a89b0-114">Pastkastes, kas ir aizturēta, admins ir noņemt aizturēšanu, pirms tie var atkopt vienumus mapē Izdzēstie vienumi.</span><span class="sxs-lookup"><span data-stu-id="a89b0-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="a89b0-115">Plašāku informāciju skatiet [Dzēst vienumus atgūstamo vienumus, turiet mākonis balstītu pastkastītes uz mapi](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a89b0-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="a89b0-116">Lai nekļūtu atkopt vienumus mapē pilna, admins var palielināt krātuves ierobežojums atgūstamo vienumus mapē pastkastēm, turēt un iestatīt pastkasti saglabāšanas politika, kas pārvieto vienumus no mapes atkopt vienumus lietotāja Arhīvs pastkasti.</span><span class="sxs-lookup"><span data-stu-id="a89b0-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="a89b0-117">Sk. [palielināt atgūstamo vienumus pastkastes uz kvotu turiet](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="a89b0-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/office365/securitycompliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
