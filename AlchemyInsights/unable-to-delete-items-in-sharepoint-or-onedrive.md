---
title: Nevar izdzēst vienumus SharePoint vai OneDrive
ms.author: kirks
author: Techwriter40
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: d25214f26a3168e3e350b5cc31ca870e65d48ad9
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35366540"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="a4812-102">Nevar izdzēst vienumus</span><span class="sxs-lookup"><span data-stu-id="a4812-102">Unable to delete items</span></span>

<span data-ttu-id="a4812-103">Problēmas, dzēšot vienumus?</span><span class="sxs-lookup"><span data-stu-id="a4812-103">Having issues deleting items?</span></span>

- <span data-ttu-id="a4812-104">Vienmēr pārliecinieties, vai jums ir [atbilstošas atļaujas](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) dzēst vienumu vai [vietņu kolekcijas administrators](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) mēģinājums noņemt vienumu.</span><span class="sxs-lookup"><span data-stu-id="a4812-104">Always make sure you have the [appropriate permissions](https://docs.microsoft.com/sharepoint/default-sharepoint-groups) to delete the item or have a [site collection administrator](https://docs.microsoft.com/sharepoint/customize-sharepoint-site-permissions#add-change-or-remove-a-site-collection-administrator) attempt remove the item.</span></span>

- <span data-ttu-id="a4812-105">Nodrošina to, ka nenotiek [saglabāšanas politiku](https://docs.microsoft.com/office365/securitycompliance/retention-policies) iestatīšana krājumam.</span><span class="sxs-lookup"><span data-stu-id="a4812-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/office365/securitycompliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="a4812-106">Nodrošinātu, ka prece nav [paņēmis](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) cits lietotājs.</span><span class="sxs-lookup"><span data-stu-id="a4812-106">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="a4812-107">Visbeidzot, administratori var izmantot [SharePoint modeļus un praksi](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) kas atrodas bibliotēka PowerShell komandu, kas ļauj jums veikt sarežģītas vadības rīcība, piemēram, piespiest spītīgs vienumu dzēšana.</span><span class="sxs-lookup"><span data-stu-id="a4812-107">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="a4812-108">Noņemt failu PNP</span><span class="sxs-lookup"><span data-stu-id="a4812-108">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="a4812-109">Noņemt mapi PNP</span><span class="sxs-lookup"><span data-stu-id="a4812-109">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="a4812-110">PNP saraksta vienuma noņemšana</span><span class="sxs-lookup"><span data-stu-id="a4812-110">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="a4812-111">Noņemt PNP sarakstu</span><span class="sxs-lookup"><span data-stu-id="a4812-111">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="a4812-112">Noņemt PNP laukā (kolonnā)</span><span class="sxs-lookup"><span data-stu-id="a4812-112">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)