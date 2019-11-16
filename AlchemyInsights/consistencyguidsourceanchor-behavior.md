---
title: ConsistencyGuid/sourceAnchor darbība
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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: b43f77221f47b50c41197a448a9c26c423ce1ad5
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/15/2019
ms.locfileid: "36516996"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor darbība

Azure AD savienojumu (Version 1.1.524.0 un pēc) tagad atvieglo izmantot BKAS-ConsistencyGuid kā sourceAnchor atribūtu. Izmantojot šo līdzekli, Azure AD Connect automātiski konfigurē sinhronizācijas kārtulas:
  
- Izmantojiet msDS-ConsistencyGuid kā sourceAnchor atribūtu lietotāja objektiem. ObjectGUID tiek izmantots citiem objektu tipiem.
    
- Jebkuru lokālo reklāmas lietotāja objekts, kura BKAS ConsistencyGuid atribūts nav aizpildīts, Azure AD savienojumu raksta objectGUID vērtību atpakaļ uz lokālo Active Directory atribūtu msDS-ConsistencyGuid. Pēc tam, kad BKAS ConsistencyGuid atribūts ir aizpildīts, Azure AD savienojumu pēc tam eksportē objektu Azure AD.
    
 **Piezīme:** Kad lokālas reklāmas objekts tiek importēts Azure AD savienojumu (tas ir, importēt uz AD Connector telpas un projicē metaverse), nevar mainīt tās sourceAnchor vērtība vairs. Lai norādītu lokālā reklāmas objekta sourceAnchor vērtību, konfigurējiet tā BKAS ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD savienojumu. 
  
Lai iegūtu papildinformāciju par SourceAnchor un ConsistencyGuid, skatiet šo: [AZURE ad Connect: dizaina koncepcijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

