---
title: DLP izmantošana transportēšanas kārtulās
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002635"
- "5153"
ms.openlocfilehash: e512b36b34c5fc4931fb0f796790ee4b01c6443c
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51827223"
---
# <a name="using-dlp-in-transport-rules"></a><span data-ttu-id="43cbd-102">DLP izmantošana transportēšanas kārtulās</span><span class="sxs-lookup"><span data-stu-id="43cbd-102">Using DLP in transport rules</span></span>

<span data-ttu-id="43cbd-103">Datu zuduma novēršanas (DLP) integrācijai esošā kārtulā, transportēšanas kārtulas iestatījumos izmantojiet nosacījumu "**Ja ziņojums satur...Sensitīvu informāciju**".</span><span class="sxs-lookup"><span data-stu-id="43cbd-103">To integrate Data Loss Prevention (DLP) into an existing transport, use the condition "**If the message contains...Sensitive Information**" in the Transport rule setting.</span></span>

<span data-ttu-id="43cbd-104">**Papildinformācijai lasiet:**</span><span class="sxs-lookup"><span data-stu-id="43cbd-104">**For more details, see:**</span></span>

- <span data-ttu-id="43cbd-105">Integrētie DLP sensitīvās informācijas tipi transportēšanas kārtulās: [Integrēt sensitīvās informācijas kārtulas](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span><span class="sxs-lookup"><span data-stu-id="43cbd-105">Integrated DLP sensitive information types in transport rules: [Integrate Sensitive Information Rules](https://docs.microsoft.com/exchange/security-and-compliance/data-loss-prevention/integrate-sensitive-information-rules).</span></span>

<span data-ttu-id="43cbd-106">Jūs varat pārbaudīt kārtulu ar vai bez politikas testa, pielietojot kārtulai testa režīmu.</span><span class="sxs-lookup"><span data-stu-id="43cbd-106">You can also test the rule with or without policy test using Test Mode on the rule.</span></span>  <span data-ttu-id="43cbd-107">Pēc kārtulas izveidošanas jums ir jāuzgaida 30 minūtes pirms to pārbaudīt. </span><span class="sxs-lookup"><span data-stu-id="43cbd-107">You should wait 30 mins after creating the rule before testing it.</span></span>

- <span data-ttu-id="43cbd-108">Lasiet [Pasta plūsmas/transportēšanas kārtulu pārbaude](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span><span class="sxs-lookup"><span data-stu-id="43cbd-108">See [Test Mail Flow/Transport rules](https://docs.microsoft.com/exchange/security-and-compliance/mail-flow-rules/test-mail-flow-rules)</span></span>

<span data-ttu-id="43cbd-109">**Piezīme**: ja EAC vēlaties ieviest jaunu DLP politiku ar transportēšanas kārtulām, tā vietā izmantojiet [DLP politikas drošības un atbilstības centrā](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="43cbd-109">**Note**: If you are trying to implement a new DLP policy with transport rules in the EAC, use [DLP Policies in the Security and Compliance center](https://docs.microsoft.com/microsoft-365/compliance/data-loss-prevention-policies?view=o365-worldwide) instead.</span></span>
