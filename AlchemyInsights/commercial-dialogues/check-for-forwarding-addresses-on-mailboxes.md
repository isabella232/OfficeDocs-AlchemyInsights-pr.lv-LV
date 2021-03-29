---
title: Pastkastu adrešu pārsūtīšanas pāradresēšana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9002486"
- "7524"
ms.openlocfilehash: 3abd45230360c61ecb62e4b7a39d1b0b547271fc
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51403318"
---
# <a name="check-for-forwarding-addresses-on-mailboxes"></a><span data-ttu-id="ccf5e-102">Pastkastu adrešu pārsūtīšanas pāradresēšana</span><span class="sxs-lookup"><span data-stu-id="ccf5e-102">Check for forwarding addresses on mailboxes</span></span>

<span data-ttu-id="ccf5e-103">Dažreiz urķi pārsūta lietotāju e-pasta ziņojumus sev, tāpēc vispirms mēs meklēsim adrešu un kārtulu pārsūtīšanu pastkastē.</span><span class="sxs-lookup"><span data-stu-id="ccf5e-103">Sometimes hackers forward users' email messages to themselves, so first we'll check for forwarding addresses and rules on the mailbox.</span></span> <span data-ttu-id="ccf5e-104">Pēc tam mēs pārbaudīsim audita žurnālus.</span><span class="sxs-lookup"><span data-stu-id="ccf5e-104">Then we'll check the audit logs.</span></span> <span data-ttu-id="ccf5e-105">Tālāk aprakstīts, kā pārbaudīt, vai nav pārsūtīšanas adrešu.</span><span class="sxs-lookup"><span data-stu-id="ccf5e-105">Here's how to check for forwarding addresses:</span></span>

1. <span data-ttu-id="ccf5e-106">Atlasiet **Lietotāji**  >  **Aktīvie lietotāji**.</span><span class="sxs-lookup"><span data-stu-id="ccf5e-106">Select **Users** > **Active users**.</span></span>
1. <span data-ttu-id="ccf5e-107">Atlasiet lietotāju, kura konts ir apdraudēts.</span><span class="sxs-lookup"><span data-stu-id="ccf5e-107">Select the user whose account has been compromised.</span></span>
1. <span data-ttu-id="ccf5e-108">Parādītajā izlidošanas logā izvērsiet Pasta iestatījumi un **pēc tam** noklikšķiniet uz Rediģēt pie **E-pasta** **pārsūtīšana.**</span><span class="sxs-lookup"><span data-stu-id="ccf5e-108">In the flyout that appears, expand **Mail Settings**, and then click **Edit** for **Email forwarding**.</span></span>
1. <span data-ttu-id="ccf5e-109">Noņemiet visas neatpazītās pārsūtīšanas adreses.</span><span class="sxs-lookup"><span data-stu-id="ccf5e-109">Remove any forwarding addresses you don't recognize.</span></span>