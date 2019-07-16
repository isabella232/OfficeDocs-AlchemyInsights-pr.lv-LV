---
title: Pārmaiņas stipras paroles prasība
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000105"
- "1600"
ms.openlocfilehash: 53affd2a347c004e7b21b353c2b3df98bc30a585
ms.sourcegitcommit: a7e5ca472000dfec471950bafd12eee8d7144f74
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2019
ms.locfileid: "35701590"
---
# <a name="change-strong-password-requirement"></a>Pārmaiņas stipras paroles prasība

Pēc noklusējuma nepieciešamas spēcīgas paroles. 

Izmantojot programmu PowerShell var atspējot stipras paroles atsevišķiem lietotājiem ar šo komandu:<br>
*Kopa MsolUser-UserPrincipalName <UserPrincipalName> -StrongPasswordRequired $false*

- [Plašāku informāciju par paroļu politika](https://docs.microsoft.com/azure/active-directory/authentication/concept-sspr-policy#password-policies-that-only-apply-to-cloud-user-accounts)
- [Kā pieslēgt ar PowerShell O365](https://docs.microsoft.com/office365/enterprise/powershell/connect-to-office-365-powershell#connect-with-the-microsoft-azure-active-directory-module-for-windows-powershell)
- [Informacijos apie PowerShell MsolUser komandas](https://docs.microsoft.com/powershell/module/msonline/set-msoluser?view=azureadps-1.0)