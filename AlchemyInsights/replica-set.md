---
title: Dublikātu kopa
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004400"
- "9004395"
- "8265"
- "9276"
ms.openlocfilehash: 3834696ff59b7e96e90a5b660a489003dfa9729c
ms.sourcegitcommit: 581c696ec108184adae9d4bc8f47cb9247131de8
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50714250"
---
# <a name="replica-set"></a><span data-ttu-id="b43dc-102">Dublikātu kopa</span><span class="sxs-lookup"><span data-stu-id="b43dc-102">Replica set</span></span>

<span data-ttu-id="b43dc-103">AADDS tiek dēvēts arī par pārvaldīto domēnu.</span><span class="sxs-lookup"><span data-stu-id="b43dc-103">AADDS is also called as the managed domain.</span></span> <span data-ttu-id="b43dc-104">Faktiski tie ir divi domēnu kontrolleri, kurus vada un ko uztur backend.</span><span class="sxs-lookup"><span data-stu-id="b43dc-104">It is actually two domain controllers that are run and maintained by the backend.</span></span> <span data-ttu-id="b43dc-105">Divi DCs ietilpst viens galvenais DC un viens replicēšanas KONTROLLERis.</span><span class="sxs-lookup"><span data-stu-id="b43dc-105">The two DCs include one main DC and one replication DC.</span></span> <span data-ttu-id="b43dc-106">Dublējumkopijas pakalpojumā AADDS (Managed Domain) ir automatizēts process, ko pārvalda Azure Platform.</span><span class="sxs-lookup"><span data-stu-id="b43dc-106">Backups in AADDS (managed domain) are an automated process managed by the Azure platform.</span></span> <span data-ttu-id="b43dc-107">Ja rodas problēmas ar jūsu pārvaldīto domēnu, Azure atbalsts var palīdzēt veikt atjaunošanu no dublējuma.</span><span class="sxs-lookup"><span data-stu-id="b43dc-107">In the event of an issue with your managed domain, Azure support can assist you in restoring from backup.</span></span>

<span data-ttu-id="b43dc-108">Jūs izveidojat katru dublikātu kopu virtuālajā tīklā.</span><span class="sxs-lookup"><span data-stu-id="b43dc-108">You create each replica set in a virtual network.</span></span> <span data-ttu-id="b43dc-109">Katrs virtuālais tīkls ir jāvienādranga visos citos virtuālajos tīklos, kas vieso pārvaldītā domēna dublikātu kopu.</span><span class="sxs-lookup"><span data-stu-id="b43dc-109">Each virtual network must be peered to every other virtual network that hosts a managed domain's replica set.</span></span> <span data-ttu-id="b43dc-110">Šī konfigurācija izveido Mesh tīkla topoloģiju, kas atbalsta direktorija replicēšanu.</span><span class="sxs-lookup"><span data-stu-id="b43dc-110">This configuration creates a mesh network topology that supports directory replication.</span></span> <span data-ttu-id="b43dc-111">Virtuālais tīkls var atbalstīt vairākas dublikātu kopas, ja katra dublikātu kopa ir citā virtuālajā apakštīklā.</span><span class="sxs-lookup"><span data-stu-id="b43dc-111">A virtual network can support multiple replica sets, provided that each replica set is in a different virtual subnet.</span></span>

<span data-ttu-id="b43dc-112">Detalizētu informāciju par dublikātu kopu skatiet rakstā [jēdzienu dublikātu kopas](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span><span class="sxs-lookup"><span data-stu-id="b43dc-112">For more details on Replica set, see [Concepts Replica sets](https://docs.microsoft.com/azure/active-directory-domain-services/concepts-replica-sets).</span></span>
