---
title: Nevar izdzēst vienumus SharePoint vai OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: ''
ms.openlocfilehash: 21d7b928fade48a6729c120e6ea33b16dafe799e
ms.sourcegitcommit: 22ce2315c8cf643137ab3420cdc1cda41433d44a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 05/14/2019
ms.locfileid: "34057740"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="2e305-102">Nevar izdzēst vienumus</span><span class="sxs-lookup"><span data-stu-id="2e305-102">Unable to delete items</span></span>

<span data-ttu-id="2e305-103">Problēmas, dzēšot vienumus?</span><span class="sxs-lookup"><span data-stu-id="2e305-103">Having issues deleting items?</span></span>

- <span data-ttu-id="2e305-104">Vienmēr pārliecinieties, vai jums ir [atbilstošas atļaujas](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) dzēst vienumu vai [vietņu kolekcijas administrators](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) mēģinājums noņemt vienumu.</span><span class="sxs-lookup"><span data-stu-id="2e305-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/en-us/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/en-us/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="2e305-105">Nodrošina to, ka nenotiek [saglabāšanas politiku](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) iestatīšana krājumam.</span><span class="sxs-lookup"><span data-stu-id="2e305-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/en-us/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="2e305-106">Nodrošinātu, ka prece nav [paņēmis](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) cits lietotājs.</span><span class="sxs-lookup"><span data-stu-id="2e305-106">Ensure the item is not [checked out](https://support.office.com/en-us/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="2e305-107">Visbeidzot, administratori var izmantot [SharePoint modeļus un praksi](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kas atrodas bibliotēka PowerShell komandu, kas ļauj jums veikt sarežģītas vadības rīcība, piemēram, piespiest spītīgs vienumu dzēšana.</span><span class="sxs-lookup"><span data-stu-id="2e305-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span> 
- [<span data-ttu-id="2e305-108">Noņemt failu PNP</span><span class="sxs-lookup"><span data-stu-id="2e305-108">Remove PNP File</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="2e305-109">Noņemt mapi PNP</span><span class="sxs-lookup"><span data-stu-id="2e305-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="2e305-110">PNP saraksta vienuma noņemšana</span><span class="sxs-lookup"><span data-stu-id="2e305-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="2e305-111">Noņemt PNP sarakstu</span><span class="sxs-lookup"><span data-stu-id="2e305-111">Remove PNP List</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="2e305-112">Noņemt PNP laukā (kolonnā)</span><span class="sxs-lookup"><span data-stu-id="2e305-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/en-us/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)