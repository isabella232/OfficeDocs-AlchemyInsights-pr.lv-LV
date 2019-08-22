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
ms.openlocfilehash: f0ff94a8e46f1fb4e0ac8653c51f8f651e29498b
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36516996"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid / sourceAnchor uzvedība

Debeszils AD Connect (versija 1.1.524.0 un pēc) tagad veicina BKAS ConsistencyGuid kā sourceAnchor atribūtu izmantošana. Lietojot šo līdzekli, Azure AD savienot automātiski konfigurē sinhronizācijas noteikumi:
  
- MsDS-ConsistencyGuid kā sourceAnchor atribūtu lietošana lietotāja objektiem. ObjectGUID tiek izmantots citu objekta tipu.
    
- Par jebkuru dota lokālā AD lietotāja objektu, kuru balsta ConsistencyGuid atribūts nav apdzīvots, Azure AD savienojumu raksta tās objectGUID vērtību atpakaļ BKAS ConsistencyGuid atribūtu lokālā Active Directory. Pēc tam, kad tiek ievietota BKAS ConsistencyGuid atribūtu, tad Azure AD savienot eksporta objekta debeszils reklāmu.
    
 **Piezīme:** Reiz uz lokālo reklāmas objekts tiks importēts Azure AD savienojumu (t.i., ieved reklāmas savienotāja telpa un projicē Metaverse), tās sourceAnchor vērtību vairs nevar mainīt. Lai norādītu vērtību sourceAnchor dota lokālā AD objektu, konfigurēt savas BKAS ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD savienojumu. 
  
Lai iegūtu vairāk informācijas par SourceAnchor un ConsistencyGuid, atsaukties uz šādiem: [Azure AD savienot: projekta koncepcijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

