---
title: ConsistencyGuid /sourceAnchor darbība
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: eafe1ec9636cddc9d73a88beb7ae3ad9f6fad660
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51816999"
---
# <a name="consistencyguid--sourceanchor-behavior"></a><span data-ttu-id="50646-102">ConsistencyGuid /sourceAnchor darbība</span><span class="sxs-lookup"><span data-stu-id="50646-102">ConsistencyGuid / sourceAnchor behavior</span></span>

<span data-ttu-id="50646-103">Azure AD Connect (versija 1.1.524.0 un pēc tam) tagad atvieglo msDS-ConsistencyGuid kā avotaanchor atribūta lietošanu.</span><span class="sxs-lookup"><span data-stu-id="50646-103">Azure AD Connect (version 1.1.524.0 and after) now facilitates the use of msDS-ConsistencyGuid as sourceAnchor attribute.</span></span> <span data-ttu-id="50646-104">Izmantojot šo līdzekli, Azure AD Connect automātiski konfigurē sinhronizācijas kārtulas, lai:</span><span class="sxs-lookup"><span data-stu-id="50646-104">When using this feature, Azure AD Connect automatically configures the synchronization rules to:</span></span>
  
- <span data-ttu-id="50646-105">Izmantojiet msDS-ConsistencyGuid kā avotaanchor atribūtu lietotāja objektiem.</span><span class="sxs-lookup"><span data-stu-id="50646-105">Use msDS-ConsistencyGuid as the sourceAnchor attribute for User objects.</span></span> <span data-ttu-id="50646-106">ObjectGUID tiek lietots citiem objektu tipiem.</span><span class="sxs-lookup"><span data-stu-id="50646-106">ObjectGUID is used for other object types.</span></span>
    
- <span data-ttu-id="50646-107">Visiem lokālajiem AD lietotāju objektiem, kuru msDS-ConsistencyGuid atribūts nav aizpildīts, Azure AD Connect raksta tās objectGUID vērtību atpakaļ uz msDS-ConsistencyGuid atribūtu lokālajā Active Directory.</span><span class="sxs-lookup"><span data-stu-id="50646-107">For any given on-premises AD User object whose msDS-ConsistencyGuid attribute isn't populated, Azure AD Connect writes its objectGUID value back to the msDS-ConsistencyGuid attribute in on-premises Active Directory.</span></span> <span data-ttu-id="50646-108">Pēc msDS-ConsistencyGuid atribūta ir aizpildīts, Azure AD Connect pēc tam eksportē objektu uz Azure AD.</span><span class="sxs-lookup"><span data-stu-id="50646-108">After the msDS-ConsistencyGuid attribute is populated, Azure AD Connect then exports the object to Azure AD.</span></span>
    
 <span data-ttu-id="50646-109">**Piezīme.** Kad lokāls AD objekts tiek importēts Azure AD Connect (tas tiek importēts AD savienotāja telpā un tiek projicēts objektā Metaverse), jūs vairs nevarat mainīt tā sourceAnchor vērtību.</span><span class="sxs-lookup"><span data-stu-id="50646-109">**Note:** Once an on-premises AD object is imported into Azure AD Connect (that is, imported into the AD Connector Space and projected into the Metaverse), you cannot change its sourceAnchor value anymore.</span></span> <span data-ttu-id="50646-110">Lai norādītu sourceAnchor vērtību dotam lokālajam AD objektam, konfigurējiet tā msDS-ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="50646-110">To specify the sourceAnchor value for a given on-premises AD object, configure its msDS-ConsistencyGuid attribute before it is imported into Azure AD Connect.</span></span> 
  
<span data-ttu-id="50646-111">Papildinformāciju par SourceAnchor un ConsistencyGuid skatiet [šajās sadaļās: Azure AD Connect: Noformējuma jēdzieni](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span><span class="sxs-lookup"><span data-stu-id="50646-111">For more information on SourceAnchor and ConsistencyGuid, refer to the following: [Azure AD Connect: Design concepts](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)</span></span>
  

