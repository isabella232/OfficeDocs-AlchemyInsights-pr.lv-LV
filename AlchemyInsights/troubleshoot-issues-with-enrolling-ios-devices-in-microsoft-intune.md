---
title: Novērst problēmas, kas saistītas ar mācās iOS ierīces Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: d28dca4fccf823e627dd179f828ba3b8baf843a6
ms.sourcegitcommit: 9d78905c512192ffc4675468abd2efc5f2e4baf4
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/23/2019
ms.locfileid: "32391014"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="520cd-102">Novērst problēmas, kas saistītas ar mācās iOS ierīces Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="520cd-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="520cd-103">Pārskata resursu, kas uzskaitīti turpmāk, lai atrisinātu jūsu problēmu tagad.</span><span class="sxs-lookup"><span data-stu-id="520cd-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="520cd-104">Daži izplatītākie kļūdu ziņojumi un rezolūcijas darbības:</span><span class="sxs-lookup"><span data-stu-id="520cd-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="520cd-105">**Sasniedza ierīces vāciņš** Lietotājam ir vairākas ierīces, kas uzņemti nekā ierīces ierobežojums.</span><span class="sxs-lookup"><span data-stu-id="520cd-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="520cd-106">Pārskatīt šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) vai [mainīt ierīces ierobežojums](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="520cd-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="520cd-107">**Šo pakalpojumu, netiek atbalstīta. Nav reģistrācijas politika:** Apple Push paziņojums pakalpojumu (APN) nepieciešams konfigurēt vai atjaunot.</span><span class="sxs-lookup"><span data-stu-id="520cd-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="520cd-108">Recenzējiet [šo dokumentu](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) norādījumus par to, kā to izdarīt.</span><span class="sxs-lookup"><span data-stu-id="520cd-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="520cd-109">**Lietotāja licences tipam nederīga vai neatpazīts lietotājvārds:** Lietotāju vajadzībām, piešķir Intune vai EMS licenci.</span><span class="sxs-lookup"><span data-stu-id="520cd-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="520cd-110">Pārskatīt šos dokumentus, lai piešķirtu licenci caur: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) vai [debeszils portāls](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="520cd-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="520cd-111">Papildu resursi, kas var palīdzēt atrisināt jūsu problēmu:</span><span class="sxs-lookup"><span data-stu-id="520cd-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="520cd-112">[Intune novēršana portāls](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) jālieto diagnosticē un risina ar kopēju reģistrācijas nepilnības.</span><span class="sxs-lookup"><span data-stu-id="520cd-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="520cd-113">Recenzējiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) sīkāku informāciju.</span><span class="sxs-lookup"><span data-stu-id="520cd-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="520cd-114">Pārskatīt šos dokumentus bieži sastopamās kļūdas, kas novērstu iesaistīšanos un rezolūcijām uz katru sarakstu: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) un [traucējummeklēšana doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="520cd-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="520cd-115">[Uzziniet, kā pieteikties Microsoft Intune iOS ierīcēm](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="520cd-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

