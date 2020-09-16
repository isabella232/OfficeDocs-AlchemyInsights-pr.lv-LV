---
title: UPN sinhronizēšana atspējota
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 31947d7c491e4116ffdb9baadf286cd4fbb50f2a
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47749521"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="08f2e-102">UPN sinhronizēšana atspējota</span><span class="sxs-lookup"><span data-stu-id="08f2e-102">UPN sync disabled</span></span>

<span data-ttu-id="08f2e-103">Ja esat sācis sinhronizēt ar Azure AD līdz 30. martam 2016, palaidiet tālāk norādīto Azure AD PowerShell cmdlet, lai iespējotu UPN atspirdzinošu atbilstību tikai jūsu organizācijai:</span><span class="sxs-lookup"><span data-stu-id="08f2e-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="08f2e-104">**Set-MsolDirSyncFeature-iezīme EnableSoftMatchOnUpn-iespējot $True**</span><span class="sxs-lookup"><span data-stu-id="08f2e-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="08f2e-105">UPN soft Match automātiski tiek ieslēgta organizācijām, kas sāka sinhronizēšanu ar Azure AD vai pēc 30. marta, 2016.</span><span class="sxs-lookup"><span data-stu-id="08f2e-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="08f2e-106">Lai uzzinātu vairāk par to, kā iespējot mīkstu atbilstību UPN un citos sinhronizācijas līdzekļos, skatiet rakstu [AZURE ad Connect sinhronizēšanas pakalpojuma līdzekļi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span><span class="sxs-lookup"><span data-stu-id="08f2e-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

