---
title: ConsistencyGuid/sourceAnchor darbība
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 6a44f797-acc7-4cbe-aa5a-47e2581fabf5
ms.openlocfilehash: 8527e7c2404742a999041f85ed12d78c48cc0d8c
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43705740"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor darbība

Azure AD savienojumu (Version 1.1.524.0 un pēc) tagad atvieglo izmantot BKAS-ConsistencyGuid kā sourceAnchor atribūtu. Izmantojot šo līdzekli, Azure AD Connect automātiski konfigurē sinhronizācijas kārtulas:
  
- Izmantojiet msDS-ConsistencyGuid kā sourceAnchor atribūtu lietotāja objektiem. ObjectGUID tiek izmantots citiem objektu tipiem.
    
- Jebkuru lokālo reklāmas lietotāja objekts, kura BKAS ConsistencyGuid atribūts nav aizpildīts, Azure AD savienojumu raksta objectGUID vērtību atpakaļ uz lokālo Active Directory atribūtu msDS-ConsistencyGuid. Pēc tam, kad BKAS ConsistencyGuid atribūts ir aizpildīts, Azure AD savienojumu pēc tam eksportē objektu Azure AD.
    
 **Piezīme:** Kad lokālas reklāmas objekts tiek importēts Azure AD savienojumu (tas ir, importēt uz AD Connector telpas un projicē metaverse), nevar mainīt tās sourceAnchor vērtība vairs. Lai norādītu lokālā reklāmas objekta sourceAnchor vērtību, konfigurējiet tā BKAS ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD savienojumu. 
  
Lai iegūtu papildinformāciju par SourceAnchor un ConsistencyGuid, skatiet šo: [AZURE ad Connect: dizaina koncepcijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

