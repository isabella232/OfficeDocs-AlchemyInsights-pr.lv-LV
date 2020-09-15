---
title: Problēmu novēršana saistībā ar iOS ierīču reģistrēšanu pakalpojumā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 7d3e0049258a77016250c8a657c8fbcaf8d65212
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47669255"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="c7e97-102">Problēmu novēršana saistībā ar iOS ierīču reģistrēšanu pakalpojumā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="c7e97-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="c7e97-103">Pārskatiet tālāk norādītos resursus, lai atrisinātu savu problēmu tūlīt.</span><span class="sxs-lookup"><span data-stu-id="c7e97-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="c7e97-104">Daži bieži sastopami kļūdu ziņojumi un atrisināšanas darbības:</span><span class="sxs-lookup"><span data-stu-id="c7e97-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="c7e97-105">**Sasniegts ierīces vāciņš** Lietotājam ir vairāk ierīču, kas reģistrējušies nekā ierīces ierobežojums.</span><span class="sxs-lookup"><span data-stu-id="c7e97-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c7e97-106">Pārskatiet šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) vai [mainītu ierīces ierobežojumu](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="c7e97-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="c7e97-107">**Šis pakalpojums netiek atbalstīts. Nav reģistrācijas politikas:** Apple push Notification Service (APN) ir jākonfigurē vai jāatjauno.</span><span class="sxs-lookup"><span data-stu-id="c7e97-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="c7e97-108">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , lai saņemtu norādījumus par to, kā to izdarīt.</span><span class="sxs-lookup"><span data-stu-id="c7e97-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="c7e97-109">**Lietotāja licences tips ir nederīgs vai lietotājvārds nav atpazīts:** Lietotājam ir jāpiešķir Intune vai EMS licence.</span><span class="sxs-lookup"><span data-stu-id="c7e97-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="c7e97-110">Pārskatiet šos dokumentus, lai piešķirtu licenci, izmantojot [Office administrēšanas centru](https://docs.microsoft.com/intune/licenses-assign) vai [Azure portālu](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="c7e97-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="c7e97-111">Papildu resursi, kas palīdz novērst problēmu:</span><span class="sxs-lookup"><span data-stu-id="c7e97-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c7e97-112">Izmantojiet [Intune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu Biežākās reģistrācijas kļūmes.</span><span class="sxs-lookup"><span data-stu-id="c7e97-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c7e97-113">Lai iegūtu papildinformāciju, pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="c7e97-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="c7e97-114">Pārskatiet šos dokumentus, lai skatītu sarakstu ar bieži sastopamām kļūdām, kas neļauj veikt reģistrāciju un risinājumus: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) un [problēmu novēršana](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c7e97-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="c7e97-115">[Uzziniet, kā reģistrēt iOS ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="c7e97-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

