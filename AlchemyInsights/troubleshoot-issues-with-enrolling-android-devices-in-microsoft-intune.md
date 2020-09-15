---
title: Problēmu novēršana saistībā ar Android ierīču reģistrēšanu pakalpojumā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: b5cb2e8a76e8e7d91bd9cd8789ae1623a7f96579
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47689961"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="829ca-102">Problēmu novēršana saistībā ar Android ierīču reģistrēšanu pakalpojumā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="829ca-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="829ca-103">Pārskatiet tālāk norādītos resursus, lai atrisinātu savu problēmu tūlīt.</span><span class="sxs-lookup"><span data-stu-id="829ca-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="829ca-104">Dažas bieži sastopamās problēmas un risināšanas darbības:</span><span class="sxs-lookup"><span data-stu-id="829ca-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="829ca-105">**Ierīce nav šifrēta kļūda uzņēmuma portālā:** Jaunākas Android versijas, it īpaši sākot ar v 7.0, ir nepieciešams startēšanas ieejas kods, lai nodrošinātu, ka jūsu ierīce ir pilnībā šifrēta.</span><span class="sxs-lookup"><span data-stu-id="829ca-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="829ca-106">Biežākie risinājumi ir iespējot startēšanas PIN vai pilnībā šifrēt ierīci.</span><span class="sxs-lookup"><span data-stu-id="829ca-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="829ca-107">Lai iegūtu papildinformāciju, pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) .</span><span class="sxs-lookup"><span data-stu-id="829ca-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="829ca-108">**Ierīces neveic atdevi, izmantojot Intune pakalpojumu vai to, ka Intune administrēšanas konsolē tiek rādīta kā "neveselīgs":** Dažas Samsung 4,4 un 5,5 ierīces nevar atdot pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="829ca-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="829ca-109">Šajā jautājumā ir pieejami 3 iespējamie risinājumi.</span><span class="sxs-lookup"><span data-stu-id="829ca-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="829ca-110">Manuāli atveriet Intune uzņēmuma portāla programmu, kas automātiski uzsāks ierīces sinhronizāciju.</span><span class="sxs-lookup"><span data-stu-id="829ca-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="829ca-111">Atjauniniet ierīci uz Android 6,0 vai jaunākā versijā.</span><span class="sxs-lookup"><span data-stu-id="829ca-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="829ca-112">Atspējojiet Samsung Smart Manager, lai pārvaldītu Intune uzņēmuma portālu.</span><span class="sxs-lookup"><span data-stu-id="829ca-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="829ca-113">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , lai iegūtu detalizētu informāciju par šīm problēmām un risinājumiem.</span><span class="sxs-lookup"><span data-stu-id="829ca-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="829ca-114">**Lietotāja licences tips ir nederīgs** vai **lietotājvārds nav atpazīts:** lietotājam ir jāpiešķir Intune vai EMS licence.</span><span class="sxs-lookup"><span data-stu-id="829ca-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="829ca-115">Pārskatiet šos dokumentus, lai piešķirtu licenci, izmantojot Office administrēšanas centru vai Azure portālu.</span><span class="sxs-lookup"><span data-stu-id="829ca-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="829ca-116">Papildu resursi, kas palīdz novērst problēmu:</span><span class="sxs-lookup"><span data-stu-id="829ca-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="829ca-117">Izmantojiet [Intune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu Biežākās reģistrācijas kļūmes.</span><span class="sxs-lookup"><span data-stu-id="829ca-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="829ca-118">Lai iegūtu papildinformāciju, pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="829ca-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="829ca-119">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , lai skatītu sarakstu ar bieži sastopamām kļūdām, kas neļauj veikt reģistrāciju un risinājumus.</span><span class="sxs-lookup"><span data-stu-id="829ca-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="829ca-120">[Uzziniet, kā reģistrēt Android ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="829ca-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
