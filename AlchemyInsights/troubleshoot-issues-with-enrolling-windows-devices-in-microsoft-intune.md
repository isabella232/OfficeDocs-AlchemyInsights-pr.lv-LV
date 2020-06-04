---
title: Problēmu novēršana saistībā ar Windows ierīču uzskaitīmēšanas Microsoft InTune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 7b298360fe31d3f52ef382e5b8f25ee3588c36c8
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "36665839"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="786f9-102">Problēmu novēršana saistībā ar Windows ierīču uzskaitīmēšanas Microsoft InTune</span><span class="sxs-lookup"><span data-stu-id="786f9-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="786f9-103">Pārskatiet tālāk uzskaitītos resursus, lai atrisinātu problēmu tūlīt.</span><span class="sxs-lookup"><span data-stu-id="786f9-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="786f9-104">Daži bieži sastopami kļūdu ziņojumi un atrisināšanas darbības:</span><span class="sxs-lookup"><span data-stu-id="786f9-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="786f9-105">**Programmatūru nevar instalēt, 0x80cf4017:** Jūsu konta sertifikātam ir beidzies derīgums.</span><span class="sxs-lookup"><span data-stu-id="786f9-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="786f9-106">Atkārtoti lejupielādējiet datora klienta programmatūras pakotni InTune administrēšanas konsole.</span><span class="sxs-lookup"><span data-stu-id="786f9-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="786f9-107">Pārskatiet šo dokumentāciju, lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="786f9-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="786f9-108">**Kļūdas kods 0x801c0003:** Kļūda var rasties šādos gadījumos:</span><span class="sxs-lookup"><span data-stu-id="786f9-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="786f9-109">Lietotājs ir uzņemti vairāk ierīču nekā ierīces ierobežojumu.</span><span class="sxs-lookup"><span data-stu-id="786f9-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="786f9-110">Pārskatiet šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) vai [mainītu ierīces ierobežojumu](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="786f9-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="786f9-111">"Lietotāji var pievienoties ierīces Azure AD" ir iestatīts uz "none".</span><span class="sxs-lookup"><span data-stu-id="786f9-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="786f9-112">Iestatiet to visiem vai atlasiet lietotāji.</span><span class="sxs-lookup"><span data-stu-id="786f9-112">Set it to all or select users.</span></span> <span data-ttu-id="786f9-113">Pārskatiet [šo dokumentāciju](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) , lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="786f9-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="786f9-114">Ierīci jau ir reģistrējušies cits lietotājs.</span><span class="sxs-lookup"><span data-stu-id="786f9-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="786f9-115">Šādā gadījumā noņemiet ierīci no Azure InTune konsoles vai manuāli atreģistrējiet ierīci, pirms mēģināt vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="786f9-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="786f9-116">Ierīce ir Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="786f9-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="786f9-117">Azure Active Directory var pievienoties tikai Windows 10 Pro, Education un Enterprise SKUs.</span><span class="sxs-lookup"><span data-stu-id="786f9-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="786f9-118">Papildu resursus, lai palīdzētu atrisināt jūsu problēmu:</span><span class="sxs-lookup"><span data-stu-id="786f9-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="786f9-119">Izmantojiet [InTune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu vispārējas reģistrācijas kļūmes.</span><span class="sxs-lookup"><span data-stu-id="786f9-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="786f9-120">Pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) , lai iegūtu detalizētu informāciju.</span><span class="sxs-lookup"><span data-stu-id="786f9-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="786f9-121">Pārskatiet šos dokumentus, lai iegūtu sarakstu ar bieži sastopamas kļūdas, kas neļauj iesaistīšanās un risinājumi: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) un [problēmu novēršana doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="786f9-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="786f9-122">[Uzziniet, kā reģistrēt Windows ierīces Microsoft InTune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="786f9-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
