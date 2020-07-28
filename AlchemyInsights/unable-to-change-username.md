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
# <a name="unable-to-change-username"></a><span data-ttu-id="d233b-102">Nevar mainīt lietotājvārdu</span><span class="sxs-lookup"><span data-stu-id="d233b-102">Unable to change UserName</span></span>

<span data-ttu-id="d233b-103">Dažos gadījumos UPN (UserPrincipalName) izmaiņas netiek izplatītas mākonī.</span><span class="sxs-lookup"><span data-stu-id="d233b-103">In some cases, UPN (UserPrincipalName) changes aren't propagated to the cloud.</span></span> <span data-ttu-id="d233b-104">Validācijas kļūdas var tikt saņemtas Office 365 portālā vai nevar mainīt lietotājvārdu vai e-pasta adresi.</span><span class="sxs-lookup"><span data-stu-id="d233b-104">You might receive validation errors in the Office 365 portal or be unable to change the username or email address.</span></span> <span data-ttu-id="d233b-105">Lai atrisinātu šo problēmu, manuāli iestatiet UserPrincipalName, izmantojot šo PowerShell komandu.</span><span class="sxs-lookup"><span data-stu-id="d233b-105">To resolve this issue, manually set UserPrincipalName using this PowerShell command.</span></span>

<span data-ttu-id="d233b-106">**Piemērs: lietotāja pārdēvēšana**</span><span class="sxs-lookup"><span data-stu-id="d233b-106">**Example: Rename a user**</span></span>

<span data-ttu-id="d233b-107">PowerShellCopy</span><span class="sxs-lookup"><span data-stu-id="d233b-107">PowerShellCopy</span></span>

<span data-ttu-id="d233b-108">PS C: \> Set-MsolUserPrincipalName-userPrincipalName "davidc@contoso.com"-NewUserPrincipalNameparametru izvēles "davidchew@contoso.com"</span><span class="sxs-lookup"><span data-stu-id="d233b-108">PS C:\> Set-MsolUserPrincipalName -UserPrincipalName "davidc@contoso.com" -NewUserPrincipalName "davidchew@contoso.com"</span></span>

<span data-ttu-id="d233b-109">Šī komanda pārdēvē davidc@contoso.com ar davidchew@contoso.com.</span><span class="sxs-lookup"><span data-stu-id="d233b-109">This command renames davidc@contoso.com to davidchew@contoso.com.</span></span>

<span data-ttu-id="d233b-110">Papildinformāciju skatiet rakstā [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span><span class="sxs-lookup"><span data-stu-id="d233b-110">For more information, see [Set-MsolUserPrincipalName](https://docs.microsoft.com/powershell/module/msonline/set-msoluserprincipalname?view=azureadps-1.0).</span></span>