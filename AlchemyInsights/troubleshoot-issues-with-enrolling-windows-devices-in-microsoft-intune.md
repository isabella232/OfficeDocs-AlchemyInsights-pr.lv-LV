---
title: Novērst problēmas, kas saistītas ar Microsoft Intune Windows ierīču mācās
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 10/24/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.openlocfilehash: 8d19bbd5a5782c7793c87499baf62b2eb7de82ae
ms.sourcegitcommit: d6ea5e9458a2b8ceaab3ac4bd483e1130b9a398a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/15/2019
ms.locfileid: "28300788"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="23db7-102">Novērst problēmas, kas saistītas ar Microsoft Intune Windows ierīču mācās</span><span class="sxs-lookup"><span data-stu-id="23db7-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="23db7-103">Pārskata resursu, kas uzskaitīti turpmāk, lai atrisinātu jūsu problēmu tagad.</span><span class="sxs-lookup"><span data-stu-id="23db7-103">Review the resources listed below to resolve your issue now.</span></span> 
  
<span data-ttu-id="23db7-104">Daži izplatītākie kļūdu ziņojumi un rezolūcijas darbības:</span><span class="sxs-lookup"><span data-stu-id="23db7-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="23db7-p101">**Programmatūru nevar instalēt, 0x80cf4017:** Jūsu kontā sertifikātu derīguma termiņš ir beidzies. Atkārtoti ielādēt PC klienta programmatūras pakotnes Intune Admin konsole. Pārskatīt šo dokumentāciju, lai iegūtu vairāk informācijas.</span><span class="sxs-lookup"><span data-stu-id="23db7-p101">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired. Re-download the PC Client software package in the Intune Admin Console. Review this documentation for more information.</span></span> 
  
 <span data-ttu-id="23db7-108">**0x801c0003. kļūdas kods:** Kļūda var rasties šādos gadījumos:</span><span class="sxs-lookup"><span data-stu-id="23db7-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span> 
  
1. <span data-ttu-id="23db7-p102">Lietotājam ir vairākas ierīces, kas uzņemti nekā ierīces ierobežojums. Pārskatīt šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/en-us/intune/devices-wipe) vai [mainīt ierīces ierobežojums](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="23db7-p102">The user has more devices enrolled than the device limit. Review these documents to [remove a device](https://docs.microsoft.com/en-us/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/en-us/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>
    
2. <span data-ttu-id="23db7-p103">"Lietotāji var pievienot ierīces debeszils reklāmu" ir iestatīts uz "neviens". Iestatīt tā, lai visu vai atlasiet lietotāju. Pārskatīt [šo dokumentāciju](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="23db7-p103">"Users may join devices to Azure AD" is set to "none". Set it to all or select users. Review [this documentation](https://docs.microsoft.com/en-us/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span> 
    
3. <span data-ttu-id="23db7-p104">Cits lietotājs ir reģistrējies ierīci. Ja tas tā ir gadījumā, izņemiet ierīci no Azure Intune konsole vai manuāli unenroll ierīci, pirms mēģināt vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="23db7-p104">The device is already enrolled by another user. If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>
    
4. <span data-ttu-id="23db7-p105">Ierīcē ir Windows 10 mājās. Tikai Windows 10 Pro, izglītība un Enterprise SKU var pievienoties Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="23db7-p105">The device is Windows 10 Home. Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>
    
<span data-ttu-id="23db7-118">Papildu resursi, kas var palīdzēt atrisināt jūsu problēmu:</span><span class="sxs-lookup"><span data-stu-id="23db7-118">Additional resources to help resolve your issue:</span></span>
  
1. <span data-ttu-id="23db7-p106">[Intune novēršana portāls](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) jālieto diagnosticē un risina ar kopēju reģistrācijas nepilnības. Recenzējiet [šo dokumentu](https://docs.microsoft.com/en-us/intune/help-desk-operators) sīkāku informāciju.</span><span class="sxs-lookup"><span data-stu-id="23db7-p106">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures. Review [this document](https://docs.microsoft.com/en-us/intune/help-desk-operators) for more details.</span></span> 
    
2. <span data-ttu-id="23db7-121">Pārskatīt šos dokumentus bieži sastopamās kļūdas, kas novērstu iesaistīšanos un rezolūcijām uz katru sarakstu: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) un [traucējummeklēšana doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="23db7-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/en-us/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/en-us/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>
    
<span data-ttu-id="23db7-122">[Uzziniet, kā pieteikties Microsoft Intune Windows ierīču](https://docs.microsoft.com/en-us/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="23db7-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/en-us/intune/windows-enroll).</span></span>
  

