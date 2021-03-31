---
title: Hibrīda Azure Active Directory savienojuma problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 08/06/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6162"
- "6158"
- "9003244"
- "9003246"
ms.openlocfilehash: 18d0ce6bdf3df96e07cc6607b9ae6142d548dabe
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51401914"
---
# <a name="troubleshoot-hybrid-azure-ad-join"></a><span data-ttu-id="83886-102">Hibrīda Azure Active Directory savienojuma problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="83886-102">Troubleshoot Hybrid Azure AD join</span></span>

<span data-ttu-id="83886-103">Ļoti ieteicams nodrošināt, ka ierīce var piekļūt ierīces reģistrācijas galapunktiem sistēmas kontā, izmantojot [Ierīces reģistrācijas savienojamības testa skriptu](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span><span class="sxs-lookup"><span data-stu-id="83886-103">Highly Recommended Ensure that a device can access Device Registration endpoints under the system account by using the [Test Device Registration Connectivity script](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/).</span></span>

1. <span data-ttu-id="83886-104">Ja ierīču reģistrācijas iestatāt pirmo reizi, noteikti pārskatiet sadaļu [Ievads par ierīču pārvaldību Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/), lai uzzinātu, kā pārvaldīt Azure Active Directory.</span><span class="sxs-lookup"><span data-stu-id="83886-104">If you are setting up device registrations for the first time, be sure to review I[ntroduction to device management in Azure Active Directory](https://docs.microsoft.com/samples/azure-samples/testdeviceregconnectivity/testdeviceregconnectivity/) to learn how to get devices under the control of Azure AD.</span></span>
1. <span data-ttu-id="83886-105">Ja tieši reģistrējat ierīces Azure AD un reģistrējat tās Intune, pārliecinieties, vai esat [konfigurējis Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) un ka instalētas [licences](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="83886-105">If you are registering devices into Azure AD directly and enrolling them into Intune, be sure that you've [configured Intune](https://docs.microsoft.com/mem/intune/enrollment/device-enrollment?WT.mc_id=Portal-Microsoft_Azure_Support) and have the [licensing](https://docs.microsoft.com/mem/intune/fundamentals/licenses-assign?WT.mc_id=Portal-Microsoft_Azure_Support) in place first.</span></span>
1. <span data-ttu-id="83886-106">Pārliecinieties, vai esat pilnvarots veikt darbības Azure Active Directory un lokālajā Active Directory.</span><span class="sxs-lookup"><span data-stu-id="83886-106">Ensure that you are authorized to perform operations in Azure AD and on-premises AD.</span></span> <span data-ttu-id="83886-107">Ierīču reģistrāciju iestatījumus var pārvaldīt tikai Azure Active Directory globālais administrators.</span><span class="sxs-lookup"><span data-stu-id="83886-107">Only a global administrator in Azure AD can manage settings for device registrations.</span></span> <span data-ttu-id="83886-108">Turklāt, ja iestatāt automātiskas reģistrācijas lokālajā Active Directory, jums būs jābūt Active Directory un AD FS administratoram (ja piemērojams).</span><span class="sxs-lookup"><span data-stu-id="83886-108">In addition, if you are setting up automatic registrations in your on-premises Active Directory, you will need to be an administrator of Active Directory and AD FS (if applicable).</span></span>

<span data-ttu-id="83886-109">Papildinformāciju par iespējamo hibrīdā savienojuma problēmu risināšanu skatiet rakstā [Hibrīda savienojuma problēmu novēršana](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current), lai iestatītu hibrīda Azure Active Directory pievienotās un pārvaldītās ierīces, izmantojot Azure Active Directory portālu, skatiet rakstu [Hibrīda Azure AD pievienoto (lokālajam domēnam pievienoto) ierīču iestatīšana](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) un [Ierīču pārvaldība, izmantojot Azure portālu](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span><span class="sxs-lookup"><span data-stu-id="83886-109">For more details on resolve potential issues with Hybrid join, see [Troubleshoot Hybrid Join](https://docs.microsoft.com/azure/active-directory/devices/troubleshoot-hybrid-join-windows-current) for set up hybrid Azure AD joined and Manage Devices using Azure Ad portal, see [Set up hybrid Azure AD joined (on-premises domain-joined) devices](https://docs.microsoft.com/azure/active-directory/devices/hybrid-azuread-join-plan?WT.mc_id=Portal-Microsoft_Azure_Support) and [Manage devices using the Azure portal](https://docs.microsoft.com/azure/active-directory/devices/device-management-azure-portal?WT.mc_id=Portal-Microsoft_Azure_Support).</span></span>

<span data-ttu-id="83886-110">Lai novērstu bieži sastopamas problēmas ar hibrīda Azure Active Directory (AD) savienojumu, skatiet rakstu [Bieži uzdotie jautājumi par hibrīda Azure Active Directory](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span><span class="sxs-lookup"><span data-stu-id="83886-110">To resolve common issues with Hybrid Azure Active Directory (AD) join, see [Hybrid Azure AD join FAQ](https://docs.microsoft.com/azure/active-directory/devices/faq#hybrid-azure-ad-join-faq).</span></span>
