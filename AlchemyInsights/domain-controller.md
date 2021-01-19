---
title: Domēna kontrolleris
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/17/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7909"
- "9003233"
ms.openlocfilehash: d4cbe80c3e8f0ce32fcbe89e852f24efd6f50575
ms.sourcegitcommit: 6d02eb533fd74199af6b20f714b3720991da2c4a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49901027"
---
# <a name="domain-controller"></a><span data-ttu-id="688ee-102">Domēna kontrolleris</span><span class="sxs-lookup"><span data-stu-id="688ee-102">Domain controller</span></span>

<span data-ttu-id="688ee-103">**Nevar iespējot AAD-DS vai izvietošanas kļūmi**</span><span class="sxs-lookup"><span data-stu-id="688ee-103">**Unable to enable AAD-DS or deployment is failing**</span></span>

<span data-ttu-id="688ee-104">Lai atrisinātu Azure AD Domain Service (AAD-DS) problēmu, kas nav iespējota vai netiek izvietota, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="688ee-104">To solve the issue of Azure AD domain service (AAD-DS) not being enabled or failing to be deployed, perform the following steps:</span></span>

1. <span data-ttu-id="688ee-105">Ja izmantojat jau esošu virtuālo tīklu, atzīmējiet savu NSG, lai iegūtu kārtulas, kas bloķē portus, kas nepieciešami, lai sinhronizētu ar AAD-DS portālā https://aka.ms/aadds-networking .</span><span class="sxs-lookup"><span data-stu-id="688ee-105">If you are using an already existing virtual network, check your NSG for rules that block ports needed to synchronize in AAD-DS in the portal https://aka.ms/aadds-networking.</span></span>
2. <span data-ttu-id="688ee-106">Pārbaudiet, vai jūsu kļūdas ziņojums ir atbildēts šajā rakstā pieejamā problēmu novēršanas rokasgrāmatā  https://aka.ms/aadds-troubleshoot-enable .</span><span class="sxs-lookup"><span data-stu-id="688ee-106">Check to see if your error message is answered in this troubleshooting guide that is available in  https://aka.ms/aadds-troubleshoot-enable.</span></span>
3. <span data-ttu-id="688ee-107">Izmēģiniet Azure AD Domain pakalpojumu izvietošanu jaunā virtuālajā tīklā.</span><span class="sxs-lookup"><span data-stu-id="688ee-107">Try deploying Azure AD Domain Services in a new virtual network.</span></span>
4. <span data-ttu-id="688ee-108">Izpildiet darba sākšanas instrukciju par to, kā izvietot AAD-DS, kas ir pieejams [apmācība AZURE ad Domain pakalpojumu izveidei](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span><span class="sxs-lookup"><span data-stu-id="688ee-108">Follow the Getting Started guide on how to deploy AAD-DS, which is available at [Tutorial to Create Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/tutorial-create-instance).</span></span>
5. <span data-ttu-id="688ee-109">Ja rodas problēmas saistībā ar Azure AD domēna pakalpojumu izvietošanu, skatiet rakstu [AZURE ad Domain Services problēmu novēršana](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) , lai atrisinātu Biežākās kļūdas, kas palīdzēs paveikt darbu atkārtoti.</span><span class="sxs-lookup"><span data-stu-id="688ee-109">If you are having issues with Deploying Azure AD Domain Services, see [Troubleshoot Azure AD Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot) to resolve common errors to help you get things working again.</span></span> 

<span data-ttu-id="688ee-110">**Nevar atspējot AAD-DS**</span><span class="sxs-lookup"><span data-stu-id="688ee-110">**Unable to disable AAD-DS**</span></span>

<span data-ttu-id="688ee-111">AAD-DS nevar pauzēt.</span><span class="sxs-lookup"><span data-stu-id="688ee-111">AAD-DS is unable to be paused.</span></span> <span data-ttu-id="688ee-112">Ja vēlaties pārtraukt pārvaldītā domēna izmantošanu, tas ir jādzēš.</span><span class="sxs-lookup"><span data-stu-id="688ee-112">If you wish to stop using your managed domain, it must be deleted.</span></span>

<span data-ttu-id="688ee-113">Ja rodas problēmas, lai atrisinātu biežāk sastopamos kļūdu ziņojumus un saistītu problēmu novēršanas darbības, lai palīdzētu atkal sākt darbu, skatiet rakstu [Azure Active Directory domēna pakalpojumu problēmu novēršana](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span><span class="sxs-lookup"><span data-stu-id="688ee-113">If you run into issues, to resolve common error messages and for associated troubleshooting steps to help you get things running again, see [Troubleshoot Azure Active Directory Domain Services](https://docs.microsoft.com/azure/active-directory-domain-services/troubleshoot).</span></span>
