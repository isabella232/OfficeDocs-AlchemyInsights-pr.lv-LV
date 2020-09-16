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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid/sourceAnchor darbība

Azure AD Connect (versija 1.1.524.0 un pēc tam) tagad atvieglo BKAS-ConsistencyGuid kā sourceAnchor atribūta lietošanu. Izmantojot šo līdzekli, Azure AD Connect automātiski konfigurē sinhronizācijas kārtulas uz:
  
- Izmantojiet msDS-ConsistencyGuid kā lietotāja objektu sourceAnchor atribūtu. ObjectGUID tiek izmantots citiem objektu tipiem.
    
- Jebkuram lokālam AD lietotāja objektam, kura msDS-ConsistencyGuid atribūts nav aizpildīts, Azure AD Connect raksta tā objectGUID vērtību atpakaļ uz msDS-ConsistencyGuid atribūtu lokālajā Active Directory. Pēc tam, kad msDS-ConsistencyGuid atribūts ir aizpildīts, Azure AD Connect pēc tam eksportē objektu uz Azure AD.
    
 **Piezīme:** Kad lokālais reklāmas objekts tiek importēts Azure AD Connect (tas ir, tiek importēts AD Connector vietā un projicēts metaverse), vairs nevar mainīt tā sourceAnchor vērtību. Lai norādītu sourceAnchor vērtību noteiktā lokālā reklāmas objektā, konfigurējiet tā msDS-ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD Connect. 
  
Papildinformāciju par SourceAnchor un ConsistencyGuid skatiet šeit: [AZURE ad Connect: noformējuma jēdzieni](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

