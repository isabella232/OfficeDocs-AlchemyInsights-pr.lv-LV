---
title: E-datu atklāšanas/satura meklēšanas rezultātu eksportēšana
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 02/26/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "3200003"
- "7221"
ms.openlocfilehash: b93377a33eebc7899041b684449e46caedb04415
ms.sourcegitcommit: 251e2e82571fb3bb1fbe3dbf7bfca30e004b3373
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/05/2021
ms.locfileid: "50482622"
---
# <a name="export-ediscoverycontent-search-results"></a><span data-ttu-id="ff1ac-102">E-datu atklāšanas/satura meklēšanas rezultātu eksportēšana</span><span class="sxs-lookup"><span data-stu-id="ff1ac-102">Export eDiscovery/Content Search results</span></span>

<span data-ttu-id="ff1ac-103">Iespējams, ka būs jāeksportē meklēšanas rezultāti uz PST failu (no e-pasta) vai uz vietējiem Office dokumentiem (no SharePoint un OneDrive darbam vietnēm).</span><span class="sxs-lookup"><span data-stu-id="ff1ac-103">You may need to export your search results to a PST file (from email) or to native Office documents (from SharePoint and OneDrive for Business sites).</span></span> <span data-ttu-id="ff1ac-104">Ja tā ir, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="ff1ac-104">If so, do the following:</span></span>

- <span data-ttu-id="ff1ac-105">Pārliecinieties, vai jūsu kontam ir piešķirtas atbilstošas atļaujas eksportēšanai.</span><span class="sxs-lookup"><span data-stu-id="ff1ac-105">Make sure your account is assigned the proper permissions to export.</span></span> <span data-ttu-id="ff1ac-106">Papildinformāciju skatiet rakstā e- [datu atklāšanas atļauju piešķiršana](https://go.microsoft.com/fwlink/?linkid=2102406).</span><span class="sxs-lookup"><span data-stu-id="ff1ac-106">For more info, see [Assign eDiscovery permission](https://go.microsoft.com/fwlink/?linkid=2102406).</span></span>
- <span data-ttu-id="ff1ac-107">Pārliecinieties, vai jūsu datorā ir ievēroti visi [priekšnosacījumi](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span><span class="sxs-lookup"><span data-stu-id="ff1ac-107">Make sure your computer has met all [prerequisites](https://docs.microsoft.com/office365/securitycompliance/export-search-results#before-you-begin).</span></span> <span data-ttu-id="ff1ac-108">Netiek atbalstītas visas pārlūkprogrammas, piemēram, Chrome.</span><span class="sxs-lookup"><span data-stu-id="ff1ac-108">Not all browsers are supported, such as Chrome.</span></span>
- <span data-ttu-id="ff1ac-109">Lai eksportētu no satura meklēšanas: a.</span><span class="sxs-lookup"><span data-stu-id="ff1ac-109">To export from a Content Search: a.</span></span> <span data-ttu-id="ff1ac-110">Dodieties uz [drošības & atbilstības centru](https://protection.office.com/contentsearch) un noklikšķiniet uz **Meklēt** un pēc tam atlasiet **satura meklēšana**.</span><span class="sxs-lookup"><span data-stu-id="ff1ac-110">Go to the [Security & Compliance Center](https://protection.office.com/contentsearch) and click **Search**, and then select **Content search**.</span></span> <span data-ttu-id="ff1ac-111">Lapā **satura meklēšana** atlasiet saglabāto meklēšanu.</span><span class="sxs-lookup"><span data-stu-id="ff1ac-111">On the **Content search** page, select a saved search.</span></span>
    <span data-ttu-id="ff1ac-112">b.</span><span class="sxs-lookup"><span data-stu-id="ff1ac-112">b.</span></span> <span data-ttu-id="ff1ac-113">Detalizētās informācijas rūts sadaļā **eksportēt rezultātus uz datoru** atlasiet **sākt eksportēšanu**.</span><span class="sxs-lookup"><span data-stu-id="ff1ac-113">On the Details pane, under **Export results to a computer**, select **Start export**.</span></span> <span data-ttu-id="ff1ac-114">Ja eksportējat vairāk nekā 100K pastkastes, ir jāizmanto PowerShell, lai lejupielādētu eksportēšanas rezultātus.</span><span class="sxs-lookup"><span data-stu-id="ff1ac-114">If you're exporting more than 100K mailboxes, you'll need to use PowerShell to download the export results.</span></span> <span data-ttu-id="ff1ac-115">Papildinformāciju skatiet rakstā [rezultātu eksportēšana no vairāk nekā 100k pastkastēm](https://go.microsoft.com/fwlink/?linkid=2143861).</span><span class="sxs-lookup"><span data-stu-id="ff1ac-115">For more info, see [Exporting results from more than 100K mailboxes](https://go.microsoft.com/fwlink/?linkid=2143861).</span></span>

<span data-ttu-id="ff1ac-116">Papildinformāciju skatiet rakstā [satura meklēšanas rezultātu eksportēšana](https://go.microsoft.com/fwlink/?linkid=2102118).</span><span class="sxs-lookup"><span data-stu-id="ff1ac-116">To learn more, see [Export Content Search Results](https://go.microsoft.com/fwlink/?linkid=2102118).</span></span>