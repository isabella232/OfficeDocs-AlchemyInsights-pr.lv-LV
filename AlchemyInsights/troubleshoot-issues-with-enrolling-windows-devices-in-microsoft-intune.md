---
title: Problēmu novēršana saistībā ar Windows ierīču reģistrāciju programmā Microsoft Intune
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 20e9bd42-2db0-4dd7-b480-966571494dd9
ms.custom:
- "784"
- "6200002"
ms.openlocfilehash: a456cc8f2336e6b902de0b7873cb233f4b846140
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51808978"
---
# <a name="troubleshoot-issues-with-enrolling-windows-devices-in-microsoft-intune"></a><span data-ttu-id="e34e3-102">Problēmu novēršana saistībā ar Windows ierīču reģistrāciju programmā Microsoft Intune</span><span class="sxs-lookup"><span data-stu-id="e34e3-102">Troubleshoot issues with enrolling Windows devices in Microsoft Intune</span></span>

<span data-ttu-id="e34e3-103">Pārskatiet tālāk norādītos resursus, lai tūlīt novērstu savu problēmu.</span><span class="sxs-lookup"><span data-stu-id="e34e3-103">Review the resources listed below to resolve your issue now.</span></span>
  
<span data-ttu-id="e34e3-104">Daži bieži sastopami kļūdu ziņojumi un risinājuma darbības:</span><span class="sxs-lookup"><span data-stu-id="e34e3-104">Some common error messages and resolution steps:</span></span>
  
 <span data-ttu-id="e34e3-105">**Programmatūru nevar instalēt, un 0x80cf4017:** Jūsu konta sertifikāta derīgums ir beidzies.</span><span class="sxs-lookup"><span data-stu-id="e34e3-105">**The software cannot be installed, 0x80cf4017:** Your account certificate has expired.</span></span> <span data-ttu-id="e34e3-106">Atkārtoti lejupielādējiet PC Client programmatūras pakotni Intune administratora konsolē.</span><span class="sxs-lookup"><span data-stu-id="e34e3-106">Re-download the PC Client software package in the Intune Admin Console.</span></span> <span data-ttu-id="e34e3-107">Lai iegūtu papildinformāciju, pārskatiet šo dokumentāciju.</span><span class="sxs-lookup"><span data-stu-id="e34e3-107">Review this documentation for more information.</span></span>
  
 <span data-ttu-id="e34e3-108">**Kļūdas kods 0x801c0003:** Kļūda var rasties šādos scenārijos:</span><span class="sxs-lookup"><span data-stu-id="e34e3-108">**Error code 0x801c0003:** The error can occur in the following scenarios:</span></span>
  
-  <span data-ttu-id="e34e3-109">Lietotājam ir reģistrēts vairāk ierīču, nekā ierīces ierobežojums.</span><span class="sxs-lookup"><span data-stu-id="e34e3-109">The user has more devices enrolled than the device limit.</span></span> <span data-ttu-id="e34e3-110">Pārskatiet šos [dokumentus, lai noņemtu ierīci](https://docs.microsoft.com/intune/devices-wipe) [vai mainītu ierīču ierobežojumu.](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions)</span><span class="sxs-lookup"><span data-stu-id="e34e3-110">Review these documents to [remove a device](https://docs.microsoft.com/intune/devices-wipe) or [change the device limit](https://docs.microsoft.com/intune/enrollment-restrictions-set#set-device-limit-restrictions).</span></span>

-  <span data-ttu-id="e34e3-111">"Lietotāji var savienot ierīces ar Azure AD" ir iestatīts uz "none".</span><span class="sxs-lookup"><span data-stu-id="e34e3-111">"Users may join devices to Azure AD" is set to "none."</span></span> <span data-ttu-id="e34e3-112">Iestatiet to visiem vai atlasiet lietotājus.</span><span class="sxs-lookup"><span data-stu-id="e34e3-112">Set it to all or select users.</span></span> <span data-ttu-id="e34e3-113">Lai [iegūtu papildinformāciju,](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) pārskatiet šo dokumentāciju.</span><span class="sxs-lookup"><span data-stu-id="e34e3-113">Review [this documentation](https://docs.microsoft.com/azure/active-directory/device-management-azure-portal#configure-device-settings) for more information.</span></span>

-  <span data-ttu-id="e34e3-114">Ierīci jau ir reģistrējis cits lietotājs.</span><span class="sxs-lookup"><span data-stu-id="e34e3-114">The device is already enrolled by another user.</span></span> <span data-ttu-id="e34e3-115">Šādā gadījumā noņemiet ierīci no Azure Intune konsoles vai manuāli atņemiet ierīces sarakstu, pirms mēģināt vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="e34e3-115">If that's the case, remove the device from the Azure Intune console or manually unenroll the device before trying again.</span></span>

-  <span data-ttu-id="e34e3-116">Ierīce ir Windows 10 Home.</span><span class="sxs-lookup"><span data-stu-id="e34e3-116">The device is Windows 10 Home.</span></span> <span data-ttu-id="e34e3-117">Pakalpojumam Azure Active Directory var pievienoties tikai Windows 10 Pro, Education un Enterprise SKU.</span><span class="sxs-lookup"><span data-stu-id="e34e3-117">Only Windows 10 Pro, Education and Enterprise SKUs can join Azure Active Directory.</span></span>

<span data-ttu-id="e34e3-118">Papildu resursi, lai palīdzētu novērst problēmu:</span><span class="sxs-lookup"><span data-stu-id="e34e3-118">Additional resources to help resolve your issue:</span></span>
  
-  <span data-ttu-id="e34e3-119">Izmantojiet [Intune problēmu novēršanas portālu,](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) lai diagnosticētu un novērstu bieži sastopamās reģistrācijas kļūmes.</span><span class="sxs-lookup"><span data-stu-id="e34e3-119">Use [Intune Troubleshooting Portal](https://devicemanagement.microsoft.com/#blade/Microsoft_Intune_DeviceSettings/TroubleshootBlade) to diagnose and resolve common enrollment failures.</span></span> <span data-ttu-id="e34e3-120">Pārskatiet [šo dokumentu,](https://docs.microsoft.com/intune/help-desk-operators) lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="e34e3-120">Review [this document](https://docs.microsoft.com/intune/help-desk-operators) for more details.</span></span>

-  <span data-ttu-id="e34e3-121">Pārskatiet šos dokumentus, lai iegūtu sarakstu ar bieži sastopamajām kļūdām, kas novērš reģistrāciju un atrisināšanu katrā sarakstā: Problēmu novēršanas [rokasgrāmata](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) un [Problēmu novēršana dokumentā](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span><span class="sxs-lookup"><span data-stu-id="e34e3-121">Review these documents for a list of common errors that prevent enrollment and resolutions to each: [Troubleshooting guide](https://support.microsoft.com/help/4089533/troubleshooting-windows-device-enrollment-problems-in-microsoft-intune) and [Troubleshooting doc](https://docs.microsoft.com/troubleshoot/mem/intune/troubleshoot-device-enrollment-in-intune).</span></span>

<span data-ttu-id="e34e3-122">[Uzziniet, kā reģistrēt Windows ierīces programmā Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span><span class="sxs-lookup"><span data-stu-id="e34e3-122">[Learn how to enroll Windows devices in Microsoft Intune](https://docs.microsoft.com/intune/windows-enroll).</span></span>
