---
title: 932 modernizāciju AADConnect
ms.author: chrisda
author: chrisda
manager: serdars
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom: 932
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 0bbb847bb1381330065ebba6e109795908b06490
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/22/2019
ms.locfileid: "30778748"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="fb445-102">Jaunināšanas debeszils AD savienojumu</span><span class="sxs-lookup"><span data-stu-id="fb445-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="fb445-103">Pēc noklusējuma ir iespējota automātiska jaunināšana Azure AD savienojumu, kas palīdz nodrošināt jūs lietojat jaunāko versiju.</span><span class="sxs-lookup"><span data-stu-id="fb445-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="fb445-104">Lai pārbaudītu automātiskās jaunināšanas iestatījumus, izmantojiet cmdlet **Get ADSyncAutoUpgrade** Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="fb445-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="fb445-105">Cmdlet atgriež vienu no šīm vērtībām:</span><span class="sxs-lookup"><span data-stu-id="fb445-105">The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="fb445-106">**Enabled**: automātisks jauninājums ir iespējota.</span><span class="sxs-lookup"><span data-stu-id="fb445-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="fb445-107">**Atspējots**: automātisks jauninājums ir atspējota.</span><span class="sxs-lookup"><span data-stu-id="fb445-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="fb445-108">**Apturēts**: sistēma vairs nav tiesības saņemt automātisku jaunināšanu.</span><span class="sxs-lookup"><span data-stu-id="fb445-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="fb445-109">Nevar konfigurēt šo vērtību; to iestata sistēma.</span><span class="sxs-lookup"><span data-stu-id="fb445-109">You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="fb445-110">Papildinformāciju skatiet sadaļā [Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="fb445-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="fb445-111">Lai lejupielādētu jaunāko versiju Azure AD savienojumu, dodieties uz [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="fb445-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

