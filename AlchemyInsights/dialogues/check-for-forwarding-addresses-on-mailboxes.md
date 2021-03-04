---
title: Pārbaudiet, vai nav pāradresēšanas adreses pastkastēs
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 17/02/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 1b0a6c8fe368196f2d1f9811aea895c2c024b2e6
ms.sourcegitcommit: 969219d6dff18d86d679d4d8741d1e39e4ce9539
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/03/2021
ms.locfileid: "50427717"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="d2719-102">Pārbaudiet, vai nav pāradresēšanas adreses pastkastēs</span><span class="sxs-lookup"><span data-stu-id="d2719-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="d2719-103">Dažreiz urķi var pārsūtīt lietotāju e-pasta ziņojumus, tāpēc vispirms mēs pārbaudām, vai pastkastē ir pāradresēšanas adreses un kārtulas.</span><span class="sxs-lookup"><span data-stu-id="d2719-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="d2719-104">Pēc tam mēs pārbaudām audita žurnālus.</span><span class="sxs-lookup"><span data-stu-id="d2719-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="d2719-105">Tālāk ir aprakstīts, kā pārbaudīt pārsūtīšanas adreses.</span><span class="sxs-lookup"><span data-stu-id="d2719-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="d2719-106">Atlasiet **lietotāji**  >  **Aktīvie lietotāji**.</span><span class="sxs-lookup"><span data-stu-id="d2719-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="d2719-107">Atlasiet lietotāju, kura konts ir apdraudēts.</span><span class="sxs-lookup"><span data-stu-id="d2719-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="d2719-108">Parādītajā izlidošanā izvērsiet **pasta iestatījumi** un pēc tam noklikšķiniet  uz rediģēt **e-pasta pārsūtīšanai**.</span><span class="sxs-lookup"><span data-stu-id="d2719-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="d2719-109">Noņemiet visas pārsūtīšanas adreses, kuras neatpazīstat.</span><span class="sxs-lookup"><span data-stu-id="d2719-109">Remove any forwarding addresses you don't recognize.</span></span>