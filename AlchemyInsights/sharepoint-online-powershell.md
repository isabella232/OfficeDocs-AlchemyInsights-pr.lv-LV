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
ms.openlocfilehash: d90b60de72cf87a56e3b7f6a792708693f31af00
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47770846"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="6f89b-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="6f89b-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="6f89b-103">Vai strādājat ar PowerShell vai skriptiem pakalpojumā SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="6f89b-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="6f89b-104">Papildinformāciju skatiet tālāk norādītajās saitēs.</span><span class="sxs-lookup"><span data-stu-id="6f89b-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="6f89b-105">Darba sākšana ar SharePoint Online pārvaldības čaulu</span><span class="sxs-lookup"><span data-stu-id="6f89b-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="6f89b-106">Savienojuma izveide ar SPO PowerShell ar daudzfaktoru autentifikāciju (MFA)</span><span class="sxs-lookup"><span data-stu-id="6f89b-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="6f89b-107">[SharePoint modelī un praksē (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) ir PowerShell komandu bibliotēka, kas ļauj veikt sarežģītas pārvaldības darbības spo.</span><span class="sxs-lookup"><span data-stu-id="6f89b-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="6f89b-108">Ja rodas problēmas saistībā ar SPO pārvaldības čaulu, pārliecinieties, vai esat atjauninājis jaunāko versiju un mēģināt [atkārtoti importēt moduli](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) , izmantojot *"Import-Module Microsoft. Online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="6f89b-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="6f89b-109">Ja mēģināt palaist klienta puses objektu modeļu skriptus, lokālajā datorā ir jāinstalē [SharePoint Online klienta komponentu SDK](https://www.microsoft.com/download/details.aspx?id=42038) .</span><span class="sxs-lookup"><span data-stu-id="6f89b-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="6f89b-110">Ja jums rodas problēmas, izpildot skriptus no PowerShell, iespējams, vēlēsities palaist PowerShell kā administrators un mainīt [izpildes politiku](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="6f89b-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>