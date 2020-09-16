---
title: Nevar iestatīt vai skatīt AllowSelfServicePurchase politiku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 5ec16b3071f95ef52af2771e95137116222a3c5b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47735206"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="3ceb4-102">Nevar iestatīt vai skatīt AllowSelfServicePurchase politiku</span><span class="sxs-lookup"><span data-stu-id="3ceb4-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="3ceb4-103">Mēģinot iestatīt vai skatīt AllowSelfServicePurchase politiku, tiek parādīts šāds kļūdas ziņojums:</span><span class="sxs-lookup"><span data-stu-id="3ceb4-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="3ceb4-104">*HandleError: neizdevās izgūt produkta politiku ar PolicyId ' AllowSelfServicePurchase ', ErrorMessage-galvenais savienojums ir aizvērts: sūtot radās neparedzēta kļūda.*</span><span class="sxs-lookup"><span data-stu-id="3ceb4-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="3ceb4-105">Iespējams, tas skaidrojams ar vecāku transporta slāņa drošības (TLS) versiju.</span><span class="sxs-lookup"><span data-stu-id="3ceb4-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="3ceb4-106">Lai izveidotu savienojumu ar MSCommerce pakalpojumu, ir jāizmanto TLS 1,2 vai jaunāka versija.</span><span class="sxs-lookup"><span data-stu-id="3ceb4-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="3ceb4-107">Izmēģiniet tālāk norādītās darbības, lai iespējotu/iestatītu TLS protokolu 1,2, pārbaudiet un mēģiniet vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="3ceb4-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="3ceb4-108">PowerShell komandu uzvedne (PS C: ievadiet šo \) komandu, lai IESTATĪTU TLS protokolu versijai 1,2:</span><span class="sxs-lookup"><span data-stu-id="3ceb4-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="3ceb4-109">Pārbaudiet lietotos TLS protokolus ar šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="3ceb4-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="3ceb4-110">Pēc nepieciešamības atkārtoti mēģiniet iegūt vai atjaunināt komandas.</span><span class="sxs-lookup"><span data-stu-id="3ceb4-110">Retry the Get or Update commands as needed.</span></span>

