---
title: Problēmu novēršana saistībā ar Windows ierīču reģistrāciju programmā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808978"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a>Problēmu novēršana saistībā ar Windows ierīču reģistrāciju programmā Microsoft Intune

Pārskatiet tālāk norādītos resursus, lai tūlīt novērstu savu problēmu.
  
Daži bieži sastopami kļūdu ziņojumi un risinājuma darbības:
  
 **Programmatūru nevar instalēt, un 0x80cf4017:** Jūsu konta sertifikāta derīgums ir beidzies. Atkārtoti lejupielādējiet PC Client programmatūras pakotni Intune administratora konsolē. Lai iegūtu papildinformāciju, pārskatiet šo dokumentāciju.
  
 **Kļūdas kods 0x801c0003:** Kļūda var rasties šādos scenārijos:
  
-  Lietotājam ir reģistrēts vairāk ierīču, nekā ierīces ierobežojums. Pārskatiet šos [dokumentus, lai noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) [vai mainītu ierīču ierobežojumu.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)

-  "Lietotāji var savienot ierīces ar Azure AD" ir iestatīts uz "none". Iestatiet to visiem vai atlasiet lietotājus. Lai [iegūtu papildinformāciju,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pārskatiet šo dokumentāciju.

-  Ierīci jau ir reģistrējis cits lietotājs. Šādā gadījumā noņemiet ierīci no Azure Intune konsoles vai manuāli atņemiet ierīces sarakstu, pirms mēģināt vēlreiz.

-  Ierīce ir Windows 10 Home. Pakalpojumam Azure Active Directory var pievienoties tikai Windows 10 Pro, Education un Enterprise SKU.

Papildu resursi, lai palīdzētu novērst problēmu:
  
-  Izmantojiet [Intune problēmu novēršanas portālu,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lai diagnosticētu un novērstu bieži sastopamās reģistrācijas kļūmes. Pārskatiet [šo dokumentu,](https://docs.microsoft.com/intune/help-desk-operators) lai iegūtu papildinformāciju.

-  Pārskatiet šos dokumentus, lai iegūtu sarakstu ar bieži sastopamajām kļūdām, kas novērš reģistrāciju un atrisināšanu katrā sarakstā: Problēmu novēršanas [rokasgrāmata](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) un [Problēmu novēršana dokumentā](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).

[Uzziniet, kā reģistrēt Windows ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).
