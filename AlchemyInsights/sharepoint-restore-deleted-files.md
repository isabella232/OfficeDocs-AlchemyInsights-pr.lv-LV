---
title: Izdzēsta faila vai mapes atjaunošana
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: ba1573a5-9f44-482b-8082-6f648f169449
ms.openlocfilehash: fc560686ec5c6a3d42a97687fda80ae5001b5c60
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47797555"
---
# <a name="restore-a-deleted-file-or-folder"></a><span data-ttu-id="fa3dc-102">Izdzēsta faila vai mapes atjaunošana</span><span class="sxs-lookup"><span data-stu-id="fa3dc-102">Restore a deleted file or folder</span></span>

<span data-ttu-id="fa3dc-103">SharePoint Online saglabā visa satura dublējumus 14 papildu dienas pēc faktiskās dzēšanas.</span><span class="sxs-lookup"><span data-stu-id="fa3dc-103">SharePoint Online retains backups of all content for 14 additional days beyond actual deletion.</span></span> <span data-ttu-id="fa3dc-104">Ja saturu nevar atjaunot, izmantojot atkritni vai failu atjaunošanu, administrators var sazināties ar Microsoft atbalsta dienestu, lai pieprasītu atjaunošanu jebkurā brīdī 14 dienas logā.</span><span class="sxs-lookup"><span data-stu-id="fa3dc-104">If content cannot be restored via the Recycle Bin or Files Restore, an administrator can contact Microsoft Support to request a restore any time inside the 14 day window.</span></span> <span data-ttu-id="fa3dc-105">Atjaunošanas darbi no dublējumkopijām var tikt izpildīti tikai vietņu kolekcijām vai apakšvietnēm, nevis konkrētiem failiem, sarakstiem vai bibliotēkām.</span><span class="sxs-lookup"><span data-stu-id="fa3dc-105">Restorations from backups can only be completed for site collections or sub-sites, not for specific files, lists, or libraries.</span></span>

<span data-ttu-id="fa3dc-106">Dzēšot vienumu vai vietni no SharePoint, tas netiek uzreiz noņemts.</span><span class="sxs-lookup"><span data-stu-id="fa3dc-106">When you delete an item or site from Sharepoint, it isn't immediately removed.</span></span> <span data-ttu-id="fa3dc-107">Izdzēstie vienumi tiek ievietoti atkritnē noteiktā laika periodā.</span><span class="sxs-lookup"><span data-stu-id="fa3dc-107">Deleted items go into the recycle bin for a period of time.</span></span> <span data-ttu-id="fa3dc-108">Šajā laikā varat atjaunot vienumus, kurus izdzēsāt to sākotnējā atrašanās vietā.</span><span class="sxs-lookup"><span data-stu-id="fa3dc-108">During that time, you can restore the items you deleted to their original location.</span></span> <span data-ttu-id="fa3dc-109">Lai iegūtu papildinformāciju, lūdzu, apmeklējiet šo tālāk norādītās saites.</span><span class="sxs-lookup"><span data-stu-id="fa3dc-109">For more information, please visit the links below.</span></span>

<span data-ttu-id="fa3dc-110">[Atjaunojiet SharePoint vietnes atkritnē esošos vienumus](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span><span class="sxs-lookup"><span data-stu-id="fa3dc-110">[Restore items in the Recycle Bin of a SharePoint site](https://support.office.com/article/restore-deleted-items-from-the-site-collection-recycle-bin-5fa924ee-16d7-487b-9a0a-021b9062d14b).</span></span>

[<span data-ttu-id="fa3dc-111">Izdzēsto failu un mapju atjaunošana pakalpojumā OneDrive</span><span class="sxs-lookup"><span data-stu-id="fa3dc-111">Restore deleted files or folders in OneDrive</span></span>](https://support.office.com/article/Restore-deleted-files-or-folders-in-OneDrive-949ada80-0026-4db3-a953-c99083e6a84f)

[<span data-ttu-id="fa3dc-112">Izdzēstas vietņu kolekcijas atjaunošana (ieskaitot grupu, saziņu un citas vietnes)</span><span class="sxs-lookup"><span data-stu-id="fa3dc-112">Restore a deleted site collection (Including group, communication and other sites)</span></span>](https://docs.microsoft.com/sharepoint/restore-deleted-site-collection)

[<span data-ttu-id="fa3dc-113">Izdzēstas OneDrive vietnes atjaunošana</span><span class="sxs-lookup"><span data-stu-id="fa3dc-113">Restore a deleted OneDrive site</span></span>](https://docs.microsoft.com/onedrive/restore-deleted-onedrive)

<span data-ttu-id="fa3dc-114">Lielapjoma atkritnes darbībām administratori var apsvērt iespēju izmantot [SharePoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span><span class="sxs-lookup"><span data-stu-id="fa3dc-114">For bulk recycle bin actions, admins may consider using [Sharepoint Online PNP](https://docs.microsoft.com/powershell/sharepoint/sharepoint-pnp/sharepoint-pnp-cmdlets?view=sharepoint-ps).</span></span>

<span data-ttu-id="fa3dc-115">**Failu atjaunošanas līdzeklis**</span><span class="sxs-lookup"><span data-stu-id="fa3dc-115">**Files Restore feature**</span></span>

<span data-ttu-id="fa3dc-116">Ja daudzi jūsu OneDrive vai SharePoint faili tiek izdzēsti, pārrakstīti, bojāti vai inficēti ļaunprogrammatūras, varat atjaunot visu OneDrive vai SharePoint bibliotēku iepriekšējā reizē, izmantojot failu atjaunošanas līdzekli.</span><span class="sxs-lookup"><span data-stu-id="fa3dc-116">If lots of your OneDrive or SharePoint files get deleted, overwritten, corrupted, or infected by malware, you can restore your entire OneDrive or SharePoint library to a previous time using the files restore feature.</span></span>

[<span data-ttu-id="fa3dc-117">OneDrive bibliotēkas atjaunošana</span><span class="sxs-lookup"><span data-stu-id="fa3dc-117">Restore a OneDrive library</span></span>](https://support.office.com/article/restore-your-onedrive-fa231298-759d-41cf-bcd0-25ac53eb8a15)

[<span data-ttu-id="fa3dc-118">Dokumentu bibliotēkas atjaunošana</span><span class="sxs-lookup"><span data-stu-id="fa3dc-118">Restore a Document library</span></span>](https://support.office.com/article/restore-a-document-library-317791c3-8bd0-4dfd-8254-3ca90883d39a)

