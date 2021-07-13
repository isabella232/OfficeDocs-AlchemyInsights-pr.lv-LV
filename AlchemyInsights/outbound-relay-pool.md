---
title: Izejošā pārraide pūls
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/08/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3000003"
- "12315"
ms.openlocfilehash: b723566a29e0be581b7fdc30332166d5cddbd38f
ms.sourcegitcommit: 270a1ca9c35b50b8be6b06f432c9c90e4090fb57
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/08/2021
ms.locfileid: "53381718"
---
# <a name="outbound-relay-pool"></a><span data-ttu-id="67667-102">Izejošā pārraide pūls</span><span class="sxs-lookup"><span data-stu-id="67667-102">Outbound relay pool</span></span>

<span data-ttu-id="67667-103">Microsoft veic dažas izmaiņas e-pasta pārsūtīšanas vai pārsūtīšanas konfigurācijā, izmantojot Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="67667-103">Microsoft is making some changes to the configuration for relaying or forwarding email through Microsoft 365.</span></span> <span data-ttu-id="67667-104">Ziņojumi noteiktos scenārijos tiek pārsūtīti vai izlaisti, Microsoft 365 izmanto īpašu pārraides pūlu.</span><span class="sxs-lookup"><span data-stu-id="67667-104">Messages in certain scenarios are forwarded or relayed through Microsoft 365 using a special relay pool.</span></span> <span data-ttu-id="67667-105">Ziņojumi, kas tiek sūtīti, izmantojot pārraides pūlu, var nokļūt adresāta nevēlamā e-pasta mapē.</span><span class="sxs-lookup"><span data-stu-id="67667-105">Messages sent by using the relay pool could end up in recipient's junk mail folder.</span></span> <span data-ttu-id="67667-106">Papildinformāciju skatiet rakstā [Izejošā piegādes maršruts](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span><span class="sxs-lookup"><span data-stu-id="67667-106">For more information, see [Outbound delivery pools](/microsoft-365/security/office-365-security/high-risk-delivery-pool-for-outbound-messages#relay-pool)</span></span>

<span data-ttu-id="67667-107">Lai izvairītos no scenārija, izmantojot pārraides pūlu, pārliecinieties, vai pārsūtītie/pārsūtītie ziņojumi atbilst vienam no šiem kritērijiem:</span><span class="sxs-lookup"><span data-stu-id="67667-107">To avoid a scenario using the relay pool, make sure that forwarded/relayed messages meet one of the following criteria:</span></span>

- <span data-ttu-id="67667-108">Izejošais sūtītājs ir nomnieka akceptētais domēns.</span><span class="sxs-lookup"><span data-stu-id="67667-108">The outbound sender is an accepted domain of the tenant.</span></span>
- <span data-ttu-id="67667-109">Sūtītāja politikas struktūra (Sender Policy Framework – SPF) nodod šādu Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="67667-109">Sender Policy Framework (SPF) passes when the message comes to Microsoft 365.</span></span>
- <span data-ttu-id="67667-110">DomainKeys identificētais pasts (DomainKeys Identified Mail – DKIM) P2 sūtītāja domēnā tiek nododams, kad ziņojums Microsoft 365.</span><span class="sxs-lookup"><span data-stu-id="67667-110">DomainKeys Identified Mail (DKIM) on the P2 sender domain passes when the message comes to Microsoft 365.</span></span>
 
<span data-ttu-id="67667-111">Ziņojumi, kas atbilst iepriekš minētajiem kritērijiem, netiek izlaisti caur pārraides pūlu.</span><span class="sxs-lookup"><span data-stu-id="67667-111">Messages that meet the above criteria are not relayed through the relay pool.</span></span>

<span data-ttu-id="67667-112">Ja jūsu domēna MX ieraksts norāda uz trešās puses vai lokālo serveri, izmantojiet uzlaboto filtrēšanu, lai pārliecinātos, vai SPF validācija ir pareiza ienākošajiem e-pasta ziņojumiem un izvairītos no e-pasta sūtīšanas caur pārraides pūlu.</span><span class="sxs-lookup"><span data-stu-id="67667-112">If the MX record for your domain is pointed to a third-party or on-premises server, use enhanced filtering to make sure the SPF validation is correct for inbound email and to avoid sending email through the relay pool.</span></span>

<span data-ttu-id="67667-113">**Kā noteikt, vai pārraides pūls ietekmēs mūs?**</span><span class="sxs-lookup"><span data-stu-id="67667-113">**How can we tell if we're impacted by the relay pool?**</span></span>

<span data-ttu-id="67667-114">Ja pārsūtītie vai izlaistie e-pasta ziņojumi izmanto kādu no iepriekš minētajiem kritērijiem, ziņojumi netiks pārsūtīti caur pārraides pūlu.</span><span class="sxs-lookup"><span data-stu-id="67667-114">If your forwarded or relayed emails use one of the above criteria, messages won't be relayed through the relay pool.</span></span> <span data-ttu-id="67667-115">Taču, ja ziņojums tiek nosūtīts caur pārraides pūlu, izejošā servera IP adrese atrodas diapazonā 40.95.0.0/16 un izejošā servera nosaukumā ir iekļauts **rly.**</span><span class="sxs-lookup"><span data-stu-id="67667-115">However, if a message is sent through a relay pool, the outbound server IP is in the 40.95.0.0/16 range and the outbound server name includes **rly** in the name.</span></span>

