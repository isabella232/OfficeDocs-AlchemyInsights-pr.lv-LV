---
title: Lietotāja politikas/pastkastes iestatījumu labošana
ms.author: v-jmathew
author: v-jmathew
manager: dansimp
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000760"
- "7391"
ms.openlocfilehash: ca998c453fcb0905b122436f0eea384a9b8a9992
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694172"
---
# <a name="fix-user-policymailbox-settings"></a><span data-ttu-id="94164-102">Lietotāja politikas/pastkastes iestatījumu labošana</span><span class="sxs-lookup"><span data-stu-id="94164-102">Fix user policy/mailbox settings</span></span>

<span data-ttu-id="94164-103">Nevēlamais e-pasta iestatījumi pastkastē ietekmēja šo ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="94164-103">The junk mail settings on the mailbox affected this message.</span></span> <span data-ttu-id="94164-104">Lai pārskatītu iestatījumus, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="94164-104">To review the settings, do the following:</span></span>

1. <span data-ttu-id="94164-105">Palaidiet Exchange pārvaldības čaulu.</span><span class="sxs-lookup"><span data-stu-id="94164-105">Launch Exchange Management Shell.</span></span> <span data-ttu-id="94164-106">Papildinformāciju skatiet rakstā [Exchange pārvaldības čaulas atvēršana](https://go.microsoft.com/fwlink/?linkid=2101432).</span><span class="sxs-lookup"><span data-stu-id="94164-106">For more information, see [Open the Exchange Management Shell](https://go.microsoft.com/fwlink/?linkid=2101432).</span></span>
2. <span data-ttu-id="94164-107">Izpildīt šo komandu (izmantojot lietotāja e-pasta adresi):  **Get-mailboxjunkmailconfiguration-Identity "user@domain.com"**</span><span class="sxs-lookup"><span data-stu-id="94164-107">Run this command (using the user's email address):  **get-mailboxjunkmailconfiguration -identity "user@domain.com"**</span></span>
3. <span data-ttu-id="94164-108">Pārbaudiet, vai sūtītāja e-pasta adrese ir daļa no **TrustedSendersAndDomains** vai **BlockedSendersAndDomains**.</span><span class="sxs-lookup"><span data-stu-id="94164-108">Check if the sender's email address is part of **TrustedSendersAndDomains** or **BlockedSendersAndDomains**.</span></span> <span data-ttu-id="94164-109">Ja e-pasta adrese ir kādā no sarakstiem, iespējams, tas ir jānoņem.</span><span class="sxs-lookup"><span data-stu-id="94164-109">If the email address is in one of the lists, you may have to remove it.</span></span> <span data-ttu-id="94164-110">Papildinformāciju skatiet rakstā [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span><span class="sxs-lookup"><span data-stu-id="94164-110">To learn more, see [Set-MailboxJunkEmailConfiguration](https://go.microsoft.com/fwlink/?linkid=2101047).</span></span>
