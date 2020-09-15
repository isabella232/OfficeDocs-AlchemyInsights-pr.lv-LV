---
title: Problēmu novēršana saistībā ar Windows ierīču reģistrēšanu pakalpojumā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658885"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Problēmu novēršana saistībā ar Windows ierīču reģistrēšanu pakalpojumā Microsoft Intune

Pārskatiet tālāk norādītos resursus, lai atrisinātu savu problēmu tūlīt.
  
Daži bieži sastopami kļūdu ziņojumi un atrisināšanas darbības:
  
 **Šo programmatūru nevar instalēt, 0x80cf4017:** Jūsu konta sertifikāta derīguma termiņš ir beidzies. Atkārtoti lejupielādējiet PC klienta programmatūras pakotni Intune administratora konsolē. Lai iegūtu papildinformāciju, pārskatiet šo dokumentāciju.
  
 **Kļūdas kods 0x801c0003:** Kļūda var rasties tālāk norādītajos gadījumos.
  
-  Lietotājam ir vairāk ierīču, kas reģistrējušies nekā ierīces ierobežojums. Pārskatiet šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) vai [mainītu ierīces ierobežojumu](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).

-  "Lietotāji var pievienoties ierīcēm uz Azure AD" ir iestatīts uz "nav". Iestatiet to visiem vai atlasiet lietotāji. Lai iegūtu papildinformāciju, pārskatiet [šo dokumentāciju](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .

-  Ierīci jau ir reģistrējis cits lietotājs. Ja tā ir, izņemiet ierīci no Azure Intune konsoles vai manuāli noņemiet ierīci, pirms mēģināt vēlreiz.

-  Ierīce ir Windows 10 Home. Azure Active Directory var pievienot tikai Windows 10 Pro, Education un Enterprise SKU.

Papildu resursi, kas palīdz novērst problēmu:
  
-  Izmantojiet [Intune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu Biežākās reģistrācijas kļūmes. Lai iegūtu papildinformāciju, pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .

-  Pārskatiet šos dokumentus, lai skatītu sarakstu ar bieži sastopamām kļūdām, kas neļauj veikt reģistrāciju un risinājumus: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) un [problēmu novēršana](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).

[Uzziniet, kā sistēmā Microsoft Intune reģistrēt Windows ierīces](https://docs.microsoft.com/intune/windows-enroll).
