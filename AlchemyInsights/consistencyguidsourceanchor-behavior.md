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
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid /sourceAnchor darbība

Azure AD Connect (versija 1.1.524.0 un pēc tam) tagad atvieglo msDS-ConsistencyGuid kā avotaanchor atribūta lietošanu. Izmantojot šo līdzekli, Azure AD Connect automātiski konfigurē sinhronizācijas kārtulas, lai:
  
- Izmantojiet msDS-ConsistencyGuid kā avotaanchor atribūtu lietotāja objektiem. ObjectGUID tiek lietots citiem objektu tipiem.
    
- Visiem lokālajiem AD lietotāju objektiem, kuru msDS-ConsistencyGuid atribūts nav aizpildīts, Azure AD Connect raksta tās objectGUID vērtību atpakaļ uz msDS-ConsistencyGuid atribūtu lokālajā Active Directory. Pēc msDS-ConsistencyGuid atribūta ir aizpildīts, Azure AD Connect pēc tam eksportē objektu uz Azure AD.
    
 **Piezīme.** Kad lokāls AD objekts tiek importēts Azure AD Connect (tas tiek importēts AD savienotāja telpā un tiek projicēts objektā Metaverse), jūs vairs nevarat mainīt tā sourceAnchor vērtību. Lai norādītu sourceAnchor vērtību dotam lokālajam AD objektam, konfigurējiet tā msDS-ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD Connect. 
  
Papildinformāciju par SourceAnchor un ConsistencyGuid skatiet [šajās sadaļās: Azure AD Connect: Noformējuma jēdzieni](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

