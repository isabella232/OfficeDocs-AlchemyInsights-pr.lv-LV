---
title: 2419 — nevar iespējot auditēšana
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 23ad07a6dd943d61d1bd45453089a771cfd51b58
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44510435"
---
# <a name="unable-to-enable-unified-auditing"></a>Nevar iespējot vienotās auditēšanas

Mēģinot iespējot vienotās auditēšanas uzņēmuma, var tikt parādīts kļūdas līdzīgs šim:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Lai novērstu šo problēmu, rīkojieties šādi:

1. [Izveidot savienojumu ar Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Palaidiet šādu cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Uzgaidiet, līdz 60 minūtes, lai stātos spēkā iepriekšējais iestatījums.

4. Izpildiet šādu komandu Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Lai iegūtu papildinformāciju, skatiet šajos rakstos:

- [Izveidot savienojumu ar Exchange Online PowerShell, izmantojot vairāku faktoru autentifikācija](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Audita žurnāla meklēšanas ieslēgšana vai izslēgšana](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
