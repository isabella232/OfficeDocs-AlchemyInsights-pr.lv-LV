---
title: Mainīt stiprās paroles prasību
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: a054735a0c139c90d76098297bb9984d37464d3b
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43706568"
---
# <a name="change-strong-password-requirement"></a>Mainīt stiprās paroles prasību

Microsoft pēc noklusējuma pieprasa spēcīgas paroles. 

Izmantojot PowerShell, jūs varat atslēgt spēcīgas paroles konkrētiem lietotājiem ar šo komandu:<br>
*Set-MsolUser – UserPrincipalName <UserPrincipalName> – strongpasswordrequired $FALSE*

- [Plašāka informācija par paroļu politiku](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kā izveidot savienojumu ar Microsoft 365 ar PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Plašāka informācija par PowerShell MsolUser komandas](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)
