---
title: ConsistencyGuid / sourceAnchor uzvedība
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: cb1b50792b07a1b3b69607bf2f6824141a15922f
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/22/2019
ms.locfileid: "30753109"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="50471-102">ConsistencyGuid / sourceAnchor uzvedība</span><span class="sxs-lookup"><span data-stu-id="50471-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="50471-103">Debeszils AD Connect (versija 1.1.524.0 un pēc) tagad veicina BKAS ConsistencyGuid kā sourceAnchor atribūtu izmantošana.</span><span class="sxs-lookup"><span data-stu-id="50471-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="50471-104">Lietojot šo līdzekli, Azure AD savienot automātiski konfigurē sinhronizācijas noteikumi:</span><span class="sxs-lookup"><span data-stu-id="50471-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="50471-105">MsDS-ConsistencyGuid kā sourceAnchor atribūtu lietošana lietotāja objektiem.</span><span class="sxs-lookup"><span data-stu-id="50471-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="50471-106">ObjectGUID tiek izmantots citu objekta tipu.</span><span class="sxs-lookup"><span data-stu-id="50471-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="50471-107">Par jebkuru dota lokālā AD lietotāja objektu, kuru balsta ConsistencyGuid atribūts nav apdzīvots, Azure AD savienojumu raksta tās objectGUID vērtību atpakaļ BKAS ConsistencyGuid atribūtu lokālā Active Directory.</span><span class="sxs-lookup"><span data-stu-id="50471-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="50471-108">Pēc tam, kad tiek ievietota BKAS ConsistencyGuid atribūtu, tad Azure AD savienot eksporta objekta debeszils reklāmu.</span><span class="sxs-lookup"><span data-stu-id="50471-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="50471-109">**Piezīme:** Reiz uz lokālo reklāmas objekts tiks importēts Azure AD savienojumu (t.i., ieved reklāmas savienotāja telpa un projicē Metaverse), tās sourceAnchor vērtību vairs nevar mainīt.</span><span class="sxs-lookup"><span data-stu-id="50471-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="50471-110">Lai norādītu vērtību sourceAnchor dota lokālā AD objektu, konfigurēt savas BKAS ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD savienojumu.</span><span class="sxs-lookup"><span data-stu-id="50471-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="50471-111">Lai iegūtu vairāk informācijas par SourceAnchor un ConsistencyGuid, atsaukties uz šādiem: [Azure AD savienot: projekta koncepcijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="50471-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

