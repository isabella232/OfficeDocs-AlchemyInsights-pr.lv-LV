---
title: 2609-saglabāšanas-vai-eDiscovery-Hold
ms.author: markjjo
author: markjjo
manager: lauraw
ms.date: ''
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2609"
- "9000048"
ms.openlocfilehash: 85c41995545efd8e1526d9f7dce4a23929f85be5
ms.sourcegitcommit: 24e8248b0f061a76af50bf566d7a13fc24d29d99
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 11/05/2019
ms.locfileid: "37994078"
---
# <a name="unable-to-delete-items-in-sharepoint-online-or-onedrive-for-business"></a><span data-ttu-id="6cc57-102">Nevar dzēst vienumus SharePoint Online vai OneDrive uzņēmumiem</span><span class="sxs-lookup"><span data-stu-id="6cc57-102">Unable to delete items in SharePoint Online or OneDrive for Business</span></span>

<span data-ttu-id="6cc57-103">Jums vai lietotājiem, iespējams, nevarēs dzēst vienumus SharePoint Online vai OneDrive uzņēmumiem, jo saglabāšanas politika, saglabāšanas etiķete vai eDiscovery aizturēšana tiek lietota SharePoint OneDrive vietnes vai noteiktu vienumu.</span><span class="sxs-lookup"><span data-stu-id="6cc57-103">You or your users may be unable to delete items in SharePoint Online or OneDrive for Business because a retention policy, retention label, or eDiscovery hold is applied to a SharePoint of OneDrive site or to a specific item.</span></span> <span data-ttu-id="6cc57-104">Tas nozīmē, ka nevar dzēst dokumentu, dokumenta versiju, mapi, dokumentu bibliotēku, sarakstu, programmu, vietni vai vietņu kolekciju.</span><span class="sxs-lookup"><span data-stu-id="6cc57-104">This includes being unable to delete a document, a document version, a folder, a document library, a list, an app, a site, or a site collection.</span></span> <span data-ttu-id="6cc57-105">Tālāk ir sniegti daži kļūdu ziņojumu piemēri, ko varat saņemt, mēģinot dzēst vienumu, kas tiek saglabāts:</span><span class="sxs-lookup"><span data-stu-id="6cc57-105">Here are some examples of the error messages you may received if you try to delete an item that is being retained:</span></span>

- <span data-ttu-id="6cc57-106">"Šo vietni nevar dzēst, jo tā ir iekļauta eDiscovery turēt vai saglabāšanas politika"</span><span class="sxs-lookup"><span data-stu-id="6cc57-106">"This site cannot be deleted because it is included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="6cc57-107">"Šī vietne ir iestatīta bloķēt dzēšanu atbilstības politika"</span><span class="sxs-lookup"><span data-stu-id="6cc57-107">"This site has a compliance policy set to block deletion"</span></span>
- <span data-ttu-id="6cc57-108">"Atbilstības politika pašlaik bloķē vietnes dzēšanu"</span><span class="sxs-lookup"><span data-stu-id="6cc57-108">"A compliance policy is currently blocking this site deletion"</span></span>
- <span data-ttu-id="6cc57-109">"Šo vietņu kolekciju nevar dzēst, jo tā satur vietnes, kas ir iekļautas eDiscovery turēt vai saglabāšanas politika"</span><span class="sxs-lookup"><span data-stu-id="6cc57-109">"This site collection can’t be deleted because it contains sites that are included in an eDiscovery hold or retention policy"</span></span>
- <span data-ttu-id="6cc57-110">"Jums ir dzēst visus vienumus šajā mapē pirms izdzēšat mapi"</span><span class="sxs-lookup"><span data-stu-id="6cc57-110">"You have to delete all the items in this folder before you delete the folder"</span></span>
- <span data-ttu-id="6cc57-111">"Šī vienuma versijas nevar dzēst, jo tas ir aizturēts vai saglabāšanas politika"</span><span class="sxs-lookup"><span data-stu-id="6cc57-111">"Versions of this item cannot be deleted because it is on hold or retention policy"</span></span>
- <span data-ttu-id="6cc57-112">"Vienumu nevar izdzēst, kamēr aizturēts"</span><span class="sxs-lookup"><span data-stu-id="6cc57-112">"Item cannot be deleted while on hold"</span></span>
- <span data-ttu-id="6cc57-113">"Etiķete, kas tiek lietots šo vienumu neļauj rediģēt vai dzēst"</span><span class="sxs-lookup"><span data-stu-id="6cc57-113">"The label that's applied to this item prevents it from being edited or deleted"</span></span>
- <span data-ttu-id="6cc57-114">Nevar dzēst sarakstu aizturēšanas vai saglabāšanas politikas laikā "</span><span class="sxs-lookup"><span data-stu-id="6cc57-114">"List cannot be deleted while on hold or retention policy"</span></span>
- <span data-ttu-id="6cc57-115">"Sarakstu nevar dzēst, ja tas ir bloķēts vai saglabāšanas politika attiecas uz to"</span><span class="sxs-lookup"><span data-stu-id="6cc57-115">"The list cannot be deleted if it is blocked or if a retention policy is applied to it"</span></span>

