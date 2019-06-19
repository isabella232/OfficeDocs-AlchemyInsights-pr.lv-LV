---
title: 2419-nevar-uz-enable-auditēšana
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 3af01c03711eed646f0009afb5bea685bc358196
ms.sourcegitcommit: 87153fec6f6468b57893abf4aac073ba4068e67b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/19/2019
ms.locfileid: "35065669"
---
# <a name="unable-to-enable-unified-auditing"></a><span data-ttu-id="1cfb2-102">Nevar iespējot vienota auditēšanas</span><span class="sxs-lookup"><span data-stu-id="1cfb2-102">Unable to enable unified auditing</span></span>

<span data-ttu-id="1cfb2-103">Tad, kad jūs mēģināt iespējot vienotu revīzijas uzņēmuma biroja 365, varat saņemt kļūdas ziņojumu, līdzīgi šādu:</span><span class="sxs-lookup"><span data-stu-id="1cfb2-103">When you try to enable unified auditing for your Office 365 organization, you may receive an error similar the following:</span></span>

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

<span data-ttu-id="1cfb2-104">Lai atrisinātu šo problēmu, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="1cfb2-104">To resolve this issue, follow these steps:</span></span>

1. <span data-ttu-id="1cfb2-105">[Izveidot savienojumu ar tiešsaistes Powershell apmainīties](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span><span class="sxs-lookup"><span data-stu-id="1cfb2-105">[Connect to Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).</span></span>

2. <span data-ttu-id="1cfb2-106">Palaist šādu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="1cfb2-106">Run the following cmdlet:</span></span>

   ```
   Enable-OrganizationCustomization
   ```

3. <span data-ttu-id="1cfb2-107">Gaidīt uz 60 minūtēm iepriekšējo uzstādījums stātos spēkā.</span><span class="sxs-lookup"><span data-stu-id="1cfb2-107">Wait for 60 minutes for the previous setting to take effect.</span></span>

4. <span data-ttu-id="1cfb2-108">Online apmaiņa PowerShell, palaidiet šādu komandu:</span><span class="sxs-lookup"><span data-stu-id="1cfb2-108">Run the following command in Exchange Online PowerShell:</span></span>

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

<span data-ttu-id="1cfb2-109">Lai iegūtu papildinformāciju, skatiet šajos rakstos:</span><span class="sxs-lookup"><span data-stu-id="1cfb2-109">For additional information, see the following articles:</span></span>

- [<span data-ttu-id="1cfb2-110">Izveidot savienojumu ar Exchange Online PowerShell izmantojot vairāku faktoru autentifikaciju</span><span class="sxs-lookup"><span data-stu-id="1cfb2-110">Connect to Exchange Online PowerShell using multi-factor authentication</span></span>](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [<span data-ttu-id="1cfb2-111">Office 365 audita žurnālu meklēšanas ieslēgšana vai izslēgšana</span><span class="sxs-lookup"><span data-stu-id="1cfb2-111">Turn Office 365 audit log search on or off</span></span>](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
