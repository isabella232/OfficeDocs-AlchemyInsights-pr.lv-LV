---
title: PowerShell patstāvīgi iegādāts pirkums
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
- "3516"
ms.openlocfilehash: 48b5b0a1be1bc03d45a531a1093f18a3f750c37d
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51797728"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="98b23-102">PowerShell patstāvīgi iegādāts pirkums</span><span class="sxs-lookup"><span data-stu-id="98b23-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="98b23-103">Lai izmantotu MSCommerce PowerShell moduli, tas ir jāinstalē Windows 10 ierīcē ar TLS 1.2 (nepieciešamas lokālā administratora atļaujas).</span><span class="sxs-lookup"><span data-stu-id="98b23-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="98b23-104">Importējiet un izveidojiet savienojumu ar MSCommerce moduli.</span><span class="sxs-lookup"><span data-stu-id="98b23-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="98b23-105">Pēc pieteikšanās ir jāizmanto globālās vai norēķinu administratora lomas akreditācijas dati.</span><span class="sxs-lookup"><span data-stu-id="98b23-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="98b23-106">Ja jums nav TLS 1.2, iespējams, mēģinot iegūt vai atjaunināt politiku, var tikt parādīts šāds kļūdas ziņojums:</span><span class="sxs-lookup"><span data-stu-id="98b23-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="98b23-107">*ErrorMessage — pamatā esošais savienojums tika aizvērts:* sūtīšanas laikā radās neparedzēta kļūda.</span><span class="sxs-lookup"><span data-stu-id="98b23-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



