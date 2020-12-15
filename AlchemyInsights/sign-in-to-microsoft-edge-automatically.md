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
# <a name="sign-in-to-microsoft-edge-automatically"></a><span data-ttu-id="bea36-102">Automātiska pierakstīšanās pārlūkprogrammā Microsoft Edge</span><span class="sxs-lookup"><span data-stu-id="bea36-102">Sign in to Microsoft Edge automatically</span></span>

<span data-ttu-id="bea36-103">Microsoft Edge izmanto OS noklusējuma kontu, lai automātiski pierakstītos lietotājam atbilstoši lietotāja ierīces konfigurēšanai.</span><span class="sxs-lookup"><span data-stu-id="bea36-103">Microsoft Edge uses the OS's default account to automatically sign in a user according to how the user's device is configured.</span></span> 

<span data-ttu-id="bea36-104">Tālāk ir aprakstīti katra ierīces konfigurācijas tipa scenāriji un tā atkarīgā lietotāja pierakstīšanās process.</span><span class="sxs-lookup"><span data-stu-id="bea36-104">The scenarios of each type of device configuration and its dependent user sign-in process are described below:</span></span>

1. <span data-ttu-id="bea36-105">**Ierīce ir hibrīds/AAD-J**: šī opcija ir pieejama operētājsistēmā Windows 10, zemākā līmeņa Windows un atbilstošajās serveru versijās.</span><span class="sxs-lookup"><span data-stu-id="bea36-105">**The device is hybrid/AAD-J**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="bea36-106">Lietotāji automātiski ir pierakstījušies ar saviem Azure Active Directory (AD) kontiem.</span><span class="sxs-lookup"><span data-stu-id="bea36-106">Users are automatically signed in with their Azure Active Directory (AD)accounts.</span></span>
2. <span data-ttu-id="bea36-107">**Ierīce ir savienota ar domēnu**: šī opcija ir pieejama Windows 10, zemākā līmeņa Windows un atbilstošajās serveru versijās.</span><span class="sxs-lookup"><span data-stu-id="bea36-107">**The device is domain-joined**: This option is available on Windows 10, down-level Windows, and corresponding server versions.</span></span> <span data-ttu-id="bea36-108">Pēc noklusējuma lietotāji ar domēnu kontiem netiek automātiski pierakstīti. lai iespējotu automātisku pierakstīšanos, izmantojiet **ConfigureOnPremisesAccountAutoSignIn** politiku.</span><span class="sxs-lookup"><span data-stu-id="bea36-108">By default, users with domain accounts are not signed in automatically; to enable automatic sign-in for them, use the **ConfigureOnPremisesAccountAutoSignIn** policy.</span></span> <span data-ttu-id="bea36-109">Lai iespējotu automātisku pierakstīšanos lietotājiem ar Azure AD kontiem, apsveriet iespēju hibrīdi savienojiet savas ierīces.</span><span class="sxs-lookup"><span data-stu-id="bea36-109">To enable automatic sign-in for users with Azure AD accounts, consider hybrid-joining their devices.</span></span>
3. <span data-ttu-id="bea36-110">**OS noklusējuma konts ir Microsoft konts**: šī opcija ir pieejama operētājsistēmā Windows 10 RS3 (versija 1709, būvējums 10.0.16299) un jaunākās versijās.</span><span class="sxs-lookup"><span data-stu-id="bea36-110">**The OS's default account is a Microsoft account**: This option is available on Windows 10 RS3 (version 1709, build 10.0.16299) and later versions.</span></span> <span data-ttu-id="bea36-111">Scenārijs nav ticams, ka tas notiks uzņēmuma ierīcēs.</span><span class="sxs-lookup"><span data-stu-id="bea36-111">The scenario is unlikely to occur on enterprise devices.</span></span> <span data-ttu-id="bea36-112">Tomēr, ja OS noklusējuma konts ir Microsoft konts, Microsoft Edge automātiski pierakstīsies lietotājam ar Microsoft kontu.</span><span class="sxs-lookup"><span data-stu-id="bea36-112">However, if the OS's default account is a Microsoft account, then Microsoft Edge will automatically sign in the user with the Microsoft account.</span></span>
 
 
