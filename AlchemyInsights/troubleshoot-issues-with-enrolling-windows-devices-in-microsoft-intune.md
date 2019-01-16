---
title: Novērst problēmas, kas saistītas ar Microsoft Intune Windows ierīču mācās
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28300788"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Novērst problēmas, kas saistītas ar Microsoft Intune Windows ierīču mācās

Pārskata resursu, kas uzskaitīti turpmāk, lai atrisinātu jūsu problēmu tagad. 
  
Daži izplatītākie kļūdu ziņojumi un rezolūcijas darbības:
  
 **Programmatūru nevar instalēt, 0x80cf4017:** Jūsu kontā sertifikātu derīguma termiņš ir beidzies. Atkārtoti ielādēt PC klienta programmatūras pakotnes Intune Admin konsole. Pārskatīt šo dokumentāciju, lai iegūtu vairāk informācijas. 
  
 **0x801c0003. kļūdas kods:** Kļūda var rasties šādos gadījumos: 
  
1. Lietotājam ir vairākas ierīces, kas uzņemti nekā ierīces ierobežojums. Pārskatīt šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/en-us/intune/devices-wipe) vai [mainīt ierīces ierobežojums](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).
    
2. "Lietotāji var pievienot ierīces debeszils reklāmu" ir iestatīts uz "neviens". Iestatīt tā, lai visu vai atlasiet lietotāju. Pārskatīt [šo dokumentāciju](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) . 
    
3. Cits lietotājs ir reģistrējies ierīci. Ja tas tā ir gadījumā, izņemiet ierīci no Azure Intune konsole vai manuāli unenroll ierīci, pirms mēģināt vēlreiz.
    
4. Ierīcē ir Windows 10 mājās. Tikai Windows 10 Pro, izglītība un Enterprise SKU var pievienoties Azure Active Directory.
    
Papildu resursi, kas var palīdzēt atrisināt jūsu problēmu:
  
1. [Intune novēršana portāls](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) jālieto diagnosticē un risina ar kopēju reģistrācijas nepilnības. Recenzējiet [šo dokumentu](https://docs.microsoft.com/en-us/intune/help-desk-operators) sīkāku informāciju. 
    
2. Pārskatīt šos dokumentus bieži sastopamās kļūdas, kas novērstu iesaistīšanos un rezolūcijām uz katru sarakstu: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) un [traucējummeklēšana doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).
    
[Uzziniet, kā pieteikties Microsoft Intune Windows ierīču](https://docs.microsoft.com/en-us/intune/windows-enroll).
  

