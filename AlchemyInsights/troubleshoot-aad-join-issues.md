---
title: Azure AD pievienošanās problēmu novēršana
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
- "9003246"
- "6157"
ms.openlocfilehash: 0e9f7c95cf522340e9976f668c1d1a9eaff71910
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405129"
---
# <a name="troubleshoot-azure-ad-join-issues"></a><span data-ttu-id="9b0c4-102">Azure AD pievienošanās problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="9b0c4-102">Troubleshoot Azure AD join issues</span></span>

1. <span data-ttu-id="9b0c4-103">Ja iestatāt ierīču reģistrācijas pirmo reizi, pārliecinieties, vai esat pārskatījis Ievads par ierīču pārvaldību pakalpojumā [Azure Active Directory,](https://docs.microsoft.com/azure/active-directory/devices/overview) kas sniegs norādījumus par to, kā Azure AD vadīklā iegūt ierīces.</span><span class="sxs-lookup"><span data-stu-id="9b0c4-103">If you are setting up device registrations for the first time, ensure that you have reviewed [Introduction to device management in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/overview) that will guide you on how to get Devices under the control to Azure AD.</span></span> 
1. <span data-ttu-id="9b0c4-104">Ja reģistrējat ierīces Azure AD tieši un reģistrējat tās Intune, jums vispirms ir jākonfigurē [Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) un vispirms jāveic licencēšana. [](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign)</span><span class="sxs-lookup"><span data-stu-id="9b0c4-104">If you are registering devices into Azure AD directly and enrolling them into Intune, you will need to ensure that you have [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign) in place first.</span></span>
1. <span data-ttu-id="9b0c4-105">Pārliecinieties, vai esat pilnvarots veikt darbības Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9b0c4-105">Ensure you are authorized to perform operations in Azure AD.</span></span> <span data-ttu-id="9b0c4-106">Ierīces reģistrāciju iestatījumus var pārvaldīt tikai globālais administrators Azure AD.</span><span class="sxs-lookup"><span data-stu-id="9b0c4-106">Only a global administrator in Azure AD can manage settings for device registrations.</span></span>
1. <span data-ttu-id="9b0c4-107">Lai ieviestu Azure AD savienojumu, skatiet [rakstu Azure AD pievienošanās plānošana.](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan)</span><span class="sxs-lookup"><span data-stu-id="9b0c4-107">To do Azure AD join implementation, see [Plan Azure AD Join](https://docs.microsoft.com/azure/active-directory/devices/azureadjoin-plan).</span></span>

<span data-ttu-id="9b0c4-108">Lai iegūtu papildinformāciju par bieži sastopamo problēmu novēršanu saistībā ar Azure AD savienojumu, skatiet rakstu Bieži uzdotie jautājumi par [Azure Ad Join](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) un Windows 10 pro ierīcēm, skatiet rakstu Nevar pievienoties Windows [10 Pro](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900) datoram uz Azure AD — Jaunināšana — Microsoft kopiena</span><span class="sxs-lookup"><span data-stu-id="9b0c4-108">For more details on resolving  common issues with Azure AD join see [Azure Ad Join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#azure-ad-join-faq) and for Windows 10 pro device, see [Unable to join Windows 10 Pro machine to Azure AD - Need to upgrade to - Microsoft Community](https://answers.microsoft.com/en-us/msoffice/forum/msoffice_install-mso_win10-mso_365hp/unable-to-join-windows-10-pro-machine-to-azure-ad/abb1ca7d-b317-45ec-a628-e1c10eae2900)</span></span>
