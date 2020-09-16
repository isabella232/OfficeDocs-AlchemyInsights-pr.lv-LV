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
# <a name="upn-sync-disabled"></a>UPN sinhronizēšana atspējota

Ja esat sācis sinhronizēt ar Azure AD līdz 30. martam 2016, palaidiet tālāk norādīto Azure AD PowerShell cmdlet, lai iespējotu UPN atspirdzinošu atbilstību tikai jūsu organizācijai:
  
 **Set-MsolDirSyncFeature-iezīme EnableSoftMatchOnUpn-iespējot $True**
  
UPN soft Match automātiski tiek ieslēgta organizācijām, kas sāka sinhronizēšanu ar Azure AD vai pēc 30. marta, 2016.
  
Lai uzzinātu vairāk par to, kā iespējot mīkstu atbilstību UPN un citos sinhronizācijas līdzekļos, skatiet rakstu [AZURE ad Connect sinhronizēšanas pakalpojuma līdzekļi](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

