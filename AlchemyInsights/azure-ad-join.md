---
title: Azure Active Directory savienojums
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003257"
- "9890"
ms.openlocfilehash: 59e3798131956847a61af2416c2e4210199cffa5
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405056"
---
# <a name="azure-active-directory-join"></a><span data-ttu-id="932cc-102">Azure Active Directory savienojums</span><span class="sxs-lookup"><span data-stu-id="932cc-102">Azure Active Directory join</span></span>

1. <span data-ttu-id="932cc-103">Ja iestatāt ierīču reģistrācijas pirmo reizi, pārliecinieties, vai esat pārskatījis Ievads par ierīču pārvaldību pakalpojumā [Azure Active Directory,](/azure/active-directory/devices/overview) kas sniegs norādījumus par to, kā Azure AD vadīklā iegūt ierīces.</span><span class="sxs-lookup"><span data-stu-id="932cc-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="932cc-104">Ja reģistrējat ierīces Azure AD tieši un reģistrējat tās Intune, jums vispirms ir jākonfigurē [Intune](/mem/intune/enrollment/device-enrollment) un vispirms jāveic licencēšana. [](/mem/intune/fundamentals/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="932cc-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](/mem/intune/enrollment/device-enrollment) and have the [licensing](/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="932cc-105">Pārliecinieties, vai esat pilnvarots veikt darbības Azure AD.</span><span class="sxs-lookup"><span data-stu-id="932cc-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="932cc-106">Ierīces reģistrāciju iestatījumus var pārvaldīt tikai globālais administrators Azure AD.</span><span class="sxs-lookup"><span data-stu-id="932cc-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="932cc-107">Lai ieviestu Azure AD savienojumu, skatiet [rakstu Azure AD pievienošanās plānošana.](/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="932cc-107">To do Azure AD join implementation, see [Plan Azure AD Join](/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="932cc-108">Papildinformāciju par bieži sastopamo problēmu novēršanu saistībā ar Azure AD savienojumu skatiet rakstā Bieži uzdotie jautājumi par [Azure Ad Join](/azure/active-directory/devices/faq) un Windows 10 pro ierīcēm skatiet rakstā Nevar pievienoties Windows [10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)datoram uz Azure AD — jaunināšana — Microsoft kopiena.</span><span class="sxs-lookup"><span data-stu-id="932cc-108">For more details on resolving common issues with Azure AD join, see [Azure Ad Join FAQ](/azure/active-directory/devices/faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900).</span></span>
