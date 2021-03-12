---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: b7580f0e609d21bdc13fc07fda0bfd15bdb7a7ca
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50709077"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="fff47-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="fff47-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="fff47-103">Vai strādājat ar PowerShell vai skriptiem pakalpojumā SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="fff47-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="fff47-104">Papildinformāciju skatiet tālāk norādītajās saitēs.</span><span class="sxs-lookup"><span data-stu-id="fff47-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="fff47-105">Darba sākšana ar SharePoint Online pārvaldības čaulu</span><span class="sxs-lookup"><span data-stu-id="fff47-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="fff47-106">Savienojuma izveide ar SPO PowerShell ar daudzfaktoru autentifikāciju (MFA)</span><span class="sxs-lookup"><span data-stu-id="fff47-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="fff47-107">[SharePoint modelī un praksē (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) ir PowerShell komandu bibliotēka, kas ļauj veikt sarežģītas pārvaldības darbības spo.</span><span class="sxs-lookup"><span data-stu-id="fff47-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="fff47-108">Ja rodas problēmas saistībā ar SPO pārvaldības čaulu, pārliecinieties, vai esat atjauninājis jaunāko versiju un mēģināt [atkārtoti importēt moduli](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) , izmantojot *"Import-Module Microsoft. Online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="fff47-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/scripting/developer/module/importing-a-powershell-module?view=powershell-7.1) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="fff47-109">Ja mēģināt palaist klienta puses objektu modeļu skriptus, lokālajā datorā ir jāinstalē [SharePoint Online klienta komponentu SDK](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="fff47-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="fff47-110">Ja jums rodas problēmas, izpildot skriptus no PowerShell, iespējams, vēlēsities palaist PowerShell kā administrators un mainīt [izpildes politiku](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="fff47-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>