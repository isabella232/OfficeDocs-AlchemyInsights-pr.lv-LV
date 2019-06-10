---
title: SharePoint failu sinhronizēšana, izmantojot jauno OneDrive sinhronizācijas klientu
ms.author: kirks
author: Techwriter40
manager: pamgreen
ms.date: 5/17/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom: ''
ms.assetid: 5ad2f1f2-9650-4eb0-b4fa-2f52a09f535a
ms.openlocfilehash: 74b79efeb7e46d03dc55f46252d152cd13e66c84
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34757825"
---
# <a name="sync-sharepoint-files-with-the-new-onedrive-sync-client"></a><span data-ttu-id="6f288-102">SharePoint failu sinhronizēšana, izmantojot jauno OneDrive sinhronizācijas klientu</span><span class="sxs-lookup"><span data-stu-id="6f288-102">Sync SharePoint files with the new OneDrive sync client</span></span>

<span data-ttu-id="6f288-103">Komanda Atvērt ar Explorer atver Windows Explorer lokālu instanci, kas parāda mapju struktūru serverī, kurā tiek viesota SharePoint vietne.</span><span class="sxs-lookup"><span data-stu-id="6f288-103">The Open with Explorer command opens a local instance of Windows Explorer that displays the folder structure on the server that hosts the SharePoint site.</span></span> <span data-ttu-id="6f288-104">Tas nozīmē, ka ieteicams [sinhronizēt SharePoint failus, izmantojot jauno OneDrive sinhronizācijas klientu](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a>, kas nodrošina [failus pēc pieprasījuma](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e), jo tas nodrošina lokālu piekļuvi jūsu failiem un sniedz vislabāko veiktspēju.</span><span class="sxs-lookup"><span data-stu-id="6f288-104">This being said , we recommend [syncing SharePoint files with the new OneDrive sync client](https://support.office.com/article/sync-sharepoint-files-with-the-new-onedrive-sync-client-6de9ede8-5b6e-4503-80b2-6190f3354a88)</a> which provides [Files On-Demand](https://support.office.com/article/learn-about-onedrive-files-on-demand-0e6860d3-d9f3-4971-b321-7092438fb38e) because it provides local access to your files and offers the best performance.</span></span>


<span data-ttu-id="6f288-105">Ja izvēlējāties izmantot pārlūka skatu, nevis izmantot jauno sinhronizācijas klientu, turpmākajos rakstos sekojiet darbībām un paraugpraksei.</span><span class="sxs-lookup"><span data-stu-id="6f288-105">If you chose to use explorer view instead of using the new sync client, ensure you follow the steps and best practices in the articles below.</span></span>

- [<span data-ttu-id="6f288-106">Kā izmantot komandu "Atvērt ar Explorer", lai novērstu problēmas ar SharePoint Online</span><span class="sxs-lookup"><span data-stu-id="6f288-106">How to use the "Open with Explorer" command to troubleshoot issues in SharePoint Online</span></span>](https://support.office.com/article/How-to-use-the-Open-with-Explorer-command-to-troubleshoot-issues-in-SharePoint-Online-87155331-0c92-4224-a4c1-da5c21c4ade4)

- [<span data-ttu-id="6f288-107">Bibliotēkas failu kopēšana vai pārvietošana, izmantojot komandu Atvērt ar Explorer</span><span class="sxs-lookup"><span data-stu-id="6f288-107">Copy or move library files by using Open with Explorer</span></span>](https://support.office.com/article/copy-or-move-library-files-by-using-open-with-explorer-aaee7bfb-e2a1-42ee-8fc0-bcc0754f04d2)

<span data-ttu-id="6f288-108">Piezīme: poga Atvērt ar Explorer nav redzama jaunākajā bibliotēku pieredzē.</span><span class="sxs-lookup"><span data-stu-id="6f288-108">Note:  The Open with Explorer button doesn't appear in the new library experience.</span></span> <span data-ttu-id="6f288-109">Noklikšķiniet uz nolaižamās izvēlnes Skats augšējā labajā stūrī (nolaižamās izvēlnes nosaukums mainās, atkarībā no pašreizējā skata), un pēc tam noklikšķiniet uz Skats failu pārlūkā.</span><span class="sxs-lookup"><span data-stu-id="6f288-109">Click the View drop-down in the upper right (the name of the drop-down changes depending on your current view), and then click View in File Explorer.</span></span>

 <span data-ttu-id="6f288-110">SharePoint Atvērt ar Explorer izmanto ActiveX vadīklas, tāpēc to atbalsta tikai pārlūkprogramma Internet Explorer 10 vai 11.</span><span class="sxs-lookup"><span data-stu-id="6f288-110">SharePoint Open with Explorer uses ActiveX controls, so it's only supported in Internet Explorer 10 or 11.</span></span> <span data-ttu-id="6f288-111">Atvērt ar Explorer nedarbojas operētājsistēmā Windows ar pārlūkprogrammām Microsoft Edge, Google Chrome un Mozilla Firefox, kā arī platformā Mac.</span><span class="sxs-lookup"><span data-stu-id="6f288-111">Open with Explorer doesn't work in Windows with Microsoft Edge, Google Chrome, Mozilla Firefox, or on the Mac platform.</span></span> <span data-ttu-id="6f288-112">Šī iemesla dēļ pārlūka skata opcija var būt pelēkota.</span><span class="sxs-lookup"><span data-stu-id="6f288-112">Due to this reason, the Explorer View option may be grayed out.</span></span>

- <span data-ttu-id="6f288-113">[Kāpēc SharePoint lentes pogas nav pieejamas vai ir pelēkotas](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span><span class="sxs-lookup"><span data-stu-id="6f288-113">[Why SharePoint ribbon buttons are unavailable or grayed out](https://support.office.com/article/Why-SharePoint-ribbon-buttons-are-unavailable-48b0939a-2efb-4e79-b5e8-b2c4cb5d04ca).</span></span>
  
