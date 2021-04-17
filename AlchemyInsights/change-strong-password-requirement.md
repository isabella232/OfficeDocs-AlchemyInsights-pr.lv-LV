---
title: Stipras paroles maiņas prasības
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
- "9000105"
- "1600"
ms.openlocfilehash: cf5cab9a1c2dd4226997d93417dc7104347f8a6e
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51818475"
---
# <a name="change-strong-password-requirement"></a>Stipras paroles prasību maiņa

Korporācijai Microsoft pēc noklusējuma ir nepieciešamas stipras paroles.

Izmantojot PowerShell, varat atspējot stipras paroles konkrētiem lietotājiem ar šīm komandām:

`Set-MsolUser –UserPrincipalName <UserPrincipalName> –StrongPasswordRequired  $false`

Lai visiem lietotājiem atspējotu spēcīgas paroles, izmantojiet:

`Get-MsolUser | Set-MsolUser -StrongPasswordRequired $false`

- [Papildinformācija par paroļu politiku](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kā izveidot savienojumu ar Microsoft 365, izmantojot PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Papildinformācija par PowerShell MsolUser komandām](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
