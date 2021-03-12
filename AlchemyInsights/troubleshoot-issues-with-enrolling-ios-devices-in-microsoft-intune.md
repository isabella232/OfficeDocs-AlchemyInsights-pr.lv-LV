---
title: Problēmu novēršana saistībā ar iOS ierīču reģistrēšanu pakalpojumā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 4aef78e5921b789b532fecc99380da3274173bdb
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50708969"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a>Problēmu novēršana saistībā ar iOS ierīču reģistrēšanu pakalpojumā Microsoft Intune

Pārskatiet tālāk norādītos resursus, lai atrisinātu savu problēmu tūlīt. 
  
Daži bieži sastopami kļūdu ziņojumi un atrisināšanas darbības:
  
- **Sasniegts ierīces vāciņš** Lietotājam ir vairāk ierīču, kas reģistrējušies nekā ierīces ierobežojums. Pārskatiet šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) vai [mainītu ierīces ierobežojumu](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
- **Šis pakalpojums netiek atbalstīts. Nav reģistrācijas politikas:** Apple push Notification Service (APN) ir jākonfigurē vai jāatjauno. Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , lai saņemtu norādījumus par to, kā to izdarīt. 
    
- **Lietotāja licences tips ir nederīgs vai lietotājvārds nav atpazīts:** Lietotājam ir jāpiešķir Intune vai EMS licence. Pārskatiet šos dokumentus, lai piešķirtu licenci, izmantojot [Office administrēšanas centru](https://docs.microsoft.com/intune/licenses-assign) vai [Azure portālu](https://docs.microsoft.com/azure/active-directory/license-users-groups).
    
Papildu resursi, kas palīdz novērst problēmu:
  
1. Izmantojiet [Intune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu Biežākās reģistrācijas kļūmes. Lai iegūtu papildinformāciju, pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) . 
    
2. Pārskatiet šos dokumentus, lai skatītu sarakstu ar bieži sastopamām kļūdām, kas neļauj veikt reģistrāciju un risinājumus: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) un [problēmu novēršana](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).
    
3. [Uzziniet, kā reģistrēt iOS ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).
    

