---
title: Nevar izdzēst vienumus pakalpojumā SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: db45aa8df40484fdcda7c430f1ca27482a1dd4ce
ms.sourcegitcommit: a9415f3ae8c7ba267b5134bcbdc1e070cea41a0f
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/12/2020
ms.locfileid: "49019590"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="00ca1-102">Nevar izdzēst vienumus</span><span class="sxs-lookup"><span data-stu-id="00ca1-102">Unable to delete items</span></span>

- <span data-ttu-id="00ca1-103">Saglabāšanas politikas var izraisīt šo problēmu, ir jāatspējo vai jāizslēdz attiecīgais aizturēšanas iemesls.</span><span class="sxs-lookup"><span data-stu-id="00ca1-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="00ca1-104">Kad saglabāšanas politika vai aizturēt ir noņemta, var paiet līdz pat 24 stundām, līdz izmaiņas stāsies spēkā.</span><span class="sxs-lookup"><span data-stu-id="00ca1-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="00ca1-105">Pārliecinieties, vai vienumā nav [saglabāšanas politikas](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) iestatījumu.</span><span class="sxs-lookup"><span data-stu-id="00ca1-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

- <span data-ttu-id="00ca1-106">Vietne, iespējams, ir pārsniedzis krātuves ierobežojumu, palielina [vietnes kvotu](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) un izdzēš vienumu.</span><span class="sxs-lookup"><span data-stu-id="00ca1-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

- <span data-ttu-id="00ca1-107">Pārliecinieties, vai vienums nav [paņemts](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) citam lietotājam.</span><span class="sxs-lookup"><span data-stu-id="00ca1-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

- <span data-ttu-id="00ca1-108">Visbeidzot administratori var izmantot [SharePoint modeļus un prakses](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP), kas satur PowerShell komandu bibliotēku, kas sniedz iespēju veikt sarežģītas pārvaldības darbības, piemēram, likt dzēst spītīgus vienumus.</span><span class="sxs-lookup"><span data-stu-id="00ca1-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="00ca1-109">PNP faila noņemšana</span><span class="sxs-lookup"><span data-stu-id="00ca1-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="00ca1-110">PNP mapes noņemšana</span><span class="sxs-lookup"><span data-stu-id="00ca1-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="00ca1-111">PNP saraksta vienuma noņemšana</span><span class="sxs-lookup"><span data-stu-id="00ca1-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="00ca1-112">PNP saraksta noņemšana</span><span class="sxs-lookup"><span data-stu-id="00ca1-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="00ca1-113">PNP lauka noņemšana (kolonna)</span><span class="sxs-lookup"><span data-stu-id="00ca1-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)