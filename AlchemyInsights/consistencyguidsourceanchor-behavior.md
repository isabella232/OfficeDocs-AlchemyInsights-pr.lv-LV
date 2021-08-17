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
ms.openlocfilehash: 9b5765ff3c59b1312bead41a45a53478a96260df0567f006ab93c3ccfaf4be64
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54044347"
---
# <a name="consistencyguid--sourceanchor-behavior"></a>ConsistencyGuid /sourceAnchor darbība

Azure AD Savienošana (versija 1.1.524.0 un pēc tam) tagad atvieglo msDS-ConsistencyGuid kā sourceAnchor atribūta lietošanu. Izmantojot šo līdzekli, Azure AD Savienošana automātiski konfigurē sinhronizācijas kārtulas, lai:
  
- Izmantojiet msDS-ConsistencyGuid kā avotaanchor atribūtu lietotāja objektiem. ObjectGUID tiek lietots citiem objektu tipiem.
    
- Visiem lokālajiem AD lietotāju objektiem, kuru msDS-ConsistencyGuid atribūts nav aizpildīts, Azure AD Savienošana raksta savu objectGUID vērtību atpakaļ uz msDS-ConsistencyGuid atribūtu lokālajā Active Directory. Pēc msDS-ConsistencyGuid atribūta ir aizpildīts, Azure AD Savienošana pēc tam eksportē objektu uz Azure AD.
    
 **Piezīme.** Kad lokāls AD objekts tiek importēts programmā Azure AD Savienošana (tas tiek importēts AD savienotāja telpā un tiek projicēts objektā Metaverse), tā avota uzmācēja vērtību vairs nevar mainīt. Lai norādītu sourceAnchor vērtību dotam lokālajam AD objektam, konfigurējiet tā msDS-ConsistencyGuid atribūtu, pirms tas tiek importēts Azure AD Savienošana. 
  
Papildinformāciju par SourceAnchor un ConsistencyGuid skatiet [šajās sadaļās: Azure AD Savienošana: Noformējuma jēdzieni](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-design-concepts)
  

