---
title: Problēmu novēršana saistībā ar Windows ierīču reģistrēšanu pakalpojumā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: 13dc77fd2a575fbd227a2a880438b78aaa2c3fb2
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47658885"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="a0310-102">Problēmu novēršana saistībā ar Windows ierīču reģistrēšanu pakalpojumā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="a0310-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="a0310-103">Pārskatiet tālāk norādītos resursus, lai atrisinātu savu problēmu tūlīt.</span><span class="sxs-lookup"><span data-stu-id="a0310-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="a0310-104">Daži bieži sastopami kļūdu ziņojumi un atrisināšanas darbības:</span><span class="sxs-lookup"><span data-stu-id="a0310-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="a0310-105">**Šo programmatūru nevar instalēt, 0x80cf4017:** Jūsu konta sertifikāta derīguma termiņš ir beidzies.</span><span class="sxs-lookup"><span data-stu-id="a0310-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="a0310-106">Atkārtoti lejupielādējiet PC klienta programmatūras pakotni Intune administratora konsolē.</span><span class="sxs-lookup"><span data-stu-id="a0310-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="a0310-107">Lai iegūtu papildinformāciju, pārskatiet šo dokumentāciju.</span><span class="sxs-lookup"><span data-stu-id="a0310-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="a0310-108">**Kļūdas kods 0x801c0003:** Kļūda var rasties tālāk norādītajos gadījumos.</span><span class="sxs-lookup"><span data-stu-id="a0310-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="a0310-109">Lietotājam ir vairāk ierīču, kas reģistrējušies nekā ierīces ierobežojums.</span><span class="sxs-lookup"><span data-stu-id="a0310-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="a0310-110">Pārskatiet šos dokumentus, lai [noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) vai [mainītu ierīces ierobežojumu](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span><span class="sxs-lookup"><span data-stu-id="a0310-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="a0310-111">"Lietotāji var pievienoties ierīcēm uz Azure AD" ir iestatīts uz "nav".</span><span class="sxs-lookup"><span data-stu-id="a0310-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="a0310-112">Iestatiet to visiem vai atlasiet lietotāji.</span><span class="sxs-lookup"><span data-stu-id="a0310-112">Set it to all or select users.</span></span> <span data-ttu-id="a0310-113">Lai iegūtu papildinformāciju, pārskatiet [šo dokumentāciju](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) .</span><span class="sxs-lookup"><span data-stu-id="a0310-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="a0310-114">Ierīci jau ir reģistrējis cits lietotājs.</span><span class="sxs-lookup"><span data-stu-id="a0310-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="a0310-115">Ja tā ir, izņemiet ierīci no Azure Intune konsoles vai manuāli noņemiet ierīci, pirms mēģināt vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="a0310-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="a0310-116">Ierīce ir Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="a0310-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="a0310-117">Azure Active Directory var pievienot tikai Windows 10 Pro, Education un Enterprise SKU.</span><span class="sxs-lookup"><span data-stu-id="a0310-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="a0310-118">Papildu resursi, kas palīdz novērst problēmu:</span><span class="sxs-lookup"><span data-stu-id="a0310-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="a0310-119">Izmantojiet [Intune problēmu novēršanas portālu](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) , lai diagnosticētu un novērstu Biežākās reģistrācijas kļūmes.</span><span class="sxs-lookup"><span data-stu-id="a0310-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="a0310-120">Lai iegūtu papildinformāciju, pārskatiet [šo dokumentu](https://docs.microsoft.com/intune/help-desk-operators) .</span><span class="sxs-lookup"><span data-stu-id="a0310-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="a0310-121">Pārskatiet šos dokumentus, lai skatītu sarakstu ar bieži sastopamām kļūdām, kas neļauj veikt reģistrāciju un risinājumus: [problēmu novēršanas rokasgrāmata](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) un [problēmu novēršana](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="a0310-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/intune-classic/troubleshoot/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="a0310-122">[Uzziniet, kā sistēmā Microsoft Intune reģistrēt Windows ierīces](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="a0310-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
