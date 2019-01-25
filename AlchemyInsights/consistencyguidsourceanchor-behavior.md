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
ms.openlocfilehash: 80516ed9e15040475a8b65a1af98a1b561704d49
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/24/2019
ms.locfileid: "29498525"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor uzvedība

Debeszils AD Connect (versija 1.1.524.0 un pēc) tagad veicina BKAS ConsistencyGuid kā sourceAnchor atribūtu izmantošana. Lietojot šo līdzekli, Azure AD savienot automātiski konfigurē sinhronizācijas noteikumi:
  
- MsDS-ConsistencyGuid kā sourceAnchor atribūtu lietošana lietotāja objektiem. ObjectGUID tiek izmantots citu objekta tipu.
    
- Par jebkuru dota lokālā AD lietotāja objektu, kuru balsta ConsistencyGuid atribūts nav apdzīvots, Azure AD savienojumu raksta tās objectGUID vērtību atpakaļ BKAS ConsistencyGuid atribūtu lokālā Active Directory. Pēc tam, kad tiek ievietota BKAS ConsistencyGuid atribūtu, tad Azure AD savienot eksporta objekta debeszils reklāmu.
    
 **Piezīme:** Reiz uz lokālo reklāmas objekts tiks importēts Azure AD savienojumu (t.i., ieved reklāmas savienotāja telpa un projicē Metaverse), tās sourceAnchor vērtību vairs nevar mainīt. Lai norādītu vērtību sourceAnchor dota lokālā AD objektu, konfigurēt savas BKAS ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD savienojumu. 
  
Lai iegūtu vairāk informācijas par SourceAnchor un ConsistencyGuid, atsaukties uz šādiem: [Azure AD savienot: projekta koncepcijas](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

