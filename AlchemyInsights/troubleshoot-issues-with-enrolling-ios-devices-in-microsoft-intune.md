---
title: Problēmu novēršana saistībā ar iOS ierīču uzskaitīmēšanas Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d717bcc9-1cc1-44f6-b5e6-c1bc059c1973
ms.openlocfilehash: 664c18daca5d8e0ad4a88f41db3ff0dbced606e5
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43736165"
---
# <a name="troubleshoot-issues-with-enrolling-ios-devices-in-microsoft-intune"></a><span data-ttu-id="c5e41-102">Problēmu novēršana saistībā ar iOS ierīču uzskaitīmēšanas Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="c5e41-102">Troubleshoot issues with enrolling iOS devices in Microsoft Intune</span></span>

<span data-ttu-id="c5e41-103">Pārskatiet tālāk uzskaitītos resursus, lai atrisinātu problēmu tūlīt.</span><span class="sxs-lookup"><span data-stu-id="c5e41-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="c5e41-104">Daži bieži sastopami kļūdu ziņojumi un atrisināšanas darbības:</span><span class="sxs-lookup"><span data-stu-id="c5e41-104">Some common error messages and resolution steps:</span></span>
  
- <span data-ttu-id="c5e41-105">**Sasniegts ierīces vāciņš** Lietotājs ir uzņemti vairāk ierīču nekā ierīces ierobežojumu.</span><span class="sxs-lookup"><span data-stu-id="c5e41-105">**Device Cap Reached** The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="c5e41-106">Pārskatiet šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) vai [mainītu ierīces ierobežojumu](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="c5e41-106">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
- <span data-ttu-id="c5e41-107">**Šis pakalpojums netiek atbalstīts. Nav reģistrācijas politikas:** ir jākonfigurē vai jāatjauno Apple stumšanas paziņojumu pakalpojums (APN).</span><span class="sxs-lookup"><span data-stu-id="c5e41-107">**This Service is not supported. No Enrollment Policy:** Apple Push Notification Service (APNS) needs to be configured or renewed.</span></span> <span data-ttu-id="c5e41-108">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) , lai uzzinātu, kā to izdarīt.</span><span class="sxs-lookup"><span data-stu-id="c5e41-108">Review [this document](https://docs.microsoft.com/intune/apple-mdm-push-certificate-get) for instructions on how to do that.</span></span> 
    
- <span data-ttu-id="c5e41-109">**Lietotāja licences tips nav derīgs vai lietotāja vārds nav atpazīts:** Lietotājam ir jāpiešķir InTune vai EMS licence.</span><span class="sxs-lookup"><span data-stu-id="c5e41-109">**User License Type Invalid or User Name Not Recognized:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="c5e41-110">Pārskatiet šos dokumentus, lai piešķirtu licenci, izmantojot: [Office administrēšanas centrs](https://docs.microsoft.com/intune/licenses-assign) vai [Azure portāls](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span><span class="sxs-lookup"><span data-stu-id="c5e41-110">Review these documents to assign a license through: [Office Admin Center](https://docs.microsoft.com/intune/licenses-assign) or [Azure portal](https://docs.microsoft.com/azure/active-directory/license-users-groups).</span></span>
    
<span data-ttu-id="c5e41-111">Papildu resursus, lai palīdzētu atrisināt jūsu problēmu:</span><span class="sxs-lookup"><span data-stu-id="c5e41-111">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="c5e41-112">Izmantojiet [InTune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu vispārējas reģistrācijas kļūmes.</span><span class="sxs-lookup"><span data-stu-id="c5e41-112">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="c5e41-113">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , lai iegūtu detalizētu informāciju.</span><span class="sxs-lookup"><span data-stu-id="c5e41-113">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="c5e41-114">Pārskatiet šos dokumentus, lai iegūtu sarakstu ar bieži sastopamas kļūdas, kas neļauj iesaistīšanās un risinājumi: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) un [problēmu novēršana doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="c5e41-114">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4039809/troubleshooting-ios-device-enrollment-in-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
3. <span data-ttu-id="c5e41-115">[Uzziniet, kā reģistrēt iOS ierīces Microsoft InTune](https://docs.microsoft.com/intune/ios-enroll).</span><span class="sxs-lookup"><span data-stu-id="c5e41-115">[Learn how to enroll iOS devices in Microsoft Intune](https://docs.microsoft.com/intune/ios-enroll).</span></span>
    

