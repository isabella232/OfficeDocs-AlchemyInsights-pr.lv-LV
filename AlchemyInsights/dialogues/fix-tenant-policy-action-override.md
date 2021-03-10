---
title: Nomnieka politikas labošana (darbības ignorēšana)
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
ms.openlocfilehash: bc7ad8acd86c9d5b2f99ffdc6fe8a8b53e1fcb8b
ms.sourcegitcommit: 60c504f3ac187eaf1141b3ba701d9e0633bdd968
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50694060"
---
# <a name="fix-tenant-policy-action-override"></a><span data-ttu-id="17f91-102">Nomnieka politikas labošana (darbības ignorēšana)</span><span class="sxs-lookup"><span data-stu-id="17f91-102">Fix Tenant policy (action override)</span></span>

<span data-ttu-id="17f91-103">Šis ziņojums ietekmēja jūsu nomnieka pretsurogātpasta politiku.</span><span class="sxs-lookup"><span data-stu-id="17f91-103">An anti-spam policy in your tenant affected this message.</span></span> <span data-ttu-id="17f91-104">Lai pārskatītu politiku, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="17f91-104">To review the policy, do the following:</span></span>

1. <span data-ttu-id="17f91-105">Dodieties uz [Office 365 drošības & atbilstības centru](https://go.microsoft.com/fwlink/p/?linkid=2077143)un pēc tam dodieties uz **Threat Management**  >  **Policy**  >  [anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span><span class="sxs-lookup"><span data-stu-id="17f91-105">Go to the [Office 365 Security & Compliance Center](https://go.microsoft.com/fwlink/p/?linkid=2077143), and then go to **Threat management** > **Policy** > [Anti-spam](https://go.microsoft.com/fwlink/?linkid=2101518).</span></span>
2. <span data-ttu-id="17f91-106">Pārbaudiet, vai **politikas avots** norāda šādu informāciju:  **Add-Xheader/ModifySubject/redirect/DELETE/bez darbības/diskrētās kopijas ziņojums**</span><span class="sxs-lookup"><span data-stu-id="17f91-106">Check to see if **Policy source** indicates the following:  **Add-Xheader/ModifySubject/Redirect/Delete/No action/ BCC message**</span></span>

    <span data-ttu-id="17f91-107">Ja tā ir, cilnē **pielāgot** atzīmējiet tās politikas iestatījumus, kas ietekmēja šo ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="17f91-107">If so, on the **Custom** tab, check the settings of the policy that affected the message.</span></span> <span data-ttu-id="17f91-108">Iespējams, ka **standarta iestatījumi** ir lietoti visiem Exchange Online aizsardzības klientiem, kas ietekmējuši šo ziņojumu.</span><span class="sxs-lookup"><span data-stu-id="17f91-108">It's possible that the **Standard settings** applied to all Exchange Online Protection customers affected the message.</span></span>

<span data-ttu-id="17f91-109">Papildinformāciju par surogātpasta filtrēšanas politiku konfigurēšanu skatiet rakstā [surogātpasta filtrēšanas politiku konfigurēšana](https://go.microsoft.com/fwlink/?linkid=2101431).</span><span class="sxs-lookup"><span data-stu-id="17f91-109">For more information on configuring spam filter policies, see [Configure your spam filter policies](https://go.microsoft.com/fwlink/?linkid=2101431).</span></span>
