---
title: 'Kļūda: šī datora kārtulas neatbilst'
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: c46eb856baafbef9bc3b7fa34a0258ef16923fb8
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782959"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="cd16e-102">Kļūda: šī datora kārtulas neatbilst</span><span class="sxs-lookup"><span data-stu-id="cd16e-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="cd16e-103">Lai skatītu šīs zināmās problēmas atjaunināto [statusu, skatiet rakstu Kārtulas šajā datorā neatbilst Microsoft Exchange kārtulām](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="cd16e-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="cd16e-104">Outlook komanda ieviesusi labojumu būvējumā 12928.10000.</span><span class="sxs-lookup"><span data-stu-id="cd16e-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="cd16e-105">Labojums jau ir pieejams Insider Fast kanālā, un tas tiks atvērts mēneša kanālā 2020. gada jūnija beigās.</span><span class="sxs-lookup"><span data-stu-id="cd16e-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="cd16e-106">Kad ir iegūts labotais būvējumu, vienu reizi var tikt parādīta uzvedne "Kuras kārtulas vēlaties paturēt".</span><span class="sxs-lookup"><span data-stu-id="cd16e-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="cd16e-107">Pēc uzaicinājuma izvēlieties Serveris, pēc tam atgriezieties programmā Outlook un atkārtoti iespējojiet visas atspējotās kārtulas.</span><span class="sxs-lookup"><span data-stu-id="cd16e-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="cd16e-108">Kamēr labojums nav pieejams, lūdzu, izmantojiet tālāk norādīto risinājumu.</span><span class="sxs-lookup"><span data-stu-id="cd16e-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="cd16e-109">**Risinājums. Jaunākajās** atskaitēs šī problēma radās tām atskaitēm, kuras Outlook datora programmā ir izveidotas tikai klienta kārtulas.</span><span class="sxs-lookup"><span data-stu-id="cd16e-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="cd16e-110">Ja problēma joprojām pastāv, apsveriet iespēju izdzēst kārtulas un pēc tam izveidot un rediģēt kārtulas tikai programmā OWA (Outlook Web App), līdz problēma tiks atrisināta.</span><span class="sxs-lookup"><span data-stu-id="cd16e-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="cd16e-111">Ja kārtulas nevarat izdzēst manuāli, varat izpildīt outlook komandu, startējot programmu Outlook, palaižot Outlook.exe /cleanrules.</span><span class="sxs-lookup"><span data-stu-id="cd16e-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="cd16e-112">Tādējādi tiks izdzēstas gan klienta, gan servera kārtulas.</span><span class="sxs-lookup"><span data-stu-id="cd16e-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="cd16e-113">Tā izdzēsīs visas kārtulas visiem kontiem Outlook profilā.</span><span class="sxs-lookup"><span data-stu-id="cd16e-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="cd16e-114">Šī komanda ir papildus dokumentēta rakstā Komandrindas slēdži.</span><span class="sxs-lookup"><span data-stu-id="cd16e-114">This command is further documented in the Command-line switches article.</span></span>

