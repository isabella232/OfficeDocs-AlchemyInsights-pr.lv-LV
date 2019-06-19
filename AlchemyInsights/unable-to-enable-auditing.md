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
# <a name="unable-to-enable-unified-auditing"></a>Nevar iespējot vienota auditēšanas

Tad, kad jūs mēģināt iespējot vienotu revīzijas uzņēmuma biroja 365, varat saņemt kļūdas ziņojumu, līdzīgi šādu:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Lai atrisinātu šo problēmu, rīkojieties šādi:

1. [Izveidot savienojumu ar tiešsaistes Powershell apmainīties](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Palaist šādu cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Gaidīt uz 60 minūtēm iepriekšējo uzstādījums stātos spēkā.

4. Online apmaiņa PowerShell, palaidiet šādu komandu:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Lai iegūtu papildinformāciju, skatiet šajos rakstos:

- [Izveidot savienojumu ar Exchange Online PowerShell izmantojot vairāku faktoru autentifikaciju](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Office 365 audita žurnālu meklēšanas ieslēgšana vai izslēgšana](https://docs.microsoft.com/office365/securitycompliance/turn-audit-log-search-on-or-off)
