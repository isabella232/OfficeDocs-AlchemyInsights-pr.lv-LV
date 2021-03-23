---
title: Azure Active Directory tranzīta autentifikācijas konfigurēšana
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/19/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6970"
- "9003915"
ms.openlocfilehash: be993b1f22d89a92afb099937dae815dc9c09e0e
ms.sourcegitcommit: c08bed4071baa3bb5879496df3ed44fb828c8367
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/19/2021
ms.locfileid: "51036299"
---
# <a name="configure-azure-active-directory-pass-through-authentication"></a><span data-ttu-id="f1666-102">Azure Active Directory tranzīta autentifikācijas konfigurēšana</span><span class="sxs-lookup"><span data-stu-id="f1666-102">Configure Azure Active Directory pass-through authentication</span></span>

<span data-ttu-id="f1666-103">Šeit sniegti daži ceļveži, kas palīdzēs konfigurēt tranzīta autentifikāciju:</span><span class="sxs-lookup"><span data-stu-id="f1666-103">Here are some guides to help you configure pass-through authentication:</span></span>

- <span data-ttu-id="f1666-104">**Lai iestatītu Azure Active Directory savienojumu**: [sinhronizācijas lietotāji jūsu direktorija](https://admin.microsoft.com/AdminPortal/Home) rokasgrāmatā palīdz konfigurēt paroļu jaukšanas sinhronizāciju vai tranzīta autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="f1666-104">**To set up Azure Active Directory Connect**: The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide helps you configure password hash synchronization or pass-through authentication.</span></span> <span data-ttu-id="f1666-105">Šī konfigurācija ļauj lietotājiem pierakstīties savā e-pastā un lokālā Active Directory (domēna kontrollerim), izmantojot vienu un to pašu paroli.</span><span class="sxs-lookup"><span data-stu-id="f1666-105">This configuration enables users to sign in to their email and to your on-premises Active Directory (domain controller) using the same password.</span></span>  <span data-ttu-id="f1666-106">[Sinhronizācijas lietotāji direktorija](https://admin.microsoft.com/AdminPortal/Home) rokasgrāmatā attiecas arī uz Federācijas pierakstīšanos, izmantojot Active Directory Federācijas pakalpojumu (AD FS).</span><span class="sxs-lookup"><span data-stu-id="f1666-106">The [Sync users to your directory](https://admin.microsoft.com/AdminPortal/Home) guide also covers federation sign-in with Active Directory Federation Services (AD FS), too.</span></span>

- <span data-ttu-id="f1666-107">**Lai iestatītu Azure līdzekļus**: Azure [ad iestatīšanas ceļvedis](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) palīdz iestatīt Azure Active Directory pamata līdzekļus, piemēram, grupas piekļuves pārvaldību, pašapkalpošanās paroles atiestatīšanu mākonī un Azure Active Directory lietojumprogrammas starpniekserveri, lai publicētu lokālās tīmekļa lietojumprogrammas.</span><span class="sxs-lookup"><span data-stu-id="f1666-107">**To set up Azure features**: The [Azure AD setup guide](https://admin.microsoft.com/adminportal/home#/modernonboarding/azureadsetup) walks you through setting up the features in Azure Active Directory Basic, like group-based access management, self-service password reset for cloud apps, and Azure Active Directory Application Proxy for publishing on-premises web apps.</span></span>


