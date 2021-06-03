---
title: Disku nosūtīšana Microsoft 365 importēšanas pakalpojumā
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 06/01/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "11514"
- "9003046"
ms.openlocfilehash: 85d6e723e56b01fd9914165d8c9740f3b055947d
ms.sourcegitcommit: 1226e9a9601dc8fc8ec427235f3c2dd88ff84ced
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2021
ms.locfileid: "52731652"
---
# <a name="drive-shipping-in-the-microsoft-365-import-service"></a><span data-ttu-id="1eef1-102">Disku nosūtīšana Microsoft 365 importēšanas pakalpojumā</span><span class="sxs-lookup"><span data-stu-id="1eef1-102">Drive shipping in the Microsoft 365 Import Service</span></span>

<span data-ttu-id="1eef1-103">Izmantojiet disku nosūtīšanu, kopējot PST uz cieto disku un pēc tam nosūtot cieto disku uz Microsoft.</span><span class="sxs-lookup"><span data-stu-id="1eef1-103">Use Drive shipping by copying PSTs to a hard drive and then shipping the hard drive to Microsoft.</span></span>

<span data-ttu-id="1eef1-104">Lai sāktu darbu:</span><span class="sxs-lookup"><span data-stu-id="1eef1-104">To start the job:</span></span>

1. <span data-ttu-id="1eef1-105">Atbilstības Microsoft 365 pārvaldības **sadaļā** atlasiet **Importēt**.</span><span class="sxs-lookup"><span data-stu-id="1eef1-105">In the Microsoft 365 Compliance Center under **Information Governance**, select **Import**.</span></span>

1. <span data-ttu-id="1eef1-106">Atlasiet **Izvēlieties importēšanas darba tipu** un pēc tam atlasiet **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="1eef1-106">Select **Choose import job type**, and then select **Next**.</span></span>

1. <span data-ttu-id="1eef1-107">Lai skatītu šīs importēšanas opcijas darbības, atlasiet Nosūtīt **cietos diskus uz kādu no mūsu fiziskajām atrašanās vietām**.</span><span class="sxs-lookup"><span data-stu-id="1eef1-107">To see the steps for this import option, select **Ship hard drives to one of our physical locations**.</span></span>

<span data-ttu-id="1eef1-108">Lūk, dažas lietas, kas jāatceras:</span><span class="sxs-lookup"><span data-stu-id="1eef1-108">Here are some things to remember:</span></span>

- <span data-ttu-id="1eef1-109">Lai importētu PST failus uz Microsoft 365 pastkastēm, jums ir Exchange Online pastkastes importēšanas/eksportēšanas loma.</span><span class="sxs-lookup"><span data-stu-id="1eef1-109">You must be assigned the Mailbox Import Export role in Exchange Online to import PST files to Microsoft 365 mailboxes.</span></span>
<span data-ttu-id="1eef1-110">PSTs, kas ir lielāki par 20 GB, veiktspēja var tikt ietekmēta.</span><span class="sxs-lookup"><span data-stu-id="1eef1-110">Performance might be impacted for PSTs larger than 20GB.</span></span>

- <span data-ttu-id="1eef1-111">Tiek atbalstīti tikai 2,5 collu cietvielu diski (SSD) vai 2,5 collu vai 3,5 collu SATA II/III iekšējie cietie diski.</span><span class="sxs-lookup"><span data-stu-id="1eef1-111">Only 2.5-inch solid-state drives (SSDs) or 2.5-inch or 3.5-inch SATA II/III internal hard drives are supported.</span></span>
<span data-ttu-id="1eef1-112">Cietais disks, kurā ir PST faili, jāšifrē ar BitLocker.</span><span class="sxs-lookup"><span data-stu-id="1eef1-112">Hard drive containing PST files must be encrypted with BitLocker.</span></span>

- <span data-ttu-id="1eef1-113">PST failu importēšanas izmaksas pastkastēs Microsoft 365 izmantojot disku nosūtīšanu, ir USD 2 par datu GB.</span><span class="sxs-lookup"><span data-stu-id="1eef1-113">The cost to import PST files to Microsoft 365 mailboxes using drive shipping is $2 USD per GB of data.</span></span>

<span data-ttu-id="1eef1-114">Papildinformāciju par disku nosūtīšanas metodes izmantošanu PST importēšanai skatiet rakstā Disku nosūtīšanas izmantošana, lai importētu [organizācijas PST failus.](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365)</span><span class="sxs-lookup"><span data-stu-id="1eef1-114">For additional information on using the Drive shipping method for importing PSTs, see [Use drive shipping to import your organization's PST files](/microsoft-365/compliance/use-drive-shipping-to-import-pst-files-to-office-365).</span></span>