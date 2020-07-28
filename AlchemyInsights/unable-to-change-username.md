---
title: Nevar mainīt lietotājvārdu
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/24/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "1729"
- "9000183"
ms.openlocfilehash: 34aecdf503699ee500179f0958158fc964d77fcb
ms.sourcegitcommit: b10cea11b4975354b91193327b58aa4740d34833
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/28/2020
ms.locfileid: "45439548"
---
# <a name="unable-to-change-username"></a>Nevar mainīt lietotājvārdu

Dažos gadījumos UPN (UserPrincipalName) izmaiņas netiek izplatītas mākonī. Validācijas kļūdas var tikt saņemtas Office 365 portālā vai nevar mainīt lietotājvārdu vai e-pasta adresi. Lai atrisinātu šo problēmu, manuāli iestatiet UserPrincipalName, izmantojot šo PowerShell komandu.

**Piemērs: lietotāja pārdēvēšana**

PowerShellCopy

PS C: \> Set-MsolUserPrincipalName-userPrincipalName "davidc@contoso.com"-NewUserPrincipalNameparametru izvēles "davidchew@contoso.com"

Šī komanda pārdēvē davidc@contoso.com ar davidchew@contoso.com.

Papildinformāciju skatiet rakstā [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).