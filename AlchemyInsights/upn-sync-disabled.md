---
title: UPN sinhronizācijas atspējots
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: Adm_O365
ms.assetid: 2a3489fe-c2a8-4e43-96c2-be4b3c5e978c
ms.openlocfilehash: d00f10688ec775c22d60a9089e291c265ada46f1
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/24/2019
ms.locfileid: "29479390"
---
# <a name="upn-sync-disabled"></a>UPN sinhronizācijas atspējots

Ja startējāt sinhronizēšana debeszils reklāmu pirms 2016. gada 30. martā, palaidiet šādu Azure AD PowerShell cmdlet iespējot UPN mīkstu sakritību tikai sava uzņēmuma:
  
 **Kopa MsolDirSyncFeature-līdzeklis EnableSoftMatchOnUpn-iespējot $True**
  
UPN mīkstu spēles tiks automātiski ieslēgta organizācijām, kas sākta sinhronizēšana debeszils reklāmu vai pēc 2016. gada 30 marts.
  
Lai uzzinātu vairāk par to, mīkstu maču UPN un citas sinhronizēšanas funkcijas, lūdzu skatīt [Azure AD pievienot sinhronizācijas pakalpojumu iespējām](https://docs.microsoft.com/en-us/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

