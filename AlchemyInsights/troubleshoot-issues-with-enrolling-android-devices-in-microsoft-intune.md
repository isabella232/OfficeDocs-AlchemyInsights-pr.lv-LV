---
title: Novērst problēmas, kas saistītas ar mācās Android ierīces Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.openlocfilehash: 6b26b2d77bceb063090986ff4e20bc4a56bb1242
ms.sourcegitcommit: 0ae6cbb8cf2836da98300767ed81b411d6551bee
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/30/2019
ms.locfileid: "29655890"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a>Novērst problēmas, kas saistītas ar mācās Android ierīces Microsoft Intune

Pārskata resursu, kas uzskaitīti turpmāk, lai atrisinātu jūsu problēmu tagad.
  
Dažas biežāk sastopamās problēmas un risināšanas soļi:
  
 **Ierīce nav šifrēts kļūdas uzņēmuma portālā:** Jaunākas versijas Android, sevišķi sākot ar v 7.0, nepieciešams starta patentatslēga, lai pārliecinātos, vai jūsu ierīce ir pilnībā šifrēts. Iespējot startēšanas pin vai pilnībā šifrēt ierīce ir kopīgi risinājumi. Recenzējiet [šo dokumentu](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) plašāku informāciju. 
  
 **Ierīces neizdodas pārbaudi ar Intune pakalpojumu vai parādītu kā "Unhealthy" Intune admin konsole:** Daži Samsung 4,4 un 5,5 ierīces var pārbaudīt ekspluatācijā. Pastāv 3 iespējamie risinājumi šo problēmu: 
  
1. Manuāli atveriet Intune uzņēmuma portāla app, kas automātiski uzsāks ierīču sinhronizēšanu.
    
2. Atjauninātu ierīces Android 6.0 vai augstāku.
    
3. Samsung Smart pārvaldnieks atspējošana no pārvaldot uzņēmuma portāls Intune. Recenzējiet [šo dokumentu](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) sīkāku informāciju par šiem jautājumiem un rezolūcijas. 
    
 **Lietotāja licences tipam nederīga** vai **lietotāja nosaukums nav atpazīts kļūda:** lietotāju vajadzībām, piešķir Intune vai EMS licenci. Pārskatīt šos dokumentus, lai piešķirtu licenci caur: Office Admin Center vai Azure portāls. 
  
Papildu resursi, kas var palīdzēt atrisināt jūsu problēmu:
  
1. [Intune novēršana portāls](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) jālieto diagnosticē un risina ar kopēju reģistrācijas nepilnības. Recenzējiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) sīkāku informāciju. 
    
2. Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) sarakstu bieži sastopamās kļūdas, kas novērstu iesaistīšanos un rezolūcijas katram. 
    
3. [Uzziniet, kā uzņemt Android ierīces Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).
    

