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
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="2c6cd-102">Automātiska pierakstīšanās microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="2c6cd-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="2c6cd-103">Microsoft Edge izmanto OS noklusējuma kontu, lai automātiski pierakstītos lietotājam atbilstoši tam, kā ir konfigurēta lietotāja ierīce.</span><span class="sxs-lookup"><span data-stu-id="2c6cd-103">Microsoft Edge uses the OS default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="2c6cd-104">Tālāk ir aprakstīti katra ierīces konfigurācijas tipa un tā atkarīgā lietotāja pierakstīšanās procesa scenāriji.</span><span class="sxs-lookup"><span data-stu-id="2c6cd-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

- <span data-ttu-id="2c6cd-105">**Ierīce ir hibrīda/AAD-J:** Šī opcija ir pieejama sistēmā Windows 10, lejupvērstā līmenī un atbilstošās servera versijās.</span><span class="sxs-lookup"><span data-stu-id="2c6cd-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="2c6cd-106">Lietotāji tiek automātiski pierakstīti ar savu Azure Active Directory (AD) kontu.</span><span class="sxs-lookup"><span data-stu-id="2c6cd-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
- <span data-ttu-id="2c6cd-107">**Ierīcei ir pievienots domēns**: šī opcija ir pieejama sistēmā Windows 10, lejupvērstā līmeņa Windows un atbilstošās servera versijās.</span><span class="sxs-lookup"><span data-stu-id="2c6cd-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="2c6cd-108">Pēc noklusējuma lietotāji ar domēnu kontiem netiek pierakstīti automātiski. lai iespējotu automātisko pierakstīšanos, izmantojiet **politiku ConfigureOnPremisesAccountAutoSignIn.**</span><span class="sxs-lookup"><span data-stu-id="2c6cd-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="2c6cd-109">Lai iespējotu automātisko pierakstīšanās lietotājiem ar Azure AD kontiem, apsveriet iespēju hibrīda pievienošanās savām ierīcēm.</span><span class="sxs-lookup"><span data-stu-id="2c6cd-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
- <span data-ttu-id="2c6cd-110">**Operētājsistēmas noklusējuma** konts ir Microsoft konts: šī opcija ir pieejama operētājsistēmā Windows 10 RS3 (versija 1709, būvējums 10.0.16299) un jaunākās versijās.</span><span class="sxs-lookup"><span data-stu-id="2c6cd-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="2c6cd-111">Maz ticams, ka scenārijs ir sastopama uzņēmuma ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="2c6cd-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="2c6cd-112">Tomēr, ja OS noklusējuma konts ir Microsoft konts, Microsoft Edge automātiski pierakstīs lietotāju ar Microsoft kontu.</span><span class="sxs-lookup"><span data-stu-id="2c6cd-112">However, if the OS default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
