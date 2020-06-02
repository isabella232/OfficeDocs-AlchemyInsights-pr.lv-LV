---
title: 1336 RecoverableItems mape ir pilna
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 4f0cba480fcc05114abd8f370b84e9a37e5f2804
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510759"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="6bc24-102">Atkopto vienumu mape ir pilna</span><span class="sxs-lookup"><span data-stu-id="6bc24-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="6bc24-103">Exchange Online pastkastes mapes atkopt vienumus noklusējuma krātuves limits ir 30 GB.</span><span class="sxs-lookup"><span data-stu-id="6bc24-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="6bc24-104">Atkopt vienumus mapē krātuves limits tiek automātiski palielināts 100 GB, ja pastkaste ir novietota aizturēšana, eDiscovery turēt vai ir piešķirta saglabāšanas politika.</span><span class="sxs-lookup"><span data-stu-id="6bc24-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="6bc24-105">Ja atkopt vienumus mapē sasniedz krātuves ierobežojums, pastkastes funkcionalitāte tiek ietekmēta šādi:</span><span class="sxs-lookup"><span data-stu-id="6bc24-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="6bc24-106">Lietotājs nevar izdzēst vienumus no pastkastes.</span><span class="sxs-lookup"><span data-stu-id="6bc24-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="6bc24-107">Pārvaldīto mapju palīgs nevar dzēst vienumus, pamatojoties uz saglabāšanas tagu vai pārvaldīto mapju iestatījumus.</span><span class="sxs-lookup"><span data-stu-id="6bc24-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="6bc24-108">Pastkastēm, kas ir iespējota viena vienuma atkopšana vai tiek aizturēts, kopiju rakstīšanas lapas aizsardzības process nevar uzturēt lietotāja rediģēto vienumu versijas.</span><span class="sxs-lookup"><span data-stu-id="6bc24-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="6bc24-109">Pastkastēm, kas ir iespējota pastkastes audita reģistrēšanu, nevar saglabāt pastkastes audita žurnāla ierakstus atkopt vienumus mapē audita apakšmapē.</span><span class="sxs-lookup"><span data-stu-id="6bc24-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="6bc24-110">Pastkastēm, kas nav aizturēts, administratori var izmantot `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komandu Exchange Online PowerShell dzēst vienumus mapē atkopt vienumus.</span><span class="sxs-lookup"><span data-stu-id="6bc24-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="6bc24-111">Papildinformāciju skatiet tālāk sniegtajās tēmās.</span><span class="sxs-lookup"><span data-stu-id="6bc24-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="6bc24-112">Ziņojumu meklēšana un dzēšana</span><span class="sxs-lookup"><span data-stu-id="6bc24-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="6bc24-113">Meklēšanas pastkaste</span><span class="sxs-lookup"><span data-stu-id="6bc24-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="6bc24-114">Pastkastēm, kas ir aizturēts, administratoriem ir jānoņem aizturi, pirms tie var dzēst vienumus no mapes atkopt vienumus.</span><span class="sxs-lookup"><span data-stu-id="6bc24-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="6bc24-115">Lai iegūtu papildinformāciju, skatiet [vienumu dzēšana mapē atkopt vienumus mākonis balstītas pastkastes](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold)aizturēts.</span><span class="sxs-lookup"><span data-stu-id="6bc24-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="6bc24-116">Lai novērstu atkopt vienumus mapē kļūst pilna, administratori var palielināt atmiņas limits atkopt vienumus mapes pastkastes aizturēts un iestatīt pastkastes saglabāšanas politika, kas pārvieto vienumus no mapes atkopt vienumus lietotāja arhīva pastkaste.</span><span class="sxs-lookup"><span data-stu-id="6bc24-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="6bc24-117">Skatiet [atkopt krājumu kvota aizturētā pastkastes](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="6bc24-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
