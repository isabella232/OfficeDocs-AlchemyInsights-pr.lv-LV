---
title: Novērst problēmas, kas saistītas ar mācās Android ierīces Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d0269461-20a8-4c9e-83b2-8fcf608dc0a5
ms.custom:
- "787"
- "6200002"
ms.openlocfilehash: 9cdfda0d7dd45af260f46738cbc85aac46f53960
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35367296"
---
# <a name="troubleshoot-issues-with-enrolling-android-devices-in-microsoft-intune"></a><span data-ttu-id="f7cb8-102">Novērst problēmas, kas saistītas ar mācās Android ierīces Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="f7cb8-102">Troubleshoot issues with enrolling Android devices in Microsoft Intune</span></span>

<span data-ttu-id="f7cb8-103">Pārskata resursu, kas uzskaitīti turpmāk, lai atrisinātu jūsu problēmu tagad.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="f7cb8-104">Dažas biežāk sastopamās problēmas un risināšanas soļi:</span><span class="sxs-lookup"><span data-stu-id="f7cb8-104">Some common issues and resolution steps:</span></span>
  
 <span data-ttu-id="f7cb8-105">**Ierīce nav šifrēts kļūdas uzņēmuma portālā:** Jaunākas versijas Android, sevišķi sākot ar v 7.0, nepieciešams starta patentatslēga, lai pārliecinātos, vai jūsu ierīce ir pilnībā šifrēts.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-105">**Device not Encrypted error in Company Portal:** Newer versions of Android, particularly starting with v7.0, require a startup passcode to make sure that your device is fully encrypted.</span></span> <span data-ttu-id="f7cb8-106">Iespējot startēšanas pin vai pilnībā šifrēt ierīce ir kopīgi risinājumi.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-106">Common solutions are to enable a startup pin or fully encrypt the device.</span></span> <span data-ttu-id="f7cb8-107">Recenzējiet [šo dokumentu](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) plašāku informāciju.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-107">Review [this document](https://docs.microsoft.com/intune-user-help/your-device-appears-encrypted-but-cp-says-otherwise-android) for more information.</span></span>
  
 <span data-ttu-id="f7cb8-108">**Ierīces neizdodas pārbaudi ar Intune pakalpojumu vai parādītu kā "Unhealthy" Intune admin konsole:** Daži Samsung 4,4 un 5,5 ierīces var pārbaudīt ekspluatācijā.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-108">**Devices fail to check in with the Intune service or display as "Unhealthy" in the Intune admin console:** Some Samsung 4.4 and 5.5 devices may not check into the service.</span></span> <span data-ttu-id="f7cb8-109">Pastāv 3 iespējamie risinājumi šo problēmu:</span><span class="sxs-lookup"><span data-stu-id="f7cb8-109">There are 3 possible solutions to this issue:</span></span>
  
1. <span data-ttu-id="f7cb8-110">Manuāli atveriet Intune uzņēmuma portāla app, kas automātiski uzsāks ierīču sinhronizēšanu.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-110">Manually open the Intune Company Portal app, which will automatically initiate a device sync.</span></span>

2. <span data-ttu-id="f7cb8-111">Atjauninātu ierīces Android 6.0 vai augstāku.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-111">Update the device to Android 6.0 or higher.</span></span>

3. <span data-ttu-id="f7cb8-112">Samsung Smart pārvaldnieks atspējošana no pārvaldot uzņēmuma portāls Intune.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-112">Disable Samsung Smart Manager from managing the Intune Company Portal.</span></span> <span data-ttu-id="f7cb8-113">Recenzējiet [šo dokumentu](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) sīkāku informāciju par šiem jautājumiem un rezolūcijas.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-113">Review [this document](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune#devices-fail-to-check-in-with-the-intune-service-and-display-as-unhealthy-in-the-intune-admin-console) for further details on these issues and resolutions.</span></span>

 <span data-ttu-id="f7cb8-114">**Lietotāja licences tipam nederīga** vai **lietotāja nosaukums nav atpazīts kļūda:** lietotāju vajadzībām, piešķir Intune vai EMS licenci.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-114">**User License Type Invalid** or **User Name Not Recognized error:** The user needs to be assigned an Intune or EMS license.</span></span> <span data-ttu-id="f7cb8-115">Pārskatīt šos dokumentus, lai piešķirtu licenci caur: Office Admin Center vai Azure portāls.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-115">Review these documents to assign a license through: Office Admin Center or Azure portal.</span></span>
  
<span data-ttu-id="f7cb8-116">Papildu resursi, kas var palīdzēt atrisināt jūsu problēmu:</span><span class="sxs-lookup"><span data-stu-id="f7cb8-116">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="f7cb8-117">[Intune novēršana portāls](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) jālieto diagnosticē un risina ar kopēju reģistrācijas nepilnības.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-117">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="f7cb8-118">Recenzējiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) sīkāku informāciju.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-118">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

2. <span data-ttu-id="f7cb8-119">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) sarakstu bieži sastopamās kļūdas, kas novērstu iesaistīšanos un rezolūcijas katram.</span><span class="sxs-lookup"><span data-stu-id="f7cb8-119">Review [this document](https://docs.microsoft.com/intune-classic/Troubleshoot/troubleshoot-device-enrollment-in-intune) for a list of common errors that prevent enrollment and resolutions to each.</span></span>

3. <span data-ttu-id="f7cb8-120">[Uzziniet, kā uzņemt Android ierīces Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span><span class="sxs-lookup"><span data-stu-id="f7cb8-120">[Learn how to enroll Android devices in Microsoft Intune](https://docs.microsoft.com/intune/android-enroll).</span></span>
