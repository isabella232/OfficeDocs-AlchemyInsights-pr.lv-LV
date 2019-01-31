---
title: ConsistencyGuid / sourceAnchor uzvedība
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 5/2/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 010474bcc4cc6f97bcaafef9dfe6f4accfed4247
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/30/2019
ms.locfileid: "29659598"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="4cc3b-102">ConsistencyGuid / sourceAnchor uzvedība</span><span class="sxs-lookup"><span data-stu-id="4cc3b-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="4cc3b-p101">Debeszils AD Connect (versija 1.1.524.0 un pēc) tagad veicina BKAS ConsistencyGuid kā sourceAnchor atribūtu izmantošana. Lietojot šo līdzekli, Azure AD savienot automātiski konfigurē sinhronizācijas noteikumi:</span><span class="sxs-lookup"><span data-stu-id="4cc3b-p101">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute. When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="4cc3b-p102">MsDS-ConsistencyGuid kā sourceAnchor atribūtu lietošana lietotāja objektiem. ObjectGUID tiek izmantots citu objekta tipu.</span><span class="sxs-lookup"><span data-stu-id="4cc3b-p102">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects. ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="4cc3b-p103">Par jebkuru dota lokālā AD lietotāja objektu, kuru balsta ConsistencyGuid atribūts nav apdzīvots, Azure AD savienojumu raksta tās objectGUID vērtību atpakaļ BKAS ConsistencyGuid atribūtu lokālā Active Directory. Pēc tam, kad tiek ievietota BKAS ConsistencyGuid atribūtu, tad Azure AD savienot eksporta objekta debeszils reklāmu.</span><span class="sxs-lookup"><span data-stu-id="4cc3b-p103">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory. After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="4cc3b-p104">**Piezīme:** Reiz uz lokālo reklāmas objekts tiks importēts Azure AD savienojumu (t.i., ieved reklāmas savienotāja telpa un projicē Metaverse), tās sourceAnchor vērtību vairs nevar mainīt. Lai norādītu vērtību sourceAnchor dota lokālā AD objektu, konfigurēt savas BKAS ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD savienojumu.</span><span class="sxs-lookup"><span data-stu-id="4cc3b-p104">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore. To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="4cc3b-111">Lai iegūtu vairāk informācijas par SourceAnchor un ConsistencyGuid, atsaukties uz šādiem: [Azure AD savienot: projekta koncepcijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="4cc3b-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

