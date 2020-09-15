---
title: 'Kļūda: šī datora kārtulas nesakrīt'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c2feb6da651d8b3eb7af6a057335b28d26f9e7f6
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47690970"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="8f56b-102">Kļūda: šī datora kārtulas nesakrīt</span><span class="sxs-lookup"><span data-stu-id="8f56b-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="8f56b-103">Lai skatītu šīs zināmās problēmas atjauninātu statusu, skatiet [šī datora kārtulas neatbilst Microsoft Exchange kārtulām](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="8f56b-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="8f56b-104">Outlook komanda ir ieviesusi labojumu būvējumā 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="8f56b-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="8f56b-105">Labojums jau ir no programmas Insider Fast, un tas tiks novirzīts uz sadaļu mēneša kanāls 2020 jūnija beigās.</span><span class="sxs-lookup"><span data-stu-id="8f56b-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="8f56b-106">Kad ir fiksēts būvējums, var tikt parādīta uzvedne "kuras kārtulas vēlaties paturēt" vienu pēdējo reizi.</span><span class="sxs-lookup"><span data-stu-id="8f56b-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="8f56b-107">Pēc uzaicinājuma izvēlieties serveris un pēc tam pārejiet atpakaļ programmā Outlook un atkārtoti iespējojiet kārtulas, kas ir atspējotas.</span><span class="sxs-lookup"><span data-stu-id="8f56b-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="8f56b-108">Līdz brīdim, kad būs pieejams labojums, lūdzu, izmantojiet šo risinājumu:</span><span class="sxs-lookup"><span data-stu-id="8f56b-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="8f56b-109">**Risinājums**: pēdējo atskaišu gadījumā problēma ir radusies tiem, kas ir izveidojuši tikai klienta kārtulas Outlook datora versijā.</span><span class="sxs-lookup"><span data-stu-id="8f56b-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="8f56b-110">Ja joprojām rodas problēma, apsveriet iespēju izdzēst kārtulas un pēc tam izveidot un rediģēt kārtulas tikai OWA (Outlook Web App), līdz problēma ir novērsta.</span><span class="sxs-lookup"><span data-stu-id="8f56b-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="8f56b-111">Ja nevarat izdzēst kārtulas manuāli, varat palaist Outlook komandu, startējot programmu Outlook, palaižot Outlook.exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="8f56b-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="8f56b-112">Tādējādi tiks izdzēsti gan klienta, gan servera kārtulas.</span><span class="sxs-lookup"><span data-stu-id="8f56b-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="8f56b-113">Tiks izdzēsti visi Outlook profilā esošo kontu noteikumi.</span><span class="sxs-lookup"><span data-stu-id="8f56b-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="8f56b-114">Šī komanda tālāk ir dokumentēta komandrindas slēdžu rakstā.</span><span class="sxs-lookup"><span data-stu-id="8f56b-114">This command is further documented in the Command-line switches article.</span></span>

