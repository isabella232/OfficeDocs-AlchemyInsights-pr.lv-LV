---
title: 'Kļūda: kārtulas šajā datorā nesakrīt'
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "3518"
- "1800021"
ms.openlocfilehash: ecc1e5ec741cc90c58698991c3a3135f87c39938
ms.sourcegitcommit: 9816ac4d0fef20558383a491e0e76b79c56323f5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/09/2020
ms.locfileid: "44618020"
---
# <a name="error-the-rules-on-this-computer-do-not-match"></a><span data-ttu-id="b7cbd-102">Kļūda: kārtulas šajā datorā nesakrīt</span><span class="sxs-lookup"><span data-stu-id="b7cbd-102">Error: The rules on this computer do not match</span></span>

<span data-ttu-id="b7cbd-103">Lai skatītu atjauninātu šīs zināmās problēmas statusu, skatiet [kārtulas šajā datorā neatbilst noteikumiem par Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span><span class="sxs-lookup"><span data-stu-id="b7cbd-103">To see updated status of this known issue, see [The rules on this computer do not match the rules on Microsoft Exchange](https://support.office.com/article/d032e037-b224-429e-b325-633afde9b5f0)</span></span>

<span data-ttu-id="b7cbd-104">Outlook komanda ir ieviesusi Fix veidot 12928,10000.</span><span class="sxs-lookup"><span data-stu-id="b7cbd-104">The Outlook Team has implemented a fix in Build 12928.10000.</span></span> <span data-ttu-id="b7cbd-105">Fix jau ir Insider Fast un dosies uz ikmēneša kanāls jūnija beigās 2020.</span><span class="sxs-lookup"><span data-stu-id="b7cbd-105">The fix is already at Insider Fast and will go to Monthly Channel in late June 2020.</span></span> <span data-ttu-id="b7cbd-106">Kad esat fiksēto būvēt jūs varat saņemt tūlītēju "kas noteikumi jūs vēlaties saglabāt" pēdējoreiz.</span><span class="sxs-lookup"><span data-stu-id="b7cbd-106">Once you have the fixed build you may get the prompt "Which rules do you want to keep" one last time.</span></span> <span data-ttu-id="b7cbd-107">Izvēlieties serveri, kad tiek parādīta uzvedne, un pēc tam atgriezieties programmā Outlook un atkārtoti iespējojiet kārtulas, kas tika atspējotas.</span><span class="sxs-lookup"><span data-stu-id="b7cbd-107">Choose Server when prompted and then go back in Outlook and re-enable any rules that were disabled.</span></span>

<span data-ttu-id="b7cbd-108">Līdz labojums ir pieejams, lūdzu, izmantojiet šo metodi:</span><span class="sxs-lookup"><span data-stu-id="b7cbd-108">Until the fix is available please use the following workaround:</span></span>

<span data-ttu-id="b7cbd-109">**Risinājums**: pēdējo ziņojumu problēma ir radusies tiem, kas izveidoti tikai klienta kārtulas Outlook darbvirsmā.</span><span class="sxs-lookup"><span data-stu-id="b7cbd-109">**Workaround**: In recent reports, the issue has occurred for those that have only created client rules in Outlook desktop.</span></span> <span data-ttu-id="b7cbd-110">Ja joprojām tiek palaists problēmu, apsveriet kārtulas dzēšanu un pēc tam izveidojiet un rediģējiet kārtulas tikai OWA (Outlook Web App) līdz problēma ir atrisināta.</span><span class="sxs-lookup"><span data-stu-id="b7cbd-110">If you continue to run into the problem, consider deleting the rules and then create and edit rules only in OWA (Outlook Web App) until the issue is resolved.</span></span>

<span data-ttu-id="b7cbd-111">Ja nevarat izdzēst kārtulas manuāli var palaist Outlook komandu, startējot programmu Outlook, palaižot Outlook. exe/Cleanrules.</span><span class="sxs-lookup"><span data-stu-id="b7cbd-111">If you cannot delete the rules manually you can run an Outlook command when you start Outlook by running Outlook.exe /cleanrules.</span></span> <span data-ttu-id="b7cbd-112">Tas dzēsīs gan klienta, gan servera kārtulas.</span><span class="sxs-lookup"><span data-stu-id="b7cbd-112">This will delete both the client and server rules.</span></span> <span data-ttu-id="b7cbd-113">Tas izdzēsīs visus noteikumus visiem Outlook profila kontiem.</span><span class="sxs-lookup"><span data-stu-id="b7cbd-113">It will delete all of the rules for all of the accounts in the Outlook Profile.</span></span> <span data-ttu-id="b7cbd-114">Šī komanda ir tālāk dokumentēta komandrindas slēdži rakstu.</span><span class="sxs-lookup"><span data-stu-id="b7cbd-114">This command is further documented in the Command-line switches  article.</span></span>