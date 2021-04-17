---
title: Nevar iestatīt vai skatīt politiku AllowSelfServicePurchase
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9001212"
- "3526"
ms.openlocfilehash: 8dac2bdc20905cf37fc30317d9b371bfd755f452
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51826098"
---
# <a name="unable-to-set-or-view-the-allowselfservicepurchase-policy"></a><span data-ttu-id="947bd-102">Nevar iestatīt vai skatīt politiku AllowSelfServicePurchase</span><span class="sxs-lookup"><span data-stu-id="947bd-102">Unable to set or view the AllowSelfServicePurchase policy</span></span>

<span data-ttu-id="947bd-103">Mēģinot iestatīt vai skatīt politiku AllowSelfServicePurchase, tiek rādīts šāds kļūdas ziņojums:</span><span class="sxs-lookup"><span data-stu-id="947bd-103">When attempting to set or view the AllowSelfServicePurchase policy, you receive the following error message:</span></span>

<span data-ttu-id="947bd-104">*HandleError: Neizdevās izgūt produkta politiku ar PolicyId 'AllowSelfServicePurchase', ErrorMessage — pamatā esošais savienojums tika aizvērts: sūtīšanas laikā radās neparedzēta kļūda.*</span><span class="sxs-lookup"><span data-stu-id="947bd-104">*HandleError : Failed to retrieve product policy with PolicyId 'AllowSelfServicePurchase', ErrorMessage - The underlying connection was closed: An unexpected error occurred on a send.*</span></span>

<span data-ttu-id="947bd-105">Iemesls var būt vecāka transporta slāņa drošības (TLS) versija.</span><span class="sxs-lookup"><span data-stu-id="947bd-105">This may be due to an older version of Transport Layer Security (TLS).</span></span> <span data-ttu-id="947bd-106">Lai izveidotu savienojumu ar MSCommerce pakalpojumu, ir jāizmanto TLS 1.2 vai jaunāka versija.</span><span class="sxs-lookup"><span data-stu-id="947bd-106">To connect the MSCommerce service, you need to use TLS 1.2 or greater.</span></span>  

<span data-ttu-id="947bd-107">Mēģiniet veikt tālāk norādītās darbības, lai iespējotu/iestatītu TLS protokolu uz 1.2, pārbaudītu un mēģinātu vēlreiz.</span><span class="sxs-lookup"><span data-stu-id="947bd-107">Try the following steps to enable/set the TLS protocol to 1.2, verify, and retry.</span></span>
 1. <span data-ttu-id="947bd-108">PowerShell komandu uzvednē (PS C: ievadiet šo komandu, lai \) iestatītu TLS protokolu uz versiju 1.2:</span><span class="sxs-lookup"><span data-stu-id="947bd-108">At the PowerShell command prompt (PS C:\) enter the following command to set the TLS protocol to version 1.2:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol = [Net.SecurityProtocolType]::Tls12`

2. <span data-ttu-id="947bd-109">Pārbaudiet lietotos TLS protokolus ar šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="947bd-109">Verify the TLS protocol(s) in use, with the following command:</span></span>

    `[Net.ServicePointManager]::SecurityProtocol` 

3. <span data-ttu-id="947bd-110">Mēģiniet vēlreiz iegūt vai atjaunināt komandas pēc nepieciešamības.</span><span class="sxs-lookup"><span data-stu-id="947bd-110">Retry the Get or Update commands as needed.</span></span>

