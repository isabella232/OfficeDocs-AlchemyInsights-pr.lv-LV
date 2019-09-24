---
title: SharePoint Online PowerShell
ms.author: v-todmc
author: todmccoy
manager: mnirkhe
ms.date: 9/18/19
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000266"
- "1867"
ms.openlocfilehash: 00ec337ce34da9d3c3fba0a71602c3078a556552
ms.sourcegitcommit: 6b102e079a7d30298105fd811a67efb707d6d5bf
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/23/2019
ms.locfileid: "37123005"
---
# <a name="sharepoint-online-powershell"></a><span data-ttu-id="2a46b-102">SharePoint Online PowerShell</span><span class="sxs-lookup"><span data-stu-id="2a46b-102">Sharepoint Online PowerShell</span></span>

<span data-ttu-id="2a46b-103">Vai strādājat ar PowerShell vai skriptiem programmā SharePoint Online?</span><span class="sxs-lookup"><span data-stu-id="2a46b-103">Working with PowerShell or Scripts within Sharepoint Online?</span></span> <span data-ttu-id="2a46b-104">Apmeklējiet saites zemāk, lai iegūtu vairāk informācijas.</span><span class="sxs-lookup"><span data-stu-id="2a46b-104">Visit the links below for more information.</span></span>
- [<span data-ttu-id="2a46b-105">Darba sākšana ar SharePoint Online pārvaldības čaulu</span><span class="sxs-lookup"><span data-stu-id="2a46b-105">Getting started with SharePoint Online Management Shell</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps)
- [<span data-ttu-id="2a46b-106">Izveidot savienojumu ar spo PowerShell daudzfaktoru autentifikācija (MFA)</span><span class="sxs-lookup"><span data-stu-id="2a46b-106">Connect to SPO PowerShell with multifactor authentication (MFA)</span></span>](https://docs.microsoft.com/powershell/sharepoint/sharepoint-online/connect-sharepoint-online?view=sharepoint-ps#to-connect-with-multifactor-authentication-mfa)
- <span data-ttu-id="2a46b-107">[SharePoint modeļos un praksē (PNP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) ir iekļauta PowerShell komandu bibliotēka, kas ļauj veikt sarežģītas pārvaldības darbības attiecībā uz spo.</span><span class="sxs-lookup"><span data-stu-id="2a46b-107">[SharePoint Patterns and Practices (PnP)](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps) contains a library of PowerShell commands that allows you to perform complex management actions towards SPO.</span></span>

> [!NOTE]
> - <span data-ttu-id="2a46b-108">Ja jums ir problēmas, kas savieno ar SPO pārvaldības čaulu, pārliecinieties, ka jums ir jāatjaunina uz jaunāko versiju un mēģiniet [atkārtoti importēt moduli](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) , izmantojot *"importa moduli Microsoft. Online. SharePoint. PowerShell".*</span><span class="sxs-lookup"><span data-stu-id="2a46b-108">If you are having issues connecting with the SPO management shell, make sure that you have updated to the latest version and try to [re-import the module](https://docs.microsoft.com/powershell/developer/module/importing-a-powershell-module) using *“Import-Module Microsoft.Online.SharePoint.PowerShell”.*</span></span>
> - <span data-ttu-id="2a46b-109">Ja mēģināt palaist klienta objekta modeļa skriptus, jums vajadzēs [SharePoint Online klienta komponenti SDK](https://www.microsoft.com/download/details.aspx?id=42038) instalēta lokālajā datorā.</span><span class="sxs-lookup"><span data-stu-id="2a46b-109">If you are attempting to run client-side object model scripts, you will need to have the [Sharepoint Online Client Components SDK](https://www.microsoft.com/download/details.aspx?id=42038) installed on your local machine.</span></span>
> - <span data-ttu-id="2a46b-110">Ja rodas problēmas, palaižot skriptus no PowerShell, iespējams, vēlēsities palaist PowerShell kā administrators un mainīt [izpildes politiku](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span><span class="sxs-lookup"><span data-stu-id="2a46b-110">If you are having issues running scripts from PowerShell, you may want to consider running PowerShell as an Administrator and changing the [Execution Policy](https://docs.microsoft.com/powershell/module/microsoft.powershell.core/about/about_execution_policies?view=powershell-6).</span></span>