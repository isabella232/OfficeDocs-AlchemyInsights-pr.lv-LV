---
title: Problēmu novēršana saistībā ar iOS ierīču reģistrāciju programmā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823470"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problēmu novēršana saistībā ar iOS ierīču reģistrāciju programmā Microsoft Intune

Pārskatiet tālāk norādītos resursus, lai tūlīt novērstu savu problēmu. 
  
Daži bieži sastopami kļūdu ziņojumi un risinājuma darbības:
  
- **Sasniegts ierīces sākumburts** Lietotājam ir reģistrēts vairāk ierīču, nekā ierīces ierobežojums. Pārskatiet šos [dokumentus, lai noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) [vai mainītu ierīču ierobežojumu.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)
    
- **Šis pakalpojums netiek atbalstīts. Nav reģistrācijas politikas:** Apple pašpiegādes paziņojumu pakalpojums (APNS) ir jākonfigurē vai jāatjauno. Pārskatiet [šo](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) dokumentu, lai saņemtu norādījumus par to, kā to paveikt. 
    
- **Lietotāja licences tips nav derīgs vai lietotājvārds netiek atpazīts:** Lietotājam ir jābūt piešķirtai Intune vai EMS licencei. Pārskatiet šos dokumentus, lai piešķirtu licenci, [izmantojot Office administrēšanas centru](https://docs.microsoft.com/intune/licenses-assign) vai Azure [portālu.](https://docs.microsoft.com/azure/active-directory/license-users-groups)
    
Papildu resursi, lai palīdzētu novērst problēmu:
  
1. Izmantojiet [Intune problēmu novēršanas portālu,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lai diagnosticētu un novērstu bieži sastopamās reģistrācijas kļūmes. Pārskatiet [šo dokumentu,](https://docs.microsoft.com/intune/help-desk-operators) lai iegūtu papildinformāciju. 
    
2. Pārskatiet šos dokumentus, lai noskaidrotu bieži sastopamās kļūdas, kas neļauj veikt reģistrāciju, un to novēršanas darbības: [problēmu novēršanas norādījumi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) un [problēmu novēršanas dokuments](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Uzziniet, kā reģistrēt iOS ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

