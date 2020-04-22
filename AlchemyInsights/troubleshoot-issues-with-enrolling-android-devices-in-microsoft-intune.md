---
title: Novērst problēmas, kas saistītas ar Android ierīču uzskaitīmēšanas Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: bd6d278ebf6cca7fb6e4ac1049deae600b516707
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43759627"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="9b789-102">Novērst problēmas, kas saistītas ar Android ierīču uzskaitīmēšanas Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="9b789-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="9b789-103">Pārskatiet tālāk uzskaitītos resursus, lai atrisinātu problēmu tūlīt.</span><span class="sxs-lookup"><span data-stu-id="9b789-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="9b789-104">Dažas bieži sastopamās problēmas un atrisināšanas darbības:</span><span class="sxs-lookup"><span data-stu-id="9b789-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="9b789-105">**Ierīce nav šifrēta kļūda uzņēmuma portālā:** Jaunākas Android versijas, īpaši sākot ar v 7.0, pieprasa startēšanas patentatslēgu, lai pārliecinātos, vai ierīce ir pilnībā šifrēta.</span><span class="sxs-lookup"><span data-stu-id="9b789-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="9b789-106">Kopīgie risinājumi ir iespējot startēšanas PIN vai pilnībā šifrēt ierīci.</span><span class="sxs-lookup"><span data-stu-id="9b789-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="9b789-107">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) , lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="9b789-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="9b789-108">**Ierīces nevar reģistrēties ar pakalpojumu InTune vai parādīt kā "neveselīgs" InTune administrēšanas konsole:** Daži Samsung 4,4 un 5,5 ierīces nevar pārbaudīt pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="9b789-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="9b789-109">Ir 3 iespējamie risinājumi, lai šo jautājumu:</span><span class="sxs-lookup"><span data-stu-id="9b789-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="9b789-110">Manuāli atveriet lietojumprogrammu InTune uzņēmuma portāls, kas automātiski iniciēs ierīces sinhronizāciju.</span><span class="sxs-lookup"><span data-stu-id="9b789-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="9b789-111">Atjauniniet ierīci uz Android 6,0 vai jaunāku.</span><span class="sxs-lookup"><span data-stu-id="9b789-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="9b789-112">Atspējojiet Samsung Smart Manager pārvaldīt InTune uzņēmuma portāls.</span><span class="sxs-lookup"><span data-stu-id="9b789-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="9b789-113">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) , lai iegūtu plašāku informāciju par šiem jautājumiem un rezolūcijām.</span><span class="sxs-lookup"><span data-stu-id="9b789-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="9b789-114">**Lietotāja licences tips nav derīgs** vai **lietotāja vārds nav atpazīts kļūda:** lietotājam ir jāpiešķir InTune vai EMS licence.</span><span class="sxs-lookup"><span data-stu-id="9b789-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="9b789-115">Pārskatiet šos dokumentus, lai piešķirtu licenci, izmantojot: Office administrēšanas centrs vai Azure portāls.</span><span class="sxs-lookup"><span data-stu-id="9b789-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="9b789-116">Papildu resursus, lai palīdzētu atrisināt jūsu problēmu:</span><span class="sxs-lookup"><span data-stu-id="9b789-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="9b789-117">Izmantojiet [InTune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu vispārējas reģistrācijas kļūmes.</span><span class="sxs-lookup"><span data-stu-id="9b789-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="9b789-118">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , lai iegūtu detalizētu informāciju.</span><span class="sxs-lookup"><span data-stu-id="9b789-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="9b789-119">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) , lai iegūtu sarakstu ar izplatītākās kļūdas, kas nepieļauj iesaistīšanos un rezolūcijas.</span><span class="sxs-lookup"><span data-stu-id="9b789-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="9b789-120">[Uzziniet, kā reģistrēt Android ierīces Microsoft InTune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="9b789-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
