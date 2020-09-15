---
title: Kļūdas kods 0x15
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "919"
- "2000022"
ms.assetid: 0d566afe-b21f-4f1b-8ca9-4b4d3b0f5435
description: Ja, aktivizējot Office 2013 attālā datora pakalpojumu (RDS) izvietojumā, rodas kļūda, apsveriet iespēju iespējot ADAL, rediģējot reģistru.
ms.openlocfilehash: deb2ac4b0fb6a7b2e0045ff1b0ba95ad6e5e4a3a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47709194"
---
# <a name="error-while-activation-office-2013-on-remote-desktop-services"></a><span data-ttu-id="78a60-103">Kļūda, aktivizējot Office 2013 attālās darbvirsmas pakalpojumos</span><span class="sxs-lookup"><span data-stu-id="78a60-103">Error while activation Office 2013 on Remote Desktop Services</span></span>

<span data-ttu-id="78a60-104">Ja, aktivizējot Office 2013 attālā datora pakalpojumu (RDS) izvietojumā, rodas kļūda, apsveriet iespēju iespējot ADAL, rediģējot reģistru.</span><span class="sxs-lookup"><span data-stu-id="78a60-104">If you're receiving an error while activating Office 2013 on Remote Desktop Services (RDS) deployments, consider enabling ADAL by editing the registry.</span></span>
  
|<span data-ttu-id="78a60-105">**Reģistra atslēga**</span><span class="sxs-lookup"><span data-stu-id="78a60-105">**Registry key**</span></span>|<span data-ttu-id="78a60-106">**Ierakstiet**</span><span class="sxs-lookup"><span data-stu-id="78a60-106">**Type**</span></span>|<span data-ttu-id="78a60-107">**Vērtību**</span><span class="sxs-lookup"><span data-stu-id="78a60-107">**Value**</span></span>|
|:-----|:-----|:-----|
|<span data-ttu-id="78a60-108">HKEY_CURRENT_USER \Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span><span class="sxs-lookup"><span data-stu-id="78a60-108">HKEY_CURRENT_USER\Software\Microsoft\Office\15.0\Common\Identity\EnableADAL</span></span>  <br/> |<span data-ttu-id="78a60-109">REG_DWORD</span><span class="sxs-lookup"><span data-stu-id="78a60-109">REG_DWORD</span></span>  <br/> |<span data-ttu-id="78a60-110">1</span><span class="sxs-lookup"><span data-stu-id="78a60-110">1</span></span>  <br/> |

<span data-ttu-id="78a60-111">Lai iegūtu papildinformāciju, skatiet rakstu [modernās autentifikācijas iespējošana pakalpojumā Office 2013 Windows ierīcēs](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span><span class="sxs-lookup"><span data-stu-id="78a60-111">For more information, see [Enable Modern Authentication for Office 2013 on Windows devices](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication).</span></span>
  
> [!NOTE]
>  <span data-ttu-id="78a60-112">ADAL ir iespējota pēc noklusējuma Microsoft 365 programmās darbam ar Enterprise un Office 2016.</span><span class="sxs-lookup"><span data-stu-id="78a60-112">ADAL is enabled by default in Microsoft 365 Apps for enterprise and Office 2016.</span></span> <span data-ttu-id="78a60-113">Attālā datora pakalpojumu (RDS) iepriekš tika nosaukts termināļa pakalpojumi.</span><span class="sxs-lookup"><span data-stu-id="78a60-113">Remote Desktop Services (RDS) was previously named Terminal Services.</span></span>
  