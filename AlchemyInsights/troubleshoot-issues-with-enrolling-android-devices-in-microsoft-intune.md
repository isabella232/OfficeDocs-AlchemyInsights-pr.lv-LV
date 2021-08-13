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
ms.openlocfilehash: 0ae926e6b31493e7359981c621fd27e8f53d49a17bdf107173b087fe6cc688fa
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54008085"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Problēmu novēršana saistībā ar Android ierīču reģistrāciju programmā Microsoft Intune

Pārskatiet tālāk norādītos resursus, lai tūlīt novērstu savu problēmu.
  
Dažas bieži sastopamās problēmas un risinājuma darbības:
  
 **Ierīces šifrēšanas kļūda programmā Company Portal:** Jaunākām Android versijām, īpaši sākot ar v7.0, nepieciešams startēšanas ieejas kods, lai nodrošinātu, ka jūsu ierīce ir pilnībā šifrēta. Bieži izmantotie risinājumi ir startēšanas PIN iespējošana vai ierīces pilnīga šifrēšana. Pārskatiet [šo dokumentu,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) lai iegūtu papildinformāciju.
  
 Ierīces nevar atdoties Intune pakalpojumā vai attēlot kā "Nav sveiks" **Intune administrēšanas konsolē:** Dažas Samsung 4.4 un 5.5 ierīces var nepārbauda pakalpojumu. Pastāv 3 iespējamie šīs problēmas risinājumi:
  
1. Manuāli atveriet programmu Intune Company Portal, kas automātiski iniciē ierīces sinhronizēšanu.

2. Atjauniniet ierīci uz Android 6.0 vai jaunāku versiju.

3. Atspējojiet Samsung Smart Manager, lai tā pārvaldītu Intune Company Portal. Pārskatiet [šo dokumentu,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) lai iegūtu papildinformāciju par šīm problēmām un risinājumu.

 **Lietotāja licences tips ir nederīgs** vai **lietotājvārds netiek atpazīts kļūda:** lietotājam ir jābūt piešķirtai Intune vai EMS licencei. Pārskatiet šos dokumentus, lai piešķirtu licenci, Office administrēšanas centrā vai Azure portālā.
  
Papildu resursi, lai palīdzētu novērst problēmu:
  
1. Izmantojiet [Intune problēmu novēršanas portālu,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lai diagnosticētu un novērstu bieži sastopamās reģistrācijas kļūmes. Pārskatiet [šo dokumentu,](https://docs.microsoft.com/intune/help-desk-operators) lai iegūtu papildinformāciju.

2. Pārskatiet [šo](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) dokumentu, lai redzētu bieži izplatītas kļūdas, kas neļauj reģistrēt un novērst problēmas katrā dokumentā.

3. [Uzziniet, kā reģistrēt Android ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
