---
title: Nevar iestatīt vai skatīt AllowSelfServicePurchase politiku
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 587a05cccbc71a970d4bd7723bff0df0c3b64ccc
ms.sourcegitcommit: 2a9d059262c07c33f9a740b3da4e6e3366b2f925
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/20/2020
ms.locfileid: "42158568"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="454fd-102">Nevar iestatīt vai skatīt AllowSelfServicePurchase politiku</span><span class="sxs-lookup"><span data-stu-id="454fd-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="454fd-103">Mēģinot iestatīt vai skatīt AllowSelfServicePurchase politiku, tiek parādīts šāds kļūdas ziņojums:</span><span class="sxs-lookup"><span data-stu-id="454fd-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="454fd-104">*HandleError: neizdevās izgūt produktu politika ar PolicyId "AllowSelfServicePurchase" ErrorMessage-pamata savienojums tika aizvērts: radās neparedzēta kļūda nosūtīt.*</span><span class="sxs-lookup"><span data-stu-id="454fd-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="454fd-105">Tas var būt saistīts ar vecākas versijas transporta slāņa drošība (TLS).</span><span class="sxs-lookup"><span data-stu-id="454fd-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="454fd-106">Lai savienotu MSCommerce pakalpojumu, ir jāizmanto TLS 1,2 vai jaunāka versija.</span><span class="sxs-lookup"><span data-stu-id="454fd-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="454fd-107">Izmēģiniet tālāk aprakstītās darbības, lai iespējotu/iestatītu TLS protokolu 1,2, pārbaudiet un mēģiniet vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="454fd-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="454fd-108">PowerShell komandu uzvednē (PS C:\) ievadiet šādu komandu, lai iestatītu TLS protokola versija 1,2:</span><span class="sxs-lookup"><span data-stu-id="454fd-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="454fd-109">Pārbaudiet, vai TLS protokolu (s) lietošanā, ar šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="454fd-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="454fd-110">Ja nepieciešams, vēlreiz mēģiniet iegūt vai atjaunināt komandas.</span><span class="sxs-lookup"><span data-stu-id="454fd-110">Retry the Get or Update commands as needed.</span></span>

