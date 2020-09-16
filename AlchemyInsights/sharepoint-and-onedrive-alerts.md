---
title: SharePoint un OneDrive brīdinājumu saņemšanas aizkave
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 27cc744bc57f1c18649e05c5b0df3b315c9c0201
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47727250"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="fe335-102">SharePoint un OneDrive brīdinājumu saņemšanas aizkave</span><span class="sxs-lookup"><span data-stu-id="fe335-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="fe335-103">Vispirms pārbaudiet mapi Nevēlamais e-pasts.</span><span class="sxs-lookup"><span data-stu-id="fe335-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="fe335-104">Ja **visi brīdinājumi no vairākiem failiem vai bibliotēkām ir aizkavēti**, apmeklējiet [Pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home?ref=/servicehealth) , lai noskaidrotu, vai nav konsultantu/starpgadījumu, kas var notikt ar SharePoint vai Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe335-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="fe335-105">Šī problēma var būt saistīta ar SharePoint brīdinājumu iespējām vai kavējumiem e-pasta ziņojumos, izmantojot Exchange.</span><span class="sxs-lookup"><span data-stu-id="fe335-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="fe335-106">Ņemiet arī vērā, vai tiek piegādāts cits e-pasta ziņojums — ja tā nav, problēma ir iespējama ar Exchange kavējumiem.</span><span class="sxs-lookup"><span data-stu-id="fe335-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="fe335-107">Ja **atsevišķa faila vai bibliotēkas brīdinājums nav piegādāts**, mēģiniet to izdzēst un izveidot no jauna.</span><span class="sxs-lookup"><span data-stu-id="fe335-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="fe335-108">Lai atkārtoti izveidotu brīdinājumu, skatiet rakstu [SharePoint brīdinājumu pārvaldība, skatīšana un dzēšana](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="fe335-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="fe335-109">Brīdinājumus nevar nosūtīt uz adresātu grupu.</span><span class="sxs-lookup"><span data-stu-id="fe335-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="fe335-110">Tiek atbalstītas tikai drošības un O365 grupas.</span><span class="sxs-lookup"><span data-stu-id="fe335-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="fe335-111">Jūs nevarat pielāgot brīdinājuma e-pasta veidnes.</span><span class="sxs-lookup"><span data-stu-id="fe335-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="fe335-112">Lai sasniegtu šos pakalpojumus, ir jāizmanto Microsoft Flow vai SharePoint Designer darbplūsma.</span><span class="sxs-lookup"><span data-stu-id="fe335-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
