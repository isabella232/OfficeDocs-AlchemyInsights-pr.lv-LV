---
title: UPN sinhronizācija ir atspējota
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: 2b1ba772459091ce1a796884997fe2516d0407eb
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51782158"
---
# <a name="upn-sync-disabled"></a><span data-ttu-id="806b1-102">UPN sinhronizācija ir atspējota</span><span class="sxs-lookup"><span data-stu-id="806b1-102">UPN sync disabled</span></span>

<span data-ttu-id="806b1-103">Ja sinhronizēšanu ar Azure AD sākāt līdz 2016. gada 30. martam, izpildiet šo Azure AD PowerShell cmdlet, lai iespējotu UPN soft atbilstību tikai jūsu organizācijai:</span><span class="sxs-lookup"><span data-stu-id="806b1-103">If you started syncing to Azure AD before March 30, 2016, run the following Azure AD PowerShell cmdlet to enable UPN soft match for your organization only:</span></span>
  
 <span data-ttu-id="806b1-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span><span class="sxs-lookup"><span data-stu-id="806b1-104">**Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**</span></span>
  
<span data-ttu-id="806b1-105">UPN softā atbilstība tiek automātiski ieslēgta organizācijām, kuras 2016. gada 30. martā vai pēc tās ir sākusi sinhronizēšanu ar Azure AD.</span><span class="sxs-lookup"><span data-stu-id="806b1-105">UPN soft match is automatically turned on for organizations that started syncing to Azure AD on or after March 30, 2016.</span></span>
  
<span data-ttu-id="806b1-106">Papildinformāciju par klusās atbilstības iespējošanu UPN un citiem sinhronizācijas līdzekļiem skatiet rakstā [Azure AD Connect sinhronizācijas pakalpojuma līdzekļi.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)</span><span class="sxs-lookup"><span data-stu-id="806b1-106">To learn more about enabling soft match on UPN and other sync features, please see [Azure AD Connect sync service features](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).</span></span>
  

