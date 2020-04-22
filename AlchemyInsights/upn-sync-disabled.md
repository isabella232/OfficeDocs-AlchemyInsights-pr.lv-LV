---
title: UPN sinhronizācijas atspējots
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 33bc7e30d41ff70e2ce55d946202acf45dbcb0f2
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43726111"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="637d0-102">UPN sinhronizācijas atspējots</span><span class="sxs-lookup"><span data-stu-id="637d0-102">UPN sync disabled</span></span>

<span data-ttu-id="637d0-103">Ja esat sācis sinhronizāciju Azure AD pirms 30. marts 2016, palaidiet šādu Azure AD PowerShell cmdlet, lai iespējotu UPN izvēles atbilstību tikai jūsu organizācijai:</span><span class="sxs-lookup"><span data-stu-id="637d0-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="637d0-104">**Set MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-iespējot $True**</span><span class="sxs-lookup"><span data-stu-id="637d0-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="637d0-105">UPN izvēles atbilstība tiek automātiski ieslēgta organizācijām, kas sāka sinhronizāciju Azure AD vai pēc 30. marts 2016.</span><span class="sxs-lookup"><span data-stu-id="637d0-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="637d0-106">Lai iegūtu papildinformāciju par iespējojot izvēles atbilstību UPN un citus sinhronizācijas līdzekļus, lūdzu, skatiet [AZURE ad savienojumu sinhronizācijas pakalpojuma līdzekļi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="637d0-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

