---
title: MC210173 — SharePoint Designer jaunā pielāgoto veidlapu līdzekļa novecošana
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9002886"
- "5508"
- "9000127"
- "5507"
ms.openlocfilehash: 5be1ac4c8a4044adbc7d37c32ba7b3cb67c6cc25
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51831813"
---
# <a name="mc210173---sharepoint-designer-new-custom-form-feature-deprecation"></a><span data-ttu-id="d2e48-102">MC210173 — SharePoint Designer jaunā pielāgoto veidlapu līdzekļa novecošana</span><span class="sxs-lookup"><span data-stu-id="d2e48-102">MC210173 - SharePoint Designer new custom Form feature deprecation</span></span>

<span data-ttu-id="d2e48-103">Mēs atklājām problēmu, kas ietekmē SharePoint Designer [pielāgoto veidlapu izveides](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) funkcionalitāti pakalpojumā SharePoint Online.</span><span class="sxs-lookup"><span data-stu-id="d2e48-103">We’ve identified an issue affecting SharePoint Designer functionality for [creating custom Forms](https://support.microsoft.com/en-us/office/create-a-custom-list-form-using-sharepoint-designer-917d8fdb-ee00-4441-adb3-a94612d1d105?ui=en-us&rs=en-us&ad=us#bm2) within SharePoint Online.</span></span> <span data-ttu-id="d2e48-104">Pēc rūpīgas pārbaudes, mēs nonācām pie secinājuma, ka šai problēmai nav zināma labojuma, un tāpēc mēs nolēmām atspējot pielāgoto veidlapu izveides līdzekli sākot ar 2020. gada 25. aprīli plkst. 03.00 UTC laika joslā.</span><span class="sxs-lookup"><span data-stu-id="d2e48-104">After careful examination, we’ve determined that there is no known fix for this issue and have elected to disable the custom Form creation feature effective as of 3:00 AM UTC on Saturday, April 25, 2020.</span></span> <span data-ttu-id="d2e48-105">Šīs izmaiņas neietekmēs iespēju rediģēt iepriekš izveidotās veidlapas vai citus SharePoint Online noformētāja esošos līdzekļus.</span><span class="sxs-lookup"><span data-stu-id="d2e48-105">This change does not impact the ability to edit previously created Forms or other existing features in SharePoint Online Designer.</span></span>

<span data-ttu-id="d2e48-106">Pēc šo izmaiņu veikšanas, lietotājiem jaunu veidlapu izveides laikā var tikt parādīts kļūdas paziņojums: “Neizdevās saglabāt saraksta izmaiņas serverī”.</span><span class="sxs-lookup"><span data-stu-id="d2e48-106">After this change was made, users may have received the error: "Could not save the list changes to the server," when creating new Forms.</span></span>

<span data-ttu-id="d2e48-107">Lietotāji, kas iepriekš izmantoja SharePoint Designer, lai veidotu pielāgotas veidlapas, tagad šim mērķim var izmantot [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form).</span><span class="sxs-lookup"><span data-stu-id="d2e48-107">Users who have previously leveraged SharePoint Designer to create custom Forms are instead able to utilize [PowerApps](https://docs.microsoft.com/powerapps/maker/canvas-apps/customize-list-form) for this purpose.</span></span>

<span data-ttu-id="d2e48-108">PowerApps ir vienkāršs, bet spēcīgs rīks, kas ļauj lietotājiem izmantot SharePoint Online Modern, lai pārlūkprogrammas logā veidotu vai rediģētu pielāgotās veidlapas SharePoint sarakstiem un dokumentu bibliotēkām.</span><span class="sxs-lookup"><span data-stu-id="d2e48-108">PowerApps is an easy and powerful tool that allows users operating in the SharePoint Online Modern experience to create and edit custom Forms for SharePoint lists and document libraries right from a browser window.</span></span> <span data-ttu-id="d2e48-109">PowerApps nav nepieciešamas papildu kodēšanas zināšanas vai papildu lietojumprogrammu lejupielāde, piemēram, InfoPath.</span><span class="sxs-lookup"><span data-stu-id="d2e48-109">PowerApps does not require traditional coding knowledge or any additional app downloads such as InfoPath.</span></span>

<span data-ttu-id="d2e48-110">**Piezīme**: SharePoint Online Classic versijas lietotājiem būs īslaicīgi jāpāriet uz Modern versiju, lai piekļūtu un izmantotu PowerApps. Visas PowerApps izveidotās pielāgotās veidlapas ir pieejamas arī SharePoint Online Classic versijas lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="d2e48-110">**Note**: SharePoint Online Classic users will need to temporarily switch to the Modern experience to access and utilize PowerApps; though, all custom Forms created in PowerApps are accessible by SharePoint Online Classic experience users.</span></span>
