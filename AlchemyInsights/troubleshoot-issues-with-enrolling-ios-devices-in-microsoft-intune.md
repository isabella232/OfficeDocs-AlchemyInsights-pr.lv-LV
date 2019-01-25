---
title: Novērst problēmas, kas saistītas ar mācās iOS ierīces Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 663ff9b101494be781095ca550a4ed3deedca175
ms.sourcegitcommit: e2864efcfb493b6e46b662b746661a61232bdba7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/24/2019
ms.locfileid: "29479743"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="dd43e-102">Novērst problēmas, kas saistītas ar mācās iOS ierīces Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="dd43e-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="dd43e-103">Pārskata resursu, kas uzskaitīti turpmāk, lai atrisinātu jūsu problēmu tagad.</span><span class="sxs-lookup"><span data-stu-id="dd43e-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="dd43e-104">Daži izplatītākie kļūdu ziņojumi un rezolūcijas darbības:</span><span class="sxs-lookup"><span data-stu-id="dd43e-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="dd43e-p101">**Sasniedza ierīces vāciņš** Lietotājam ir vairākas ierīces, kas uzņemti nekā ierīces ierobežojums. Pārskatīt šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/en-us/intune/devices-wipe) vai [mainīt ierīces ierobežojums](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="dd43e-p101">**Device Cap Reached** The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="dd43e-p102">**Šo pakalpojumu, netiek atbalstīta. Nav reģistrācijas politika:** Apple Push paziņojums pakalpojumu (APN) nepieciešams konfigurēt vai atjaunot. Recenzējiet [šo dokumentu](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) norādījumus par to, kā to izdarīt.</span><span class="sxs-lookup"><span data-stu-id="dd43e-p102">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed. Review [this document](https://docs.microsoft.com/en-us/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="dd43e-p103">**Lietotāja licences tipam nederīga vai neatpazīts lietotājvārds:** Lietotāju vajadzībām, piešķir Intune vai EMS licenci. Pārskatīt šos dokumentus, lai piešķirtu licenci caur: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) vai [debeszils portāls](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="dd43e-p103">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license. Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/en-us/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/en-us/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="dd43e-111">Papildu resursi, kas var palīdzēt atrisināt jūsu problēmu:</span><span class="sxs-lookup"><span data-stu-id="dd43e-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="dd43e-p104">[Intune novēršana portāls](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) jālieto diagnosticē un risina ar kopēju reģistrācijas nepilnības. Recenzējiet [šo dokumentu](https://docs.microsoft.com/en-us/intune/help-desk-operators) sīkāku informāciju.</span><span class="sxs-lookup"><span data-stu-id="dd43e-p104">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="dd43e-114">Pārskatīt šos dokumentus bieži sastopamās kļūdas, kas novērstu iesaistīšanos un rezolūcijām uz katru sarakstu: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) un [traucējummeklēšana doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="dd43e-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="dd43e-115">[Uzziniet, kā pieteikties Microsoft Intune iOS ierīcēm](https://docs.microsoft.com/en-us/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="dd43e-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/ios-enroll).</span></span>
    

