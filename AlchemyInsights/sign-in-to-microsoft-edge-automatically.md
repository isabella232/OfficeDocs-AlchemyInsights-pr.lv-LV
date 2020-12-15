---
title: Automātiska pierakstīšanās pārlūkprogrammā Microsoft Edge
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 12/03/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003848"
- "6898"
ms.openlocfilehash: 68a1119abd0a3f687b6448bb6e58c6485c239c0f
ms.sourcegitcommit: 94036315916fbc79dca2a692c2e9bc1139dd28f6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/08/2020
ms.locfileid: "49677767"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automātiska pierakstīšanās pārlūkprogrammā Microsoft Edge

Microsoft Edge izmanto OS noklusējuma kontu, lai automātiski pierakstītos lietotājam atbilstoši lietotāja ierīces konfigurēšanai. 

Tālāk ir aprakstīti katra ierīces konfigurācijas tipa scenāriji un tā atkarīgā lietotāja pierakstīšanās process.

1. **Ierīce ir hibrīds/AAD-J**: šī opcija ir pieejama operētājsistēmā Windows 10, zemākā līmeņa Windows un atbilstošajās serveru versijās. Lietotāji automātiski ir pierakstījušies ar saviem Azure Active Directory (AD) kontiem.
2. **Ierīce ir savienota ar domēnu**: šī opcija ir pieejama Windows 10, zemākā līmeņa Windows un atbilstošajās serveru versijās. Pēc noklusējuma lietotāji ar domēnu kontiem netiek automātiski pierakstīti. lai iespējotu automātisku pierakstīšanos, izmantojiet **ConfigureOnPremisesAccountAutoSignIn** politiku. Lai iespējotu automātisku pierakstīšanos lietotājiem ar Azure AD kontiem, apsveriet iespēju hibrīdi savienojiet savas ierīces.
3. **OS noklusējuma konts ir Microsoft konts**: šī opcija ir pieejama operētājsistēmā Windows 10 RS3 (versija 1709, būvējums 10.0.16299) un jaunākās versijās. Scenārijs nav ticams, ka tas notiks uzņēmuma ierīcēs. Tomēr, ja OS noklusējuma konts ir Microsoft konts, Microsoft Edge automātiski pierakstīsies lietotājam ar Microsoft kontu.
 
 
