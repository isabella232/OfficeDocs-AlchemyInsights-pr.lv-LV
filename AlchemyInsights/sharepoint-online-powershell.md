---
title: SharePoint Online PowerShell
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 300c07e7f0010eae2bd4fe893ece9d09aab93ba5
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/17/2020
ms.locfileid: "46786896"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="80fbb-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="80fbb-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="80fbb-103">Vai strādājat ar PowerShell vai skriptiem pakalpojumā SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="80fbb-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="80fbb-104">Papildinformāciju skatiet tālāk norādītajās saitēs.</span><span class="sxs-lookup"><span data-stu-id="80fbb-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="80fbb-105">Darba sākšana ar SharePoint Online pārvaldības čaulu</span><span class="sxs-lookup"><span data-stu-id="80fbb-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="80fbb-106">Savienojuma izveide ar SPO PowerShell ar daudzfaktoru autentifikāciju (MFA)</span><span class="sxs-lookup"><span data-stu-id="80fbb-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="80fbb-107">[SharePoint modelī un praksē (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) ir PowerShell komandu bibliotēka, kas ļauj veikt sarežģītas pārvaldības darbības spo.</span><span class="sxs-lookup"><span data-stu-id="80fbb-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="80fbb-108">Ja rodas problēmas saistībā ar SPO pārvaldības čaulu, pārliecinieties, vai esat atjauninājis jaunāko versiju un mēģināt [atkārtoti importēt moduli](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) , izmantojot *"Import-Module Microsoft. Online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="80fbb-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="80fbb-109">Ja mēģināt palaist klienta puses objektu modeļu skriptus, lokālajā datorā ir jāinstalē [SharePoint Online klienta komponentu SDK](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="80fbb-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="80fbb-110">Ja jums rodas problēmas, izpildot skriptus no PowerShell, iespējams, vēlēsities palaist PowerShell kā administrators un mainīt [izpildes politiku](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="80fbb-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>