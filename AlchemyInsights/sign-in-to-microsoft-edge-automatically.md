---
title: Automātiska pierakstīšanās microsoft Edge
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
ms.openlocfilehash: 6021991c125f5cb2a33ce8db8fe7717b528bf49b
ms.sourcegitcommit: 6bfe9cd9d0b18481e0cac6f1f5bc86ed7df31037
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/27/2021
ms.locfileid: "51398736"
---
# <a name="sign-in-to-microsoft-edge-automatically"></a>Automātiska pierakstīšanās microsoft Edge

Microsoft Edge izmanto OS noklusējuma kontu, lai automātiski pierakstītos lietotājam atbilstoši tam, kā ir konfigurēta lietotāja ierīce. 

Tālāk ir aprakstīti katra ierīces konfigurācijas tipa un tā atkarīgā lietotāja pierakstīšanās procesa scenāriji.

- **Ierīce ir hibrīda/AAD-J:** Šī opcija ir pieejama sistēmā Windows 10, lejupvērstā līmenī un atbilstošās servera versijās. Lietotāji tiek automātiski pierakstīti ar savu Azure Active Directory (AD) kontu.
- **Ierīcei ir pievienots domēns**: šī opcija ir pieejama sistēmā Windows 10, lejupvērstā līmeņa Windows un atbilstošās servera versijās. Pēc noklusējuma lietotāji ar domēnu kontiem netiek pierakstīti automātiski. lai iespējotu automātisko pierakstīšanos, izmantojiet **politiku ConfigureOnPremisesAccountAutoSignIn.** Lai iespējotu automātisko pierakstīšanās lietotājiem ar Azure AD kontiem, apsveriet iespēju hibrīda pievienošanās savām ierīcēm.
- **Operētājsistēmas noklusējuma** konts ir Microsoft konts: šī opcija ir pieejama operētājsistēmā Windows 10 RS3 (versija 1709, būvējums 10.0.16299) un jaunākās versijās. Maz ticams, ka scenārijs ir sastopama uzņēmuma ierīcēs. Tomēr, ja OS noklusējuma konts ir Microsoft konts, Microsoft Edge automātiski pierakstīs lietotāju ar Microsoft kontu.
 
 
