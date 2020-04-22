---
title: Kļūdas kods 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ja saņemat kļūdas ziņojumu, aktivizējot Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietošanu, apsveriet iespēju iespējot ADAL, rediģējot reģistru.
ms.openlocfilehash: 566d63cbe37d295b3546b9d7d5b14dfc8e8fe0ec
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43703145"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="6d0a6-103">Kļūda, aktivizējot Office 2013 attālās darbvirsmas pakalpojumos</span><span class="sxs-lookup"><span data-stu-id="6d0a6-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="6d0a6-104">Ja saņemat kļūdas ziņojumu, aktivizējot Office 2013 attālās darbvirsmas pakalpojumu (RDS) izvietošanu, apsveriet iespēju iespējot ADAL, rediģējot reģistru.</span><span class="sxs-lookup"><span data-stu-id="6d0a6-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="6d0a6-105">**Reģistra atslēgu**</span><span class="sxs-lookup"><span data-stu-id="6d0a6-105">**Registry key**</span></span>|<span data-ttu-id="6d0a6-106">**Tipa**</span><span class="sxs-lookup"><span data-stu-id="6d0a6-106">**Type**</span></span>|<span data-ttu-id="6d0a6-107">**Vērtību**</span><span class="sxs-lookup"><span data-stu-id="6d0a6-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="6d0a6-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="6d0a6-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="6d0a6-109">Reg_dword</span><span class="sxs-lookup"><span data-stu-id="6d0a6-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="6d0a6-110">1</span><span class="sxs-lookup"><span data-stu-id="6d0a6-110">1</span></span>  <br/> |

<span data-ttu-id="6d0a6-111">Lai iegūtu papildinformāciju, skatiet [Iespējot mūsdienu autentifikācijas Office 2013 Windows ierīcēs](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="6d0a6-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="6d0a6-112">ADAL ir iespējota pēc noklusējuma Microsoft 365 lietojumprogrammas Enterprise un Office 2016.</span><span class="sxs-lookup"><span data-stu-id="6d0a6-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="6d0a6-113">Attālās darbvirsmas pakalpojumu (RDS) iepriekš tika nosaukts termināļa pakalpojumus.</span><span class="sxs-lookup"><span data-stu-id="6d0a6-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  