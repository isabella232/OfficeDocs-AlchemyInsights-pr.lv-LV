---
title: 2419 nevar iespējot auditēšanu
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
ms.openlocfilehash: 0566a8d002b1bd9e38f3184824193394e49d56494d347338f96cfcdfdb758f4c
ms.sourcegitcommit: b5f7da89a650d2915dc652449623c78be6247175
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/05/2021
ms.locfileid: "54007797"
---
# <a name="unable-to-enable-unified-auditing"></a>Nevar iespējot vienoto auditēšanu

Kad organizācijā mēģināt iespējot vienoto auditēšanu, var tikt parādīts šāds kļūdas ziņojums:

```
Request: /api/adminauditlogconfig/EnableUnifiedAuditLogIngestion Status code: 500 Exception message: {"Message":"The command you tried to run isn't currently allowed in your organization. To run this command, you first need to run the command: Enable-OrganizationCustomization."
```

Lai novērstu šo problēmu, veiciet tālāk norādītās darbības.

1. [Savienošana uz Exchange Online Powershell](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/connect-to-exchange-online-powershell).

2. Palaidiet šādu cmdlet:

   ```
   Enable-OrganizationCustomization
   ```

3. Uzgaidiet 60 minūtes, līdz iepriekšējais iestatījums stāsies spēkā.

4. Exchange Online PowerShell izpildiet šādu komandu:

   ```
   Set-AdminAuditLogConfig -UnifiedAuditLogIngestionEnabled $true
   ```

Papildinformāciju skatiet šādos rakstos:

- [Savienošana uz Exchange Online PowerShell, izmantojot daudzfaktors autentifikāciju](https://docs.microsoft.com/powershell/exchange/exchange-online/connect-to-exchange-online-powershell/mfa-connect-to-exchange-online-powershell)

-  [Audita žurnāla meklēšanas ieslēgšana vai izslēgšana](https://docs.microsoft.com/microsoft-365/compliance/turn-audit-log-search-on-or-off)
