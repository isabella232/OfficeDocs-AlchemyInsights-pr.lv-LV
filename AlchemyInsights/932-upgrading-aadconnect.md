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
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 8038d5ef768d6ee228db7d038ad71d926f4047f3
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29937951"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="28fa3-102">Jaunināšanas debeszils AD savienojumu</span><span class="sxs-lookup"><span data-stu-id="28fa3-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="28fa3-p101">Pēc noklusējuma ir iespējota automātiska jaunināšana Azure AD savienojumu, kas palīdz nodrošināt jūs lietojat jaunāko versiju. Lai pārbaudītu automātiskās jaunināšanas iestatījumus, izmantojiet cmdlet **Get ADSyncAutoUpgrade** Azure AD PowerShell. Cmdlet atgriež vienu no šīm vērtībām:</span><span class="sxs-lookup"><span data-stu-id="28fa3-p101">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version. To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell. The cmdlet will return one of following values:</span></span> 
  
- <span data-ttu-id="28fa3-106">**Enabled**: automātisks jauninājums ir iespējota.</span><span class="sxs-lookup"><span data-stu-id="28fa3-106">**Enabled**: Automatic upgrade is enabled.</span></span> 
    
- <span data-ttu-id="28fa3-107">**Atspējots**: automātisks jauninājums ir atspējota.</span><span class="sxs-lookup"><span data-stu-id="28fa3-107">**Disabled**: Automatic upgrade is disabled.</span></span> 
    
- <span data-ttu-id="28fa3-p102">**Apturēts**: sistēma vairs nav tiesības saņemt automātisku jaunināšanu. Nevar konfigurēt šo vērtību; to iestata sistēma.</span><span class="sxs-lookup"><span data-stu-id="28fa3-p102">**Suspended**: The system is no longer eligible to receive automatic upgrades. You can't configure this value; it's set by the system.</span></span> 
    
<span data-ttu-id="28fa3-110">Papildinformāciju skatiet sadaļā [Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="28fa3-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>
  
<span data-ttu-id="28fa3-111">Lai lejupielādētu jaunāko versiju Azure AD savienojumu, dodieties uz [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="28fa3-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
  

