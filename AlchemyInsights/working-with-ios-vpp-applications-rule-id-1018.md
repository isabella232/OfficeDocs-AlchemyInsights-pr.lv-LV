---
title: Darbs ar iOS VPP lietojumprogrammu kārtulas ID 1018
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1018"
- "6700004"
ms.assetid: 2e51ae64-8ba2-42e1-9e3e-f4aad102c391
ms.openlocfilehash: 67800b261e7d670181b17783bc81e276d75026e0
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47688953"
---
# <a name="working-with-ios-vpp-applications"></a><span data-ttu-id="47ded-102">Darbs ar iOS VPP lietojumprogrammām</span><span class="sxs-lookup"><span data-stu-id="47ded-102">Working with iOS VPP Applications</span></span>

<span data-ttu-id="47ded-103">Izlasiet, [kā pārvaldīt iOS lietojumprogrammas, kas iegādātas, izmantojot lielapjoma pirkumu programmu, ar Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) , lai iegūtu informāciju par līdzekļiem, ierobežojumiem un darbībām, kas jāveic, lai izmantotu Apple lielapjoma pirkumu programmu un tās atbalstu pakalpojumā Microsoft Intune.</span><span class="sxs-lookup"><span data-stu-id="47ded-103">Read [How to manage iOS apps purchased through a volume-purchase program with Microsoft Intune](https://docs.microsoft.com/intune/vpp-apps-ios) to learn about features, constraints, and steps to make use of the Apple Volume Purchase Program and the support for it in Microsoft Intune.</span></span>
  
 <span data-ttu-id="47ded-104">**Biežāk sastopamās problēmas:** "Esmu piešķīris iOS VPP lietojumprogrammu saviem lietotājiem, taču instalēšana neizdevās."</span><span class="sxs-lookup"><span data-stu-id="47ded-104">**Common Issues:** "I assigned an iOS VPP app to my users, but the installation failed."</span></span>
  
- <span data-ttu-id="47ded-105">Tas var notikt, ja vairāku mobilo ierīču pārvaldības pakalpojumu sniedzēji izmanto vienu VPP žetonu.</span><span class="sxs-lookup"><span data-stu-id="47ded-105">This can happen if a single VPP token is used across multiple mobile device management providers.</span></span> <span data-ttu-id="47ded-106">VPP žetoni no Apple var tikt izmantoti tikai ar vienu pakalpojumu sniedzēju.</span><span class="sxs-lookup"><span data-stu-id="47ded-106">VPP tokens from Apple may only be used with one provider.</span></span> <span data-ttu-id="47ded-107">Ja izmantojāt VPP zīmi ar vairākiem pakalpojumu sniedzējiem, jums ir atkārtoti jāaugšupielādē pilnvara Intune.</span><span class="sxs-lookup"><span data-stu-id="47ded-107">If you used a VPP token with multiple providers, you must re-upload the token to Intune.</span></span>

- <span data-ttu-id="47ded-108">Instalēšana var neizdoties arī tad, ja instalācijas kopējais skaits pārsniedz licenču skaitu.</span><span class="sxs-lookup"><span data-stu-id="47ded-108">The installation can also fail if the total number of installations exceed the number of licenses.</span></span> <span data-ttu-id="47ded-109">Lai skatītu licenču lietojuma pārskatu, dodieties uz lapu **Intune Mobile Apps** \> **lietojumprogrammu licences** .</span><span class="sxs-lookup"><span data-stu-id="47ded-109">To view a usage report for your licenses, go to the **Intune Mobile apps** \> **App licenses** page.</span></span> <span data-ttu-id="47ded-110">Lai uzzinātu, kā atgūt licences izmantošanai, skatiet [šo rakstu.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span><span class="sxs-lookup"><span data-stu-id="47ded-110">To learn how to reclaim licenses in use, see [this article.](https://docs.microsoft.com/intune/vpp-apps-ios#revoking-app-licenses-and-deleting-tokens)</span></span>
