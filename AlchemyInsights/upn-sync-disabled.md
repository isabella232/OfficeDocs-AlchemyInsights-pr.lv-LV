---
title: UPN sinhronizācijas atspējots
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: f390d659b191fa4c44bd7c8acb32409cd3021489
ms.sourcegitcommit: 1d98db8acb9959aba3b5e308a567ade6b62da56c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/22/2019
ms.locfileid: "36532338"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="dd23d-102">UPN sinhronizācijas atspējots</span><span class="sxs-lookup"><span data-stu-id="dd23d-102">UPN sync disabled</span></span>

<span data-ttu-id="dd23d-103">Ja startējāt sinhronizēšana debeszils reklāmu pirms 2016. gada 30. martā, palaidiet šādu Azure AD PowerShell cmdlet iespējot UPN mīkstu sakritību tikai sava uzņēmuma:</span><span class="sxs-lookup"><span data-stu-id="dd23d-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="dd23d-104">**Kopa MsolDirSyncFeature-līdzeklis EnableSoftMatchOnUpn-iespējot $True**</span><span class="sxs-lookup"><span data-stu-id="dd23d-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="dd23d-105">UPN mīkstu spēles tiks automātiski ieslēgta organizācijām, kas sākta sinhronizēšana debeszils reklāmu vai pēc 2016. gada 30 marts.</span><span class="sxs-lookup"><span data-stu-id="dd23d-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="dd23d-106">Lai uzzinātu vairāk par to, mīkstu maču UPN un citas sinhronizēšanas funkcijas, lūdzu skatīt [Azure AD pievienot sinhronizācijas pakalpojumu iespējām](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="dd23d-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

