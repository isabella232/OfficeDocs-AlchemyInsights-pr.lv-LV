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
ms.openlocfilehash: 2a03ac64d92c07b523b015850251b33c58bb76f8
ms.sourcegitcommit: 03a156a9c9740521155a30775492c7dff0982588
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/22/2019
ms.locfileid: "30767243"
---
# <a name="upn-sync-disabled"></a>UPN sinhronizācijas atspējots

Ja startējāt sinhronizēšana debeszils reklāmu pirms 2016. gada 30. martā, palaidiet šādu Azure AD PowerShell cmdlet iespējot UPN mīkstu sakritību tikai sava uzņēmuma:
  
 **Kopa MsolDirSyncFeature-līdzeklis EnableSoftMatchOnUpn-iespējot $True**
  
UPN mīkstu spēles tiks automātiski ieslēgta organizācijām, kas sākta sinhronizēšana debeszils reklāmu vai pēc 2016. gada 30 marts.
  
Lai uzzinātu vairāk par to, mīkstu maču UPN un citas sinhronizēšanas funkcijas, lūdzu skatīt [Azure AD pievienot sinhronizācijas pakalpojumu iespējām](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsyncservice-features).
  

