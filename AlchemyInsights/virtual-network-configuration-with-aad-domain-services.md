---
title: Virtuālā konfigurācija ar AAD Domain Services
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 01/15/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "7927"
- "9004397"
ms.openlocfilehash: 7c56e467679f9b9a48cfd7a6f70f7ee148ded3e8
ms.sourcegitcommit: a61a29dbd0382370fea0be5fa4a61c9a1a9354c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/18/2021
ms.locfileid: "49885655"
---
# <a name="virtual-configuration-with-aad-domain-services"></a><span data-ttu-id="b8693-102">Virtuālā konfigurācija ar AAD Domain Services</span><span class="sxs-lookup"><span data-stu-id="b8693-102">Virtual configuration with AAD domain services</span></span>

<span data-ttu-id="b8693-103">Virtuālā konfigurācija ar AAD Domain Services ietver tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="b8693-103">Virtual configuration with AAD domain services involves the following steps:</span></span> 

1. <span data-ttu-id="b8693-104">Domēna darbspējas pārbaude Azure portālā https://aka.ms/aadds-health</span><span class="sxs-lookup"><span data-stu-id="b8693-104">Checking your domain’s health on the Azure portal https://aka.ms/aadds-health</span></span>
2. <span data-ttu-id="b8693-105">NSG pārbaude, vai nav tādu kārtulu, kas bloķē portus, kas nepieciešami, lai sinhronizētu Azure AD domēna pakalpojumos portālā https://aka.ms/aadds-networking</span><span class="sxs-lookup"><span data-stu-id="b8693-105">Checking your NSG for rules that block ports needed to synchronize in Azure AD Domain Services on the portal https://aka.ms/aadds-networking</span></span>
3. <span data-ttu-id="b8693-106">Pārliecinieties, vai jūsu virtuālais tīkls ir izvietots vienā Azure reģionā kā Azure AD Domain Services pārvaldītais domēns.</span><span class="sxs-lookup"><span data-stu-id="b8693-106">Ensuring that your virtual network is deployed in the same Azure Region as your Azure AD Domain Services-managed domain.</span></span>
4. <span data-ttu-id="b8693-107">Nodrošināt, ka jums nav tāda domēna, kuram ir tāds pats domēna nosaukums, kas pieejams virtuālajā tīklā.</span><span class="sxs-lookup"><span data-stu-id="b8693-107">Ensuring you don’t have an existent domain with the same domain name available on the virtual network.</span></span>

<span data-ttu-id="b8693-108">Lai iegūtu detalizētu informāciju par noformējuma atmaksu Azure virtuālajā tīklā, kas atbalsta AAD domēna pakalpojumus, skatiet rakstu [virtuālā tīkla uzmanība](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span><span class="sxs-lookup"><span data-stu-id="b8693-108">For more details on design consideration on Azure Virtual Network to support AAD domain services, see [Virtual Network Consideration](https://docs.microsoft.com/azure/active-directory-domain-services/network-considerations).</span></span>

