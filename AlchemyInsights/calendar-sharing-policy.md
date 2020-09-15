---
title: 618 kalendāra koplietošanas politika
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: d2511183d068330cdcfb4e08b08df4f18625c822
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47684237"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="2ec79-102">Politikas kļūda, kopīgojot kalendāru</span><span class="sxs-lookup"><span data-stu-id="2ec79-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="2ec79-103">Atbilstoši situācijai veiciet kādu no šīm darbībām:</span><span class="sxs-lookup"><span data-stu-id="2ec79-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="2ec79-104">Savienojuma izveide ar Exchange Online, izmantojot Remote PowerShell.</span><span class="sxs-lookup"><span data-stu-id="2ec79-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="2ec79-105">Papildinformāciju skatiet rakstā Savienojuma izveide [ar Exchange Online, izmantojot Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="2ec79-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="2ec79-106">Lokālajā serverī atveriet Exchange pārvaldības čaulu.</span><span class="sxs-lookup"><span data-stu-id="2ec79-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="2ec79-107">Noteikt lietotājam piešķirto koplietošanas politiku.</span><span class="sxs-lookup"><span data-stu-id="2ec79-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="2ec79-108">Lai to paveiktu, izpildiet šādu komandu un ievērojiet, ka tiek atgriezta politika:</span><span class="sxs-lookup"><span data-stu-id="2ec79-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="2ec79-109">Atjauniniet lietotāja kopīgošanas politiku.</span><span class="sxs-lookup"><span data-stu-id="2ec79-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="2ec79-110">Lai to izdarītu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="2ec79-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="2ec79-111">Atveriet Exchange administrēšanas centru.</span><span class="sxs-lookup"><span data-stu-id="2ec79-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="2ec79-112">Noklikšķiniet uz **organizācija**un pēc tam veiciet dubultklikšķi uz lietotāja piešķirtās **politikas.**</span><span class="sxs-lookup"><span data-stu-id="2ec79-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="2ec79-113">Šī ir politika, kas tika atgriezta 2. darbībā.</span><span class="sxs-lookup"><span data-stu-id="2ec79-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="2ec79-114">Lapā koplietošanas kārtula atlasiet kalendāra koplietošanas līmeni, kuru vēlaties atļaut sadaļā **Norādiet, kādu informāciju vēlaties koplietot**. noklikšķiniet uz **Saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="2ec79-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="2ec79-115">Lai iegūtu papildinformāciju, skatiet rakstu: ["politika neļauj piešķirt atļaujas šajā līmenī vienam vai vairākiem adresātiem", ja lietotājs mēģina kopīgot kalendāru](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="2ec79-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
