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
# <a name="upn-sync-disabled"></a>UPN sinhronizācijas atspējots

Ja esat sācis sinhronizāciju Azure AD pirms 30. marts 2016, palaidiet šādu Azure AD PowerShell cmdlet, lai iespējotu UPN izvēles atbilstību tikai jūsu organizācijai:
  
 **Set MsolDirSyncFeature-Feature EnableSoftMatchOnUpn-iespējot $True**
  
UPN izvēles atbilstība tiek automātiski ieslēgta organizācijām, kas sāka sinhronizāciju Azure AD vai pēc 30. marts 2016.
  
Lai iegūtu papildinformāciju par iespējojot izvēles atbilstību UPN un citus sinhronizācijas līdzekļus, lūdzu, skatiet [AZURE ad savienojumu sinhronizācijas pakalpojuma līdzekļi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

