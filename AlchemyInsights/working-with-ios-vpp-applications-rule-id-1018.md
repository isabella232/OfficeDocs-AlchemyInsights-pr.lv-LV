---
title: Darbs ar iOS. VPP programmas kārtulas Id 1018
ms.author: pebaum
author: pebaum
ms.date: 9/10/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 65b9a727171a7551068717f6327f15e1aa8e6bed
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32420491"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="d4137-102">Darbs ar iOS. VPP programmas</span><span class="sxs-lookup"><span data-stu-id="d4137-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="d4137-103">Izlasiet, [kā pārvaldīt iOS progr, kas iegādāta saskaņā ar lielapjoma pirkumu programmas ar Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) apgūt līdzekļus, ierobežojumus un pasākumus, lai padarītu izmantot Apple lielapjoma pirkumu programma un atbalsts Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="d4137-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span> 
  
 <span data-ttu-id="d4137-104">**Jautājumi:** "Mans lietotājiem ir piešķirt iOS VPP app, bet instalēšana neizdevās."</span><span class="sxs-lookup"><span data-stu-id="d4137-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span> 
  
- <span data-ttu-id="d4137-105">Tas var notikt, ja vienota VPP pilnvara tiek izmantota pāri vairākiem mobilo ierīču pārvaldības pakalpojumu sniedzējiem.</span><span class="sxs-lookup"><span data-stu-id="d4137-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="d4137-106">VPP žetoni no Apple, drīkst izmantot tikai ar vienu pakalpojumu sniedzēju.</span><span class="sxs-lookup"><span data-stu-id="d4137-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="d4137-107">Ja izmantojāt VPP pilnvara ar vairākiem pakalpojumu sniedzējiem, ir atkārtoti augšupielādēt Intune marķieri.</span><span class="sxs-lookup"><span data-stu-id="d4137-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>
    
- <span data-ttu-id="d4137-108">Instalēšana var arī neizdoties, ja kopējais iekārtu skaits pārsniedz nepieciešamo licenču skaitu.</span><span class="sxs-lookup"><span data-stu-id="d4137-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="d4137-109">Lai skatītu lietojuma pārskats par savām licencēm, dodieties uz **Intune Mobile apps** \> **App licences** lapa.</span><span class="sxs-lookup"><span data-stu-id="d4137-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="d4137-110">Lai uzzinātu, kā atņemt licences lietošanu, skatiet [šajā pantā.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="d4137-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
    

