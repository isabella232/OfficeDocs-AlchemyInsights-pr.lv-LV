---
title: PowerShell pašapkalpošanās iegāde
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
- "3516"
ms.openlocfilehash: e6cc504ebef19cbe78f576d9b207fe2d951d0ef5
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47739977"
---
# <a name="self-service-purchase-of-powershell"></a><span data-ttu-id="58760-102">PowerShell pašapkalpošanās iegāde</span><span class="sxs-lookup"><span data-stu-id="58760-102">Self-service purchase of PowerShell</span></span>

<span data-ttu-id="58760-103">Lai izmantotu MSCommerce PowerShell moduli, tas ir jāinstalē Windows 10 ierīcē, izmantojot TLS 1,2 (lokālās administratora atļaujas).</span><span class="sxs-lookup"><span data-stu-id="58760-103">To use the MSCommerce PowerShell module, you need to install it on a Windows 10 device with TLS 1.2 (local administrator permissions required).</span></span>  <span data-ttu-id="58760-104">Importējiet un izveidojiet savienojumu ar MSCommerce moduli.</span><span class="sxs-lookup"><span data-stu-id="58760-104">Import and connect to the MSCommerce module.</span></span>  <span data-ttu-id="58760-105">Kad tiek prasīts pieteikties, jums ir jāizmanto globālie vai norēķinu administratora lomu akreditācijas dati.</span><span class="sxs-lookup"><span data-stu-id="58760-105">When prompted to log in, you will need to use Global or Billing Admin role credentials.</span></span>  

<span data-ttu-id="58760-106">Ja jums nav TLS 1,2, iespējams, tiek parādīts šāds kļūdas ziņojums, mēģinot iegūt vai atjaunināt politiku.</span><span class="sxs-lookup"><span data-stu-id="58760-106">If you don't have TLS 1.2, you may receive the following error when attempting to get or update the policy:</span></span>

<span data-ttu-id="58760-107">*ErrorMessage — pamatā esošais savienojums ir aizvērts: nosūtīšanas laikā radās neparedzēta kļūda*.</span><span class="sxs-lookup"><span data-stu-id="58760-107">*ErrorMessage -The underlying connection was closed: An unexpected error occurred on a send*.</span></span>



