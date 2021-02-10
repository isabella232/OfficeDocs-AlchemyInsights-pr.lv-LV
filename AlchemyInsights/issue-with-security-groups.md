---
title: Problēma ar drošības grupām
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 02/09/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "8252"
- "9004397"
ms.openlocfilehash: 1198b79c3301bd2752a7385a6ba6746c8f0c2b5b
ms.sourcegitcommit: 22eaf0a151ab95414476f596db8d318b6540ff31
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/09/2021
ms.locfileid: "50177498"
---
# <a name="issue-with-security-groups"></a><span data-ttu-id="297ad-102">Problēma ar drošības grupām</span><span class="sxs-lookup"><span data-stu-id="297ad-102">Issue with security groups</span></span>

<span data-ttu-id="297ad-103">**Ja saņemat tīkla kļūdu AADDS104**</span><span class="sxs-lookup"><span data-stu-id="297ad-103">**If you are getting Network Error AADDS104**</span></span>

<span data-ttu-id="297ad-104">Nederīgi tīkla drošības grupas kārtulas ir visbiežāk sastopamais tīkla kļūdu cēlonis Azure Active Directory domēna pakalpojumos (AD DS).</span><span class="sxs-lookup"><span data-stu-id="297ad-104">Invalid network security group rules are the most common cause of network errors for Azure Active Directory Domain Services (AD DS).</span></span> <span data-ttu-id="297ad-105">Virtuālā tīkla tīkla drošības grupai ir jāatļauj piekļūt konkrētiem portiem un protokoliem.</span><span class="sxs-lookup"><span data-stu-id="297ad-105">The network security group for the virtual network must allow access to specific ports and protocols.</span></span> <span data-ttu-id="297ad-106">Ja šie porti ir bloķēti, Azure Platform nevar pārraudzīt vai atjaunināt pārvaldīto domēnu.</span><span class="sxs-lookup"><span data-stu-id="297ad-106">If these ports are blocked, the Azure platform can't monitor or update the managed domain.</span></span> <span data-ttu-id="297ad-107">Tiek ietekmēta arī sinhronizēšana starp Azure AD un Azure AD DS.</span><span class="sxs-lookup"><span data-stu-id="297ad-107">The synchronization between the Azure AD and Azure AD DS is also impacted.</span></span> <span data-ttu-id="297ad-108">Pārliecinieties, vai ir pieejami noklusējuma porti, lai izvairītos no pakalpojuma darbības traucējumiem.</span><span class="sxs-lookup"><span data-stu-id="297ad-108">Ensure you keep the default ports open to avoid interruption in service.</span></span>

<span data-ttu-id="297ad-109">Lai izprastu un novērstu vispārējus brīdinājumus par tīkla drošības grupas konfigurācijas problēmām, skatiet rakstu [drošības grupu pievienošana un pārbaude](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span><span class="sxs-lookup"><span data-stu-id="297ad-109">To understand and to resolve common alerts for network security group configuration issues, see [Add and Verify Security Groups](https://docs.microsoft.com/azure/active-directory-domain-services/alert-nsg#verify-and-edit-existing-security-rules).</span></span>
