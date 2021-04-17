---
title: Problēmu novēršana saistībā ar iOS ierīču reģistrāciju programmā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 14f7a897f0c7504db1b605485e170183c3a1afb2
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51823470"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="f3860-102">Problēmu novēršana saistībā ar iOS ierīču reģistrāciju programmā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f3860-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="f3860-103">Pārskatiet tālāk norādītos resursus, lai tūlīt novērstu savu problēmu.</span><span class="sxs-lookup"><span data-stu-id="f3860-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="f3860-104">Daži bieži sastopami kļūdu ziņojumi un risinājuma darbības:</span><span class="sxs-lookup"><span data-stu-id="f3860-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="f3860-105">**Sasniegts ierīces sākumburts** Lietotājam ir reģistrēts vairāk ierīču, nekā ierīces ierobežojums.</span><span class="sxs-lookup"><span data-stu-id="f3860-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="f3860-106">Pārskatiet šos [dokumentus, lai noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) [vai mainītu ierīču ierobežojumu.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="f3860-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="f3860-107">**Šis pakalpojums netiek atbalstīts. Nav reģistrācijas politikas:** Apple pašpiegādes paziņojumu pakalpojums (APNS) ir jākonfigurē vai jāatjauno.</span><span class="sxs-lookup"><span data-stu-id="f3860-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="f3860-108">Pārskatiet [šo](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) dokumentu, lai saņemtu norādījumus par to, kā to paveikt.</span><span class="sxs-lookup"><span data-stu-id="f3860-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="f3860-109">**Lietotāja licences tips nav derīgs vai lietotājvārds netiek atpazīts:** Lietotājam ir jābūt piešķirtai Intune vai EMS licencei.</span><span class="sxs-lookup"><span data-stu-id="f3860-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="f3860-110">Pārskatiet šos dokumentus, lai piešķirtu licenci, [izmantojot Office administrēšanas centru](https://docs.microsoft.com/intune/licenses-assign) vai Azure [portālu.](https://docs.microsoft.com/azure/active-directory/license-users-groups)</span><span class="sxs-lookup"><span data-stu-id="f3860-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="f3860-111">Papildu resursi, lai palīdzētu novērst problēmu:</span><span class="sxs-lookup"><span data-stu-id="f3860-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f3860-112">Izmantojiet [Intune problēmu novēršanas portālu,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lai diagnosticētu un novērstu bieži sastopamās reģistrācijas kļūmes.</span><span class="sxs-lookup"><span data-stu-id="f3860-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f3860-113">Pārskatiet [šo dokumentu,](https://docs.microsoft.com/intune/help-desk-operators) lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="f3860-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="f3860-114">Pārskatiet šos dokumentus, lai noskaidrotu bieži sastopamās kļūdas, kas neļauj veikt reģistrāciju, un to novēršanas darbības: [problēmu novēršanas norādījumi](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) un [problēmu novēršanas dokuments](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="f3860-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="f3860-115">[Uzziniet, kā reģistrēt iOS ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="f3860-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

