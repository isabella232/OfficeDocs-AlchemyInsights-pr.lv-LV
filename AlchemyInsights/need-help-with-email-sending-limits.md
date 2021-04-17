---
title: Vai nepieciešama palīdzība saistībā ar e-pasta sūtīšanas ierobežojumiem?
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
- "9002938"
- "5630"
ms.openlocfilehash: b5bdfbf818328c97ec93b3468aeedcbe88e03913
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836286"
---
# <a name="need-help-with-email-sending-limits"></a><span data-ttu-id="171f2-102">Vai nepieciešama palīdzība saistībā ar e-pasta sūtīšanas ierobežojumiem?</span><span class="sxs-lookup"><span data-stu-id="171f2-102">Need help with email sending limits?</span></span>

<span data-ttu-id="171f2-103">Tālāk ir norādīti **izstrādē iekļautie sūtīšanas ierobežojumi**, kurus izmanto pakalpojums.</span><span class="sxs-lookup"><span data-stu-id="171f2-103">Below is the **by-design sending limits** enforced in the service.</span></span> <span data-ttu-id="171f2-104">Papildinformācija par šiem ierobežojumiem ir dokumentēta [šeit](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span><span class="sxs-lookup"><span data-stu-id="171f2-104">More information on these limits is documented [here](https://docs.microsoft.com/office365/servicedescriptions/exchange-online-service-description/exchange-online-limits#receiving-and-sending-limits).</span></span>

- <span data-ttu-id="171f2-105">Lai novērstu nevēlamu lielapjoma ziņojumu piegādi, katra lietotājam mēs lietojam **adresātu daudzuma ierobežojumus visiem izejošajiem un iekšējiem ziņojumiem**.</span><span class="sxs-lookup"><span data-stu-id="171f2-105">To discourage the delivery of unsolicited bulk messages, we apply per-user **recipient rate limits to all outbound and internal messages**.</span></span> <span data-ttu-id="171f2-106">Visos SKU šis ierobežojums ir **10 000 adresātu dienā**.</span><span class="sxs-lookup"><span data-stu-id="171f2-106">Across all SKUs, this limit is **10,000 recipients per day**.</span></span>  <span data-ttu-id="171f2-107">Klientiem, kuriem jānosūta likumīgs komercpasts (piemēram, biļeteni klientiem), ir jāizmanto tādu trešo pušu pakalpojumu sniedzēju pakalpojumi, kas specializējas šādu pakalpojumu sniegšanā.</span><span class="sxs-lookup"><span data-stu-id="171f2-107">Customers who need to send legitimate bulk commercial email (for example, customer newsletters) should use third-party providers that specialize in these services.</span></span>
    - <span data-ttu-id="171f2-108">**Piezīme**. Tiklīdz šis ierobežojums tiek sasniegts, ziņojumus no pastkastes nevar nosūtīt līdz brīdim, kad adresātu, kuriem pēdējo 24 stundu laikā tika nosūtīti ziņojumi, skaits kļūst mazāks par šo ierobežojuma vērtību.</span><span class="sxs-lookup"><span data-stu-id="171f2-108">**Note**: Once the recipient rate limit is reached, messages can't be sent from the mailbox until the number of recipients that were sent messages in the past 24 hours drops below the limit.</span></span> <span data-ttu-id="171f2-109">Līdz tam lietotājs nevarēs nosūtīt ziņojumus.</span><span class="sxs-lookup"><span data-stu-id="171f2-109">The user will not be able to send messages until that point.</span></span>
- <span data-ttu-id="171f2-110">Ziņojumu daudzuma ierobežojums **30 ziņojumi minūtē** tiek lietots visos SKU.</span><span class="sxs-lookup"><span data-stu-id="171f2-110">Message rate limit of **30 messages per minute** is applied across all SKUs.</span></span> <span data-ttu-id="171f2-111">Tas nosaka, cik daudz ziņojumu lietotājs var nosūtīt no sava Exchange Online konta noteiktā laika periodā.</span><span class="sxs-lookup"><span data-stu-id="171f2-111">This determines how many messages a user can send from their Exchange Online account within a specified period.</span></span>
- <span data-ttu-id="171f2-112">**Maksimālais adresātu skaits, kas atļauts viena e-pasta ziņojuma laukā Kam, Kopija un Diskrētā kopija**, ir **1000 adresātu**.</span><span class="sxs-lookup"><span data-stu-id="171f2-112">The **maximum number of recipients allowed in the To, Cc, and Bcc** fields for a single email message, across all SKUs, is **1000 recipients**.</span></span> <span data-ttu-id="171f2-113">Lai pielāgotu šo ierobežojumu, dodieties [šeit](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span><span class="sxs-lookup"><span data-stu-id="171f2-113">To customize this limit, go [here](https://techcommunity.microsoft.com/t5/exchange-team-blog/customizable-recipient-limits-in-office-365/ba-p/1183228).</span></span>
