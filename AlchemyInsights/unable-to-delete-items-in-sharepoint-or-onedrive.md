---
title: Nevar dzēst vienumus SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1851"
- "2377"
- "9000255"
ms.assetid: ''
ms.openlocfilehash: 8647b65c52a782ca48ca58bb2700556db528796b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511983"
---
# <a name="unable-to-delete-items"></a><span data-ttu-id="a705b-102">Nevar izdzēst objektus</span><span class="sxs-lookup"><span data-stu-id="a705b-102">Unable to delete items</span></span>

<span data-ttu-id="a705b-103">Saglabāšanas politikas var izraisīt šo, jums ir atspējota vai izslēgt attiecīgo aizturēšanu, kas izraisa šo problēmu.</span><span class="sxs-lookup"><span data-stu-id="a705b-103">Retention policies can cause this, you need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="a705b-104">Pēc saglabāšanas politika vai aizturēšana ir noņemta, var ilgt līdz 24 stundām izmaiņas stātos spēkā.</span><span class="sxs-lookup"><span data-stu-id="a705b-104">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> <span data-ttu-id="a705b-105">Pārliecinieties, vai krājumam nav [saglabāšanas politikas](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) iestatījuma.</span><span class="sxs-lookup"><span data-stu-id="a705b-105">Ensure that there is not a [retention policy](https://docs.microsoft.com/microsoft-365/compliance/retention-policies) setup on the item.</span></span>

<span data-ttu-id="a705b-106">Iespējams, ka vietne ir pārsniegusi krātuves ierobežojumu, palielina [vietnes kvotu](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) un dzēš vienumu.</span><span class="sxs-lookup"><span data-stu-id="a705b-106">The site might have exceeded storage limit, increase the [site quota](https://docs.microsoft.com/powershell/module/sharepoint-online/set-sposite?view=sharepoint-ps) and delete the item.</span></span>

<span data-ttu-id="a705b-107">Pārliecinieties, vai vienums nav [paņemts](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) citam lietotājam.</span><span class="sxs-lookup"><span data-stu-id="a705b-107">Ensure the item is not [checked out](https://support.office.com/article/check-out-check-in-or-discard-changes-to-files-in-a-library-7e2c12a9-a874-4393-9511-1378a700f6de) to another user.</span></span>

<span data-ttu-id="a705b-108">Visbeidzot, administratori var izmantot [SharePoint modeļus un praksi](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PNP), kurā ir PowerShell komandu bibliotēka, kas ļauj veikt sarežģītas pārvaldības darbības, piemēram, Force dzēšot spītīgs vienumus.</span><span class="sxs-lookup"><span data-stu-id="a705b-108">Finally, administrators can use [SharePoint Patterns and Practices](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps#installation) (PnP) which contains a library of PowerShell commands that allow you to perform complex management actions such as force deleting stubborn items.</span></span>
- [<span data-ttu-id="a705b-109">PNP faila noņemšana</span><span class="sxs-lookup"><span data-stu-id="a705b-109">Remove PNP File</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfile?view=sharepoint-ps)
- [<span data-ttu-id="a705b-110">Noņemt PNP mapi</span><span class="sxs-lookup"><span data-stu-id="a705b-110">Remove PNP Folder</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfolder?view=sharepoint-ps)
- [<span data-ttu-id="a705b-111">Noņemt PNP saraksta vienumu</span><span class="sxs-lookup"><span data-stu-id="a705b-111">Remove PNP List Item</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplistitem?view=sharepoint-ps)
- [<span data-ttu-id="a705b-112">Noņemt PNP sarakstu</span><span class="sxs-lookup"><span data-stu-id="a705b-112">Remove PNP List</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnplist?view=sharepoint-ps)
- [<span data-ttu-id="a705b-113">Noņemt PNP lauku (kolonna)</span><span class="sxs-lookup"><span data-stu-id="a705b-113">Remove PNP Field (Column)</span></span>](https://docs.microsoft.com/powershell/module/sharepoint-pnp/remove-pnpfield?view=sharepoint-ps)