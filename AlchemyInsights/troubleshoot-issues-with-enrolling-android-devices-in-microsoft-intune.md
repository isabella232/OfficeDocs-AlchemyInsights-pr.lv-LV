---
title: Problēmu novēršana saistībā ar Android ierīču reģistrēšanu pakalpojumā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: cc8c68a1e838f67c4510002b2c7ff5294a4649fe
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709005"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Problēmu novēršana saistībā ar Android ierīču reģistrēšanu pakalpojumā Microsoft Intune

Pārskatiet tālāk norādītos resursus, lai atrisinātu savu problēmu tūlīt.
  
Dažas bieži sastopamās problēmas un risināšanas darbības:
  
 **Ierīce nav šifrēta kļūda uzņēmuma portālā:** Jaunākas Android versijas, it īpaši sākot ar v 7.0, ir nepieciešams startēšanas ieejas kods, lai nodrošinātu, ka jūsu ierīce ir pilnībā šifrēta. Biežākie risinājumi ir iespējot startēšanas PIN vai pilnībā šifrēt ierīci. Lai iegūtu papildinformāciju, pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .
  
 **Ierīces neveic atdevi, izmantojot Intune pakalpojumu vai to, ka Intune administrēšanas konsolē tiek rādīta kā "neveselīgs":** Dažas Samsung 4,4 un 5,5 ierīces nevar atdot pakalpojumu. Šajā jautājumā ir pieejami 3 iespējamie risinājumi.
  
1. Manuāli atveriet Intune uzņēmuma portāla programmu, kas automātiski uzsāks ierīces sinhronizāciju.

2. Atjauniniet ierīci uz Android 6,0 vai jaunākā versijā.

3. Atspējojiet Samsung Smart Manager, lai pārvaldītu Intune uzņēmuma portālu. Pārskatiet [šo dokumentu](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , lai iegūtu detalizētu informāciju par šīm problēmām un risinājumiem.

 **Lietotāja licences tips ir nederīgs** vai **lietotājvārds nav atpazīts:** lietotājam ir jāpiešķir Intune vai EMS licence. Pārskatiet šos dokumentus, lai piešķirtu licenci, izmantojot Office administrēšanas centru vai Azure portālu.
  
Papildu resursi, kas palīdz novērst problēmu:
  
1. Izmantojiet [Intune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu Biežākās reģistrācijas kļūmes. Lai iegūtu papildinformāciju, pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .

2. Pārskatiet [šo dokumentu](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) , lai skatītu sarakstu ar bieži sastopamām kļūdām, kas neļauj veikt reģistrāciju un risinājumus.

3. [Uzziniet, kā reģistrēt Android ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
