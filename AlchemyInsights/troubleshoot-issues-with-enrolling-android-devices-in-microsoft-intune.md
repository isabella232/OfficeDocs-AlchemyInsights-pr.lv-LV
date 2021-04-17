---
title: Problēmu novēršana saistībā ar Android ierīču reģistrāciju programmā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830949"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Problēmu novēršana saistībā ar Android ierīču reģistrāciju programmā Microsoft Intune

Pārskatiet tālāk norādītos resursus, lai tūlīt novērstu savu problēmu.
  
Dažas bieži sastopamās problēmas un risinājuma darbības:
  
 **Ierīce nav šifrēta kļūda uzņēmuma portālā:** Jaunākām Android versijām, īpaši sākot ar v7.0, nepieciešams startēšanas ieejas kods, lai nodrošinātu, ka jūsu ierīce ir pilnībā šifrēta. Bieži izmantotie risinājumi ir startēšanas PIN iespējošana vai ierīces pilnīga šifrēšana. Pārskatiet [šo dokumentu,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) lai iegūtu papildinformāciju.
  
 Ierīces nevar atdoties Intune pakalpojumā vai attēlot kā "Nav sveiks" **Intune administrēšanas konsolē:** Dažas Samsung 4.4 un 5.5 ierīces var nepārbauda pakalpojumu. Pastāv 3 iespējamie šīs problēmas risinājumi:
  
1. Manuāli atveriet lietojumprogrammu Intune Company Portal, kas automātiski iniciē ierīces sinhronizēšanu.

2. Atjauniniet ierīci uz Android 6.0 vai jaunāku versiju.

3. Atspējojiet Samsung Smart Manager no Intune uzņēmuma portāla pārvaldības. Pārskatiet [šo dokumentu,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) lai iegūtu papildinformāciju par šīm problēmām un risinājumu.

 **Lietotāja licences tips ir nederīgs** vai **lietotājvārds netiek atpazīts kļūda:** lietotājam ir jābūt piešķirtai Intune vai EMS licencei. Pārskatiet šos dokumentus, lai piešķirtu licenci, izmantojot Office administrēšanas centru vai Azure portālu.
  
Papildu resursi, lai palīdzētu novērst problēmu:
  
1. Izmantojiet [Intune problēmu novēršanas portālu,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lai diagnosticētu un novērstu bieži sastopamās reģistrācijas kļūmes. Pārskatiet [šo dokumentu,](https://docs.microsoft.com/intune/help-desk-operators) lai iegūtu papildinformāciju.

2. Pārskatiet [šo](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) dokumentu, lai redzētu bieži izplatītas kļūdas, kas neļauj reģistrēt un novērst problēmas katrā dokumentā.

3. [Uzziniet, kā reģistrēt Android ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
