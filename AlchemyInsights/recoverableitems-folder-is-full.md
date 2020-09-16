---
title: 1336 RecoverableItems mape ir pilna
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
- "1336"
- "3700003"
ms.assetid: a3a923e8-fece-4a26-b8b6-00970d75275e
ms.openlocfilehash: 6ae608b776332402fe333315f5e4ff6072b0a651
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47741274"
---
# <a name="the-recoverable-items-folder-is-full"></a><span data-ttu-id="3aed8-102">Mape Atkoptie vienumi ir pilna</span><span class="sxs-lookup"><span data-stu-id="3aed8-102">The Recoverable Items folder is full</span></span>

<span data-ttu-id="3aed8-103">Exchange Online pastkastēm mapes Atkoptie vienumi noklusējuma krātuves ierobežojums ir 30 GB.</span><span class="sxs-lookup"><span data-stu-id="3aed8-103">For Exchange Online mailboxes, the default storage limit for the Recoverable Items folder is 30 GB.</span></span> <span data-ttu-id="3aed8-104">Mapes atkopto vienumu krātuves ierobežojums tiek automātiski palielināts līdz 100 GB, ja pastkaste tiek ievietota tiesas prāvā, e-datu atklāšanas aizturēšana vai ir piešķirta saglabāšanas politikai.</span><span class="sxs-lookup"><span data-stu-id="3aed8-104">The storage limit for the Recoverable Items folder is automatically increased to 100 GB if the mailbox is placed on Litigation Hold, eDiscovery hold, or is assigned to a retention policy.</span></span>

<span data-ttu-id="3aed8-105">Kad mapē Atkoptie vienumi sasniedz krātuves ierobežojumu, pastkastes funkcionalitāte tiek ietekmēta tālāk norādītajos veidos.</span><span class="sxs-lookup"><span data-stu-id="3aed8-105">When the Recoverable Items folder reaches the storage limit, mailbox functionality is affected in the following ways:</span></span>

- <span data-ttu-id="3aed8-106">Lietotājs nevar izdzēst vienumus no pastkastes.</span><span class="sxs-lookup"><span data-stu-id="3aed8-106">The user can't delete items from the mailbox.</span></span>

- <span data-ttu-id="3aed8-107">Pārvaldītās mapes palīgs nevar izdzēst vienumus, kuru pamatā ir saglabāšanas atzīmes vai pārvaldītās mapes iestatījumi.</span><span class="sxs-lookup"><span data-stu-id="3aed8-107">The Managed Folder Assistant can't delete items based on retention tag or managed folder settings.</span></span>

- <span data-ttu-id="3aed8-108">Ja pastkastēm ir iespējota viena vienumu atkopšana vai tās tiek ievietotas aizturētas, kopēšanas lapu aizsardzības process nevar uzturēt lietotāja rediģēto vienumu versijas.</span><span class="sxs-lookup"><span data-stu-id="3aed8-108">For mailboxes that have Single Item Recovery enabled or are placed on hold, the copy-on-write page protection process can't maintain versions of items edited by the user.</span></span>

- <span data-ttu-id="3aed8-109">Pastkastes, kurās ir iespējots pastkastes audita reģistrēšana, nav pastkastes audita žurnāla ierakstu, kurus var saglabāt mapē atlasītie vienumi.</span><span class="sxs-lookup"><span data-stu-id="3aed8-109">For mailboxes that have mailbox audit logging enabled, no mailbox audit log entries can be saved in the Audits subfolder in the Recoverable Items folder.</span></span>

<span data-ttu-id="3aed8-110">Pastkastes, kas nav aizturētas, administratori var izmantot `Search-Mailbox -SearchDumpsterOnly -DeleteContent` komandu pakalpojumā Exchange Online PowerShell, lai dzēstu vienumus mapē Atkoptie vienumi.</span><span class="sxs-lookup"><span data-stu-id="3aed8-110">For mailboxes that aren't on hold, admins can use the `Search-Mailbox -SearchDumpsterOnly -DeleteContent` command in Exchange Online PowerShell to delete items in the Recoverable Items folder.</span></span> <span data-ttu-id="3aed8-111">Papildinformāciju skatiet tālāk sniegtajās tēmās.</span><span class="sxs-lookup"><span data-stu-id="3aed8-111">For more information, see the following topics:</span></span>

- [<span data-ttu-id="3aed8-112">Ziņojumu meklēšana un dzēšana</span><span class="sxs-lookup"><span data-stu-id="3aed8-112">Search for and delete messages</span></span>](https://docs.microsoft.com/microsoft-365/compliance/search-for-and-delete-messagesadmin-help)

- [<span data-ttu-id="3aed8-113">Meklēšana — pastkaste</span><span class="sxs-lookup"><span data-stu-id="3aed8-113">Search-Mailbox</span></span>](https://docs.microsoft.com/powershell/module/exchange/mailboxes/Search-Mailbox)

<span data-ttu-id="3aed8-114">Pastkastēm, kas ir aizturētas, administratoriem ir jānoņem aizturēšana, pirms tie var izdzēst vienumus no mapes Atkoptie vienumi.</span><span class="sxs-lookup"><span data-stu-id="3aed8-114">For mailboxes that are on hold, admins have to remove the hold before they can deleted items from the Recoverable Items folder.</span></span> <span data-ttu-id="3aed8-115">Lai iegūtu papildinformāciju, skatiet sadaļu [vienumu dzēšana mākonī izvietoto pastkastu mapē](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="3aed8-115">For more information, see [Delete items in the Recoverable Items folder of cloud-based mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/delete-items-in-the-recoverable-items-folder-of-mailboxes-on-hold).</span></span>

<span data-ttu-id="3aed8-116">Lai novērstu to, ka mape Atkoptie vienumi kļūst pilna, administratori var palielināt mapes atkopto vienumu krātuves ierobežojumu pastkastēm un iestatīt pastkastes saglabāšanas politiku, kas pārvieto vienumus no mapes Atkoptie vienumi uz lietotāja arhīva pastkasti.</span><span class="sxs-lookup"><span data-stu-id="3aed8-116">To help prevent the Recoverable Items folder from becoming full, admins can increase the storage limit of the Recoverable Items folder for mailboxes on hold and set up a mailbox retention policy that moves items from the Recoverable Items folder to the user's archive mailbox.</span></span> <span data-ttu-id="3aed8-117">Skatiet tēmu [pieaugošo pastkastu kvotas palielināšana](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span><span class="sxs-lookup"><span data-stu-id="3aed8-117">See [Increase the Recoverable Items quota for mailboxes on hold](https://docs.microsoft.com/microsoft-365/compliance/increase-the-recoverable-quota-for-mailboxes-on-hold).</span></span>
