---
title: Atjaunot izdzēstu failu vai mapi
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: d5250d75a982c0afc9d3e1b2a43be2ba9c3e8f59
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/04/2019
ms.locfileid: "34716513"
---
## <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="ded44-102">Atjaunot izdzēstu failu vai mapi</span><span class="sxs-lookup"><span data-stu-id="ded44-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="ded44-103">SharePoint Online backups visu saturu saglabā 14 papildu dienas pēc faktiskā dzēšanu.</span><span class="sxs-lookup"><span data-stu-id="ded44-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="ded44-104">Ja satura nevar atjaunot, izmantojot atkritni vai atjaunot failus, administrators var sazināties ar Microsoft Support pieprasīt atjaunot jebkurā laikā 14 dienu loga iekšpusē.</span><span class="sxs-lookup"><span data-stu-id="ded44-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="ded44-105">Restaurācija no backups var pabeigt tikai vietņu kolekcijas vai apakšvietnes, nevis par konkrētiem failiem, sarakstiem vai bibliotēkām.</span><span class="sxs-lookup"><span data-stu-id="ded44-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="ded44-106">Dzēšot vienumu vai vietnes Sharepoint, uzreiz netiek noņemta.</span><span class="sxs-lookup"><span data-stu-id="ded44-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="ded44-107">Izdzēstie vienumi atkritnē iedziļināties laika periodu.</span><span class="sxs-lookup"><span data-stu-id="ded44-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="ded44-108">Šajā laikā jūs Izdzēstie vienumi var atjaunot to sākotnējā atrašanās vietā.</span><span class="sxs-lookup"><span data-stu-id="ded44-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="ded44-109">Lai iegūtu vairāk informācijas, lūdzu apmeklējiet šīs saites.</span><span class="sxs-lookup"><span data-stu-id="ded44-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="ded44-110">[Vienumu atjaunošana atkritnē no SharePoint vietnes](https://support.office.com/en-us/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span><span class="sxs-lookup"><span data-stu-id="ded44-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/en-us/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b?ui=en-US&amp;rs=en-US&amp;ad=US).</span></span>

[<span data-ttu-id="ded44-111">Atjaunot dzēstos failus vai mapes, kas OneDrive</span><span class="sxs-lookup"><span data-stu-id="ded44-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/en-us/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="ded44-112">Atjaunot dzēstos vietņu kolekcijas (ieskaitot grupa, komunikācijas un citās vietās)</span><span class="sxs-lookup"><span data-stu-id="ded44-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="ded44-113">Atjaunot dzēstos OneDrive vietni</span><span class="sxs-lookup"><span data-stu-id="ded44-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/en-us/onedrive/restore-deleted-onedrive)

<span data-ttu-id="ded44-114">Beztaras pārstrādā bin darbībām admins var izskatīt, izmantojot [Sharepoint Online PNP](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="ded44-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/en-us/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

## <a name="files-restore-feature"></a><span data-ttu-id="ded44-115">Failu atjaunošanas līdzekli</span><span class="sxs-lookup"><span data-stu-id="ded44-115">Files Restore feature</span></span>

<span data-ttu-id="ded44-116">Ja partijām OneDrive vai Sharepoint faili saņemt dzēsts, pārrakstīts, bojāti vai inficēts ar ļaunprātīgu programmatūru, var atjaunot iepriekšējā laikā, izmantojot failu atjaunošanas līdzekli visu OneDrive vai Sharepoint bibliotēku.</span><span class="sxs-lookup"><span data-stu-id="ded44-116">If lots of your OneDrive or Sharepoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or Sharepoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="ded44-117">Atjaunot OneDrive bibliotēka</span><span class="sxs-lookup"><span data-stu-id="ded44-117">Restore a OneDrive library</span></span>](https://support.office.com/en-us/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="ded44-118">Atjaunot dokumentu bibliotēkā</span><span class="sxs-lookup"><span data-stu-id="ded44-118">Restore a Document library</span></span>](https://support.office.com/en-us/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a?ui=en-US&amp;rs=en-US&amp;ad=US.)