<span data-ttu-id="6cc57-116">Dzēst vienumus vienā no šiem scenārijiem, saglabāšanas politika, saglabāšanas etiķete vai eDiscovery aizturēšana ir jānoņem (vai vietne ir jāizslēdz no saglabāšanas politikas).</span><span class="sxs-lookup"><span data-stu-id="6cc57-116">To delete items in one of these scenarios, the retention policy, retention label, or eDiscovery hold has to be removed (or a site has to be excluded from a retention policy).</span></span> <span data-ttu-id="6cc57-117">Jums ir nepieciešams vai nu atspējot vai izslēgt attiecīgo turiet, kas izraisa šo problēmu.</span><span class="sxs-lookup"><span data-stu-id="6cc57-117">You need to either disable or exclude respective hold that's causing this issue.</span></span> <span data-ttu-id="6cc57-118">Pēc saglabāšanas politika vai aizturēšana ir noņemta, var ilgt līdz 24 stundām izmaiņas stātos spēkā.</span><span class="sxs-lookup"><span data-stu-id="6cc57-118">After a retention policy or hold is removed, it may take up to 24 hours for the change to take effect.</span></span> 

<span data-ttu-id="6cc57-119">Lai iegūtu informāciju par dažādiem saglabāšanas un aizturēšanas līdzekļiem, ko var lietot SharePoint vietnēs un OneDrive kontos, skatiet vienu no tālāk norādītajām tēmām.</span><span class="sxs-lookup"><span data-stu-id="6cc57-119">For information about about the different retention and hold features that can be applied to SharePoint sites and OneDrive accounts, see one of the following topics.</span></span>

- [<span data-ttu-id="6cc57-120">Saglabāšanas politikas pārskats</span><span class="sxs-lookup"><span data-stu-id="6cc57-120">Overview of retention policies</span></span>](https://docs.microsoft.com/microsoft-365/compliance/retention-policies)

- [<span data-ttu-id="6cc57-121">Saglabāšanas etiķešu pārskats</span><span class="sxs-lookup"><span data-stu-id="6cc57-121">Overview of retention labels</span></span>](https://docs.microsoft.com/microsoft-365/compliance/labels)

- [<span data-ttu-id="6cc57-122">Pārvaldīt aizturēšanu detalizētā e-datu atklāšanā</span><span class="sxs-lookup"><span data-stu-id="6cc57-122">Manage holds in Advanced eDiscovery</span></span>](https://docs.microsoft.com/microsoft-365/compliance/managing-holds)

- [<span data-ttu-id="6cc57-123">eDiscovery tur</span><span class="sxs-lookup"><span data-stu-id="6cc57-123">eDiscovery holds</span></span>](https://docs.microsoft.com/microsoft-365/compliance/ediscovery-cases#step-4-place-content-locations-on-hold)

- [<span data-ttu-id="6cc57-124">Mantotās vietnes slēgšanas un dzēšanas politikas</span><span class="sxs-lookup"><span data-stu-id="6cc57-124">Legacy site closure and deletion policies</span></span>](https://support.office.com/article/Use-policies-for-site-closure-and-deletion-A8280D82-27FD-48C5-9ADF-8A5431208BA5)
