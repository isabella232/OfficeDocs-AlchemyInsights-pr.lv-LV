---
title: Self-pakalpojumu iegāde PowerShell
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
- "3516"
ms.openlocfilehash: 5e47e08e3309b3d58908e10ee06021da00f230bb
ms.sourcegitcommit: cb9505f9eca032af3a4194c68d18c91789365690
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/16/2020
ms.locfileid: "42091729"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="29dca-102">Self-pakalpojumu iegāde PowerShell</span><span class="sxs-lookup"><span data-stu-id="29dca-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="29dca-103">Lai izmantotu MSCommerce PowerShell moduli, tas jāinstalē Windows 10 ierīcē ar TLS 1,2 (nepieciešams lokālā administratora atļaujas).</span><span class="sxs-lookup"><span data-stu-id="29dca-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="29dca-104">Importējiet un izveidojiet savienojumu ar MSCommerce moduli.</span><span class="sxs-lookup"><span data-stu-id="29dca-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="29dca-105">Kad tiek piedāvāts pieteikties, jums vajadzēs izmantot globālo vai norēķinu administratora lomas akreditācijas datus.</span><span class="sxs-lookup"><span data-stu-id="29dca-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="29dca-106">Ja jums nav TLS 1,2, var tikt parādīts šāds kļūdas ziņojums, mēģinot iegūt vai atjaunināt politiku:</span><span class="sxs-lookup"><span data-stu-id="29dca-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="29dca-107">*ErrorMessage — pamata savienojums tika aizvērts: sūtīšanas laikā radās neparedzēta kļūda*.</span><span class="sxs-lookup"><span data-stu-id="29dca-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



