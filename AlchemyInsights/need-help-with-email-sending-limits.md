---
title: Vai nepieciešama palīdzība ar e-pasta sūtīšanas ierobežojumiem?
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002938"
- "5630"
ms.openlocfilehash: 7f563df313c869d18c3e4240d271c649a74914af
ms.sourcegitcommit: 88d2918aa51f4ba10771527380c3e0db0f5a9147
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/20/2020
ms.locfileid: "44357866"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="e7467-102">Vai nepieciešama palīdzība ar e-pasta sūtīšanas ierobežojumiem?</span><span class="sxs-lookup"><span data-stu-id="e7467-102">Need help with email sending limits?</span></span>

<span data-ttu-id="e7467-103">Tālāk ir norādīts **pēc konstrukcijas sūtīšanas ierobežojumi** , kas tiek ieviesti pakalpojumā.</span><span class="sxs-lookup"><span data-stu-id="e7467-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="e7467-104">Plašāka informācija par šiem limitiem ir dokumentēta [šeit](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="e7467-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="e7467-105">Lai atturētu no nevēlamu lielapjoma ziņojumu piegādes, mēs izmantojam katra lietotāja **adresāta likmju ierobežojumus visiem izejošajiem un iekšējiem ziņojumiem**.</span><span class="sxs-lookup"><span data-stu-id="e7467-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="e7467-106">Visos SKU, šis limits ir **10 000 adresāti dienā**.</span><span class="sxs-lookup"><span data-stu-id="e7467-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="e7467-107">Klientiem, kuriem jānosūta likumīgs lielapjoma komerciālais e-pasts (piemēram, klientu biļeteni), jāizmanto trešo pušu pakalpojumu sniedzēji, kas specializējas šajos pakalpojumos.</span><span class="sxs-lookup"><span data-stu-id="e7467-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="e7467-108">**Piezīme**: pēc adresāta likmju ierobežojums ir sasniegts, ziņojumus nevar nosūtīt no pastkastes līdz adresātu skaits, kas tika nosūtīti ziņojumi pēdējo 24 stundu laikā nokrītas zem ierobežojuma.</span><span class="sxs-lookup"><span data-stu-id="e7467-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="e7467-109">Lietotājs nevarēs nosūtīt ziņojumus līdz šim brīdim.</span><span class="sxs-lookup"><span data-stu-id="e7467-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="e7467-110">Ziņojumu pārraides ātruma ierobežojums **30 ziņojumiem minūtē** tiek lietots visās SKU.</span><span class="sxs-lookup"><span data-stu-id="e7467-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="e7467-111">Tas nosaka, cik daudz ziņojumu lietotājs var nosūtīt no sava Exchange Online konta noteiktā periodā.</span><span class="sxs-lookup"><span data-stu-id="e7467-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="e7467-112">**Maksimālais atļautais adresātu skaits laukos kam, kopija un Diskrētā kopija** vienam e-pasta ziņojumam visās skus ir **1000 adresāti**.</span><span class="sxs-lookup"><span data-stu-id="e7467-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="e7467-113">Lai pielāgotu šo limitu, dodieties [šeit](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="e7467-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
