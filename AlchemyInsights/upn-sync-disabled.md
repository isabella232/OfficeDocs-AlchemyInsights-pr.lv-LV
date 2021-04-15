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
# <a name="upn-sync-disabled"></a>UPN sinhronizācija ir atspējota

Ja sinhronizēšanu ar Azure AD sākāt līdz 2016. gada 30. martam, izpildiet šo Azure AD PowerShell cmdlet, lai iespējotu UPN soft atbilstību tikai jūsu organizācijai:
  
 **Set-MsolDirSyncFeature -Feature EnableSoftMatchOnUpn -Enable $True**
  
UPN softā atbilstība tiek automātiski ieslēgta organizācijām, kuras 2016. gada 30. martā vai pēc tās ir sākusi sinhronizēšanu ar Azure AD.
  
Papildinformāciju par klusās atbilstības iespējošanu UPN un citiem sinhronizācijas līdzekļiem skatiet rakstā [Azure AD Connect sinhronizācijas pakalpojuma līdzekļi.](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features)
  

