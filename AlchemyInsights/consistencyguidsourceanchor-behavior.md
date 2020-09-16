---
title: ConsistencyGuid/sourceAnchor darbība
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: adac469328485696d1ee1532aa3d6828af0642eb
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47756290"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="92269-102">ConsistencyGuid/sourceAnchor darbība</span><span class="sxs-lookup"><span data-stu-id="92269-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="92269-103">Azure AD Connect (versija 1.1.524.0 un pēc tam) tagad atvieglo BKAS-ConsistencyGuid kā sourceAnchor atribūta lietošanu.</span><span class="sxs-lookup"><span data-stu-id="92269-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="92269-104">Izmantojot šo līdzekli, Azure AD Connect automātiski konfigurē sinhronizācijas kārtulas uz:</span><span class="sxs-lookup"><span data-stu-id="92269-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="92269-105">Izmantojiet msDS-ConsistencyGuid kā lietotāja objektu sourceAnchor atribūtu.</span><span class="sxs-lookup"><span data-stu-id="92269-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="92269-106">ObjectGUID tiek izmantots citiem objektu tipiem.</span><span class="sxs-lookup"><span data-stu-id="92269-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="92269-107">Jebkuram lokālam AD lietotāja objektam, kura msDS-ConsistencyGuid atribūts nav aizpildīts, Azure AD Connect raksta tā objectGUID vērtību atpakaļ uz msDS-ConsistencyGuid atribūtu lokālajā Active Directory.</span><span class="sxs-lookup"><span data-stu-id="92269-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="92269-108">Pēc tam, kad msDS-ConsistencyGuid atribūts ir aizpildīts, Azure AD Connect pēc tam eksportē objektu uz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="92269-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="92269-109">**Piezīme:** Kad lokālais reklāmas objekts tiek importēts Azure AD Connect (tas ir, tiek importēts AD Connector vietā un projicēts metaverse), vairs nevar mainīt tā sourceAnchor vērtību.</span><span class="sxs-lookup"><span data-stu-id="92269-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="92269-110">Lai norādītu sourceAnchor vērtību noteiktā lokālā reklāmas objektā, konfigurējiet tā msDS-ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="92269-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="92269-111">Papildinformāciju par SourceAnchor un ConsistencyGuid skatiet šeit: [AZURE ad Connect: noformējuma jēdzieni](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="92269-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

