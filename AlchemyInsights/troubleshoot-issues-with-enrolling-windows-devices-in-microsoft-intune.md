---
title: Problēmu novēršana saistībā ar Windows ierīču uzskaitīmēšanas Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665839"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Problēmu novēršana saistībā ar Windows ierīču uzskaitīmēšanas Microsoft InTune

Pārskatiet tālāk uzskaitītos resursus, lai atrisinātu problēmu tūlīt.
  
Daži bieži sastopami kļūdu ziņojumi un atrisināšanas darbības:
  
 **Programmatūru nevar instalēt, 0x80cf4017:** Jūsu konta sertifikātam ir beidzies derīgums. Atkārtoti lejupielādējiet datora klienta programmatūras pakotni InTune administrēšanas konsole. Pārskatiet šo dokumentāciju, lai iegūtu papildinformāciju.
  
 **Kļūdas kods 0x801c0003:** Kļūda var rasties šādos gadījumos:
  
-  Lietotājs ir uzņemti vairāk ierīču nekā ierīces ierobežojumu. Pārskatiet šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) vai [mainītu ierīces ierobežojumu](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Lietotāji var pievienoties ierīces Azure AD" ir iestatīts uz "none". Iestatiet to visiem vai atlasiet lietotāji. Pārskatiet [šo dokumentāciju](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , lai iegūtu papildinformāciju.

-  Ierīci jau ir reģistrējušies cits lietotājs. Šādā gadījumā noņemiet ierīci no Azure InTune konsoles vai manuāli atreģistrējiet ierīci, pirms mēģināt vēlreiz.

-  Ierīce ir Windows 10 Home. Azure Active Directory var pievienoties tikai Windows 10 Pro, Education un Enterprise SKUs.

Papildu resursus, lai palīdzētu atrisināt jūsu problēmu:
  
-  Izmantojiet [InTune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu vispārējas reģistrācijas kļūmes. Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , lai iegūtu detalizētu informāciju.

-  Pārskatiet šos dokumentus, lai iegūtu sarakstu ar bieži sastopamas kļūdas, kas neļauj iesaistīšanās un risinājumi: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) un [problēmu novēršana doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Uzziniet, kā reģistrēt Windows ierīces Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).
