---
title: Savienojuma politikas labošana
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
ms.openlocfilehash: 0b6286350e706e493f6d30b7978aacedc02daff5
ms.sourcegitcommit: bd6a9cb5d357baee5134c0dea430afc2a035c810
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/09/2021
ms.locfileid: "50694169"
---
# <a name="fix-connection-policy"></a><span data-ttu-id="5bfd1-102">Savienojuma politikas labošana</span><span class="sxs-lookup"><span data-stu-id="5bfd1-102">Fix connection policy</span></span>

<span data-ttu-id="5bfd1-103">E-pasta ziņojums tika atzīmēts kā drošs un piegādāts lietotāja iesūtnei, jo sūtītāja IP adrese ir atzīmēta kā droša savienojuma filtra politikā.</span><span class="sxs-lookup"><span data-stu-id="5bfd1-103">The email was marked safe and delivered to the user's inbox because the sending IP address was marked safe in the Connection Filter policy.</span></span> <span data-ttu-id="5bfd1-104">Lai pārskatītu politiku, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="5bfd1-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="5bfd1-105">Dodieties uz [Office 365 drošības & atbilstības centru](https://go.microsoft.com/fwlink/p/?linkid=2077143)un pēc tam dodieties uz **Threat Management**  >  **Policy**  >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="5bfd1-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="5bfd1-106">Cilnē **Pielāgota** atlasiet **savienojuma filtra politiku** un pēc tam atlasiet **Rediģēt politiku**.</span><span class="sxs-lookup"><span data-stu-id="5bfd1-106">On the **Custom** tab, select the **Connection filter policy**, and then select **Edit policy**.</span></span>
3. <span data-ttu-id="5bfd1-107">Pārskatiet **IP atļauto** sarakstu.</span><span class="sxs-lookup"><span data-stu-id="5bfd1-107">Review the **IP Allow** list.</span></span> <span data-ttu-id="5bfd1-108">Pārbaudiet, vai ir iespējots **Drošais saraksts** .</span><span class="sxs-lookup"><span data-stu-id="5bfd1-108">See if **Safe list** is enabled.</span></span>

    > [!NOTE]
    > <span data-ttu-id="5bfd1-109">Microsoft abonē trešo pušu uzticamo sūtītāju avotus.</span><span class="sxs-lookup"><span data-stu-id="5bfd1-109">Microsoft subscribes to third-party sources of trusted senders.</span></span> <span data-ttu-id="5bfd1-110">Ja **Drošais saraksts** ir iespējots, šie uzticamie sūtītāji nav kļūdaini atzīmēti kā mēstules.</span><span class="sxs-lookup"><span data-stu-id="5bfd1-110">If **Safe list** is enabled, these trusted senders aren't mistakenly marked as spam.</span></span> <span data-ttu-id="5bfd1-111">Iesakām atlasīt šo opciju, jo tādējādi tiks samazināts maldīgu pozitīvu darbību skaits (labs pasts, kas ir klasificēts kā surogātpasts), ko saņemat.</span><span class="sxs-lookup"><span data-stu-id="5bfd1-111">I recommend selecting this option, because it will reduce the number of false positives (good mail that's classified as spam) that you receive.</span></span>
