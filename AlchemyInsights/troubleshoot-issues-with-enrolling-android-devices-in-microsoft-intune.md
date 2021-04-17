---
title: Problēmu novēršana saistībā ar Android ierīču reģistrāciju programmā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
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
ms.openlocfilehash: 08620a44dcf693482c65ff05e19f11870f67afbe
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51830949"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="e9941-102">Problēmu novēršana saistībā ar Android ierīču reģistrāciju programmā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e9941-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="e9941-103">Pārskatiet tālāk norādītos resursus, lai tūlīt novērstu savu problēmu.</span><span class="sxs-lookup"><span data-stu-id="e9941-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="e9941-104">Dažas bieži sastopamās problēmas un risinājuma darbības:</span><span class="sxs-lookup"><span data-stu-id="e9941-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="e9941-105">**Ierīce nav šifrēta kļūda uzņēmuma portālā:** Jaunākām Android versijām, īpaši sākot ar v7.0, nepieciešams startēšanas ieejas kods, lai nodrošinātu, ka jūsu ierīce ir pilnībā šifrēta.</span><span class="sxs-lookup"><span data-stu-id="e9941-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="e9941-106">Bieži izmantotie risinājumi ir startēšanas PIN iespējošana vai ierīces pilnīga šifrēšana.</span><span class="sxs-lookup"><span data-stu-id="e9941-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="e9941-107">Pārskatiet [šo dokumentu,](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="e9941-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="e9941-108">Ierīces nevar atdoties Intune pakalpojumā vai attēlot kā "Nav sveiks" **Intune administrēšanas konsolē:** Dažas Samsung 4.4 un 5.5 ierīces var nepārbauda pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="e9941-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="e9941-109">Pastāv 3 iespējamie šīs problēmas risinājumi:</span><span class="sxs-lookup"><span data-stu-id="e9941-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="e9941-110">Manuāli atveriet lietojumprogrammu Intune Company Portal, kas automātiski iniciē ierīces sinhronizēšanu.</span><span class="sxs-lookup"><span data-stu-id="e9941-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="e9941-111">Atjauniniet ierīci uz Android 6.0 vai jaunāku versiju.</span><span class="sxs-lookup"><span data-stu-id="e9941-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="e9941-112">Atspējojiet Samsung Smart Manager no Intune uzņēmuma portāla pārvaldības.</span><span class="sxs-lookup"><span data-stu-id="e9941-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="e9941-113">Pārskatiet [šo dokumentu,](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) lai iegūtu papildinformāciju par šīm problēmām un risinājumu.</span><span class="sxs-lookup"><span data-stu-id="e9941-113">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="e9941-114">**Lietotāja licences tips ir nederīgs** vai **lietotājvārds netiek atpazīts kļūda:** lietotājam ir jābūt piešķirtai Intune vai EMS licencei.</span><span class="sxs-lookup"><span data-stu-id="e9941-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="e9941-115">Pārskatiet šos dokumentus, lai piešķirtu licenci, izmantojot Office administrēšanas centru vai Azure portālu.</span><span class="sxs-lookup"><span data-stu-id="e9941-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="e9941-116">Papildu resursi, lai palīdzētu novērst problēmu:</span><span class="sxs-lookup"><span data-stu-id="e9941-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="e9941-117">Izmantojiet [Intune problēmu novēršanas portālu,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lai diagnosticētu un novērstu bieži sastopamās reģistrācijas kļūmes.</span><span class="sxs-lookup"><span data-stu-id="e9941-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e9941-118">Pārskatiet [šo dokumentu,](https://docs.microsoft.com/intune/help-desk-operators) lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="e9941-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="e9941-119">Pārskatiet [šo](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) dokumentu, lai redzētu bieži izplatītas kļūdas, kas neļauj reģistrēt un novērst problēmas katrā dokumentā.</span><span class="sxs-lookup"><span data-stu-id="e9941-119">Review [this document](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="e9941-120">[Uzziniet, kā reģistrēt Android ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="e9941-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
