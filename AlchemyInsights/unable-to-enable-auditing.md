---
title: 2419-nav iespējams iespējot-audits
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: 2419
ms.assetid: ''
ms.openlocfilehash: 81fd8e33feb2f2b10b04cc7cdc746a8603aa366b
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767606"
---
# <a name="unable-to-enable-unified-auditing"></a>Nevar iespējot unificēto auditēšanu

Kad mēģināt iespējot unificēto auditēšanu savai organizācijai, iespējams, parādās kļūdas ziņojums, kas līdzīgs šim:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Lai atrisinātu šo problēmu, veiciet tālāk norādītās darbības.

1. [Savienojuma izveide ar Exchange Online PowerShell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Palaidiet šādu cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Uzgaidiet, līdz 60 minūtes iepriekšējais iestatījums stājas spēkā.

4. Palaidiet tālāk norādīto komandu pakalpojumā Exchange Online PowerShell:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Papildinformāciju skatiet šajos rakstos:

- [Savienojuma izveide ar Exchange Online PowerShell, izmantojot daudzfaktoru autentifikāciju](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Audita žurnālu meklēšanas ieslēgšana vai izslēgšana](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
