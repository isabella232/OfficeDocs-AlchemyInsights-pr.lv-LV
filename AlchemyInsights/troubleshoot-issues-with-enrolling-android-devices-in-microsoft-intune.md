---
title: Novērst problēmas, kas saistītas ar Android ierīču uzskaitīmēšanas Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759627"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Novērst problēmas, kas saistītas ar Android ierīču uzskaitīmēšanas Microsoft InTune

Pārskatiet tālāk uzskaitītos resursus, lai atrisinātu problēmu tūlīt.
  
Dažas bieži sastopamās problēmas un atrisināšanas darbības:
  
 **Ierīce nav šifrēta kļūda uzņēmuma portālā:** Jaunākas Android versijas, īpaši sākot ar v 7.0, pieprasa startēšanas patentatslēgu, lai pārliecinātos, vai ierīce ir pilnībā šifrēta. Kopīgie risinājumi ir iespējot startēšanas PIN vai pilnībā šifrēt ierīci. Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , lai iegūtu papildinformāciju.
  
 **Ierīces nevar reģistrēties ar pakalpojumu InTune vai parādīt kā "neveselīgs" InTune administrēšanas konsole:** Daži Samsung 4,4 un 5,5 ierīces nevar pārbaudīt pakalpojumu. Ir 3 iespējamie risinājumi, lai šo jautājumu:
  
1. Manuāli atveriet lietojumprogrammu InTune uzņēmuma portāls, kas automātiski iniciēs ierīces sinhronizāciju.

2. Atjauniniet ierīci uz Android 6,0 vai jaunāku.

3. Atspējojiet Samsung Smart Manager pārvaldīt InTune uzņēmuma portāls. Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , lai iegūtu plašāku informāciju par šiem jautājumiem un rezolūcijām.

 **Lietotāja licences tips nav derīgs** vai **lietotāja vārds nav atpazīts kļūda:** lietotājam ir jāpiešķir InTune vai EMS licence. Pārskatiet šos dokumentus, lai piešķirtu licenci, izmantojot: Office administrēšanas centrs vai Azure portāls.
  
Papildu resursus, lai palīdzētu atrisināt jūsu problēmu:
  
1. Izmantojiet [InTune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu vispārējas reģistrācijas kļūmes. Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , lai iegūtu detalizētu informāciju.

2. Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , lai iegūtu sarakstu ar izplatītākās kļūdas, kas nepieļauj iesaistīšanos un rezolūcijas.

3. [Uzziniet, kā reģistrēt Android ierīces Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).
