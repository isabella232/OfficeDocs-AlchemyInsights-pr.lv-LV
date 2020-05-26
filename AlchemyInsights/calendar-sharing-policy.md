---
title: 618 kalendāra koplietošanas politika
ms.author: chrisda
author: chrisda
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "618"
- "899"
- "3800014"
ms.assetid: bc3db17b-87f8-4e50-b3ee-8b105b70d67a
ms.openlocfilehash: cc5827975eff10a119281541622224d0e37f08a7
ms.sourcegitcommit: 2afad0b107d03cd8c4de0b85b5bee38a13a7960d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/26/2020
ms.locfileid: "44373006"
---
# <a name="policy-error-when-sharing-a-calendar"></a><span data-ttu-id="befdd-102">Politikas kļūda, koplietojot kalendāru</span><span class="sxs-lookup"><span data-stu-id="befdd-102">Policy error when sharing a calendar</span></span>

1. <span data-ttu-id="befdd-103">Veiciet kādu no šīm darbībām atbilstoši situācijai:</span><span class="sxs-lookup"><span data-stu-id="befdd-103">Do one of the following, as appropriate for your situation:</span></span>
    - <span data-ttu-id="befdd-104">Izveidot savienojumu ar Exchange Online, izmantojot attālo PowerShell.</span><span class="sxs-lookup"><span data-stu-id="befdd-104">Connect to Exchange Online by using Remote PowerShell.</span></span> <span data-ttu-id="befdd-105">Lai iegūtu papildinformāciju, skatiet [izveidot savienojumu ar Exchange Online, izmantojot attālo PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span><span class="sxs-lookup"><span data-stu-id="befdd-105">For more information, see [Connect to Exchange Online using Remote PowerShell](https://technet.microsoft.com/library/jj984289%28v=exchg.160%29.aspx).</span></span>
    - <span data-ttu-id="befdd-106">Lokālas serverī atveriet Exchange pārvaldības čaulu.</span><span class="sxs-lookup"><span data-stu-id="befdd-106">On the on-premises server, open the Exchange Management Shell.</span></span>
2. <span data-ttu-id="befdd-107">Nosakiet koplietošanas politikas, kas ir piešķirts lietotājam.</span><span class="sxs-lookup"><span data-stu-id="befdd-107">Determine the sharing policy that's assigned to the user.</span></span> <span data-ttu-id="befdd-108">Lai to paveiktu, izpildiet šādu komandu un iegaumējiet atgriezto politiku:</span><span class="sxs-lookup"><span data-stu-id="befdd-108">To do this, run the following command and note the policy returned:</span></span>

    `
    Get-Mailbox User1 | fl *sharing*
    `

3. <span data-ttu-id="befdd-109">Atjauniniet lietotāja koplietošanas politiku.</span><span class="sxs-lookup"><span data-stu-id="befdd-109">Update the sharing policy for the user.</span></span> <span data-ttu-id="befdd-110">Lai to izdarītu, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="befdd-110">To do this, follow these steps:</span></span>
    - <span data-ttu-id="befdd-111">Atveriet Exchange administrēšanas centrs.</span><span class="sxs-lookup"><span data-stu-id="befdd-111">Open the Exchange admin center.</span></span>
    - <span data-ttu-id="befdd-112">Noklikšķiniet uz **organizācija**un pēc tam veiciet dubultklikšķi uz politikas, kas ir piešķirta lietotājam sadaļā **individuāla koplietošana**.</span><span class="sxs-lookup"><span data-stu-id="befdd-112">Click **Organization**, and then double-click the policy that's assigned to the user under **Individual Sharing**.</span></span> <span data-ttu-id="befdd-113">Šī ir politika, kas tika atgriezta 2. darbībā.</span><span class="sxs-lookup"><span data-stu-id="befdd-113">This is the policy that was returned in step 2.</span></span>
    - <span data-ttu-id="befdd-114">Lapā koplietošanas kārtula atlasiet kalendāra koplietošanas līmeni, kuru vēlaties atļaut sadaļā **Norādiet, kādu informāciju vēlaties kopīgot**; noklikšķiniet uz **saglabāt**.</span><span class="sxs-lookup"><span data-stu-id="befdd-114">On the Sharing Rule page, select the calendar sharing level that you want to allow under **Specify what information you want to share**; click **Save**.</span></span>

<span data-ttu-id="befdd-115">Lai iegūtu papildinformāciju, skatiet: ["politika neatļauj šajā līmenī piešķirt atļaujas vienam vai vairākiem adresātiem" kļūda, kad lietotājs mēģina koplietot kalendāru](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span><span class="sxs-lookup"><span data-stu-id="befdd-115">For more information see: ["Policy does not allow granting permissions at this level to one or more of the recipient(s)" error when user tries to share calendar](https://docs.microsoft.com/exchange/troubleshoot/calendar-sharing/policy-permissions-issue).</span></span>
