---
title: Automātiska pierakstīšanās pakalpojumā Microsoft Edge
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
- "8333"
- "9004625"
ms.openlocfilehash: 4e069a1c75caabf3bef7387140edd5650cf966856b888b5c6b5618a603986d6d
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54050701"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automātiska pierakstīšanās pakalpojumā Microsoft Edge

Microsoft Edge izmanto OS noklusējuma kontu, lai automātiski pierakstītos lietotāju atbilstoši tam, kā ir konfigurēta lietotāja ierīce. 

Tālāk ir aprakstīti katra ierīces konfigurācijas tipa un tā atkarīgā lietotāja pierakstīšanās procesa scenāriji.

- **Ierīce ir hibrīda/AAD-J:** Šī opcija ir pieejama Windows 10, lejupvērstā līmeņa Windows un atbilstošās servera versijās. Lietotāji tiek automātiski pierakstīti ar savu Azure Active Directory (AD) kontu.
- **Ierīcei ir pievienots domēns**: šī opcija ir pieejama pakalpojumā Windows 10, lejupvērstā Windows un atbilstošās servera versijās. Pēc noklusējuma lietotāji ar domēnu kontiem netiek pierakstīti automātiski. lai iespējotu automātisko pierakstīšanos, izmantojiet **politiku ConfigureOnPremisesAccountAutoSignIn.** Lai iespējotu automātisko pierakstīšanās lietotājiem ar Azure AD kontiem, apsveriet iespēju hibrīda pievienošanās savām ierīcēm.
- **Operētājsistēmas noklusējuma** konts ir Microsoft konts: šī opcija ir pieejama versijā Windows 10 RS3 (versija 1709, būvējums 10.0.16299) un jaunākās versijās. Maz ticams, ka scenārijs ir sastopama uzņēmuma ierīcēs. Tomēr, ja OS noklusējuma konts ir Microsoft konts, Microsoft Edge automātiski pierakstīsies lietotājs ar Microsoft kontu.
 
 
