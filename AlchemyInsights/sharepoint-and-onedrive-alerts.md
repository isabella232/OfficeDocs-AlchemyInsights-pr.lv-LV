---
title: SharePoint un OneDrive brīdinājumu saņemšanas aizkave
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000118"
- "2642"
ms.openlocfilehash: 92e517ae6e83aa91b9838047ec77759dc893bc57
ms.sourcegitcommit: 90f37eebec9aaa9e49c2cf4d201152c5e20e384b
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/17/2020
ms.locfileid: "46785672"
---
# <a name="delays-in-receiving-sharepoint-and-onedrive-alerts"></a><span data-ttu-id="f10be-102">SharePoint un OneDrive brīdinājumu saņemšanas aizkave</span><span class="sxs-lookup"><span data-stu-id="f10be-102">Delays in receiving SharePoint and OneDrive alerts</span></span>

- <span data-ttu-id="f10be-103">Vispirms pārbaudiet mapi Nevēlamais e-pasts.</span><span class="sxs-lookup"><span data-stu-id="f10be-103">First check the Junk or Spam folder in your email.</span></span>
- <span data-ttu-id="f10be-104">Ja **visi brīdinājumi no vairākiem failiem vai bibliotēkām ir aizkavēti**, apmeklējiet [Pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home?ref=/servicehealth) , lai noskaidrotu, vai nav konsultantu/starpgadījumu, kas var notikt ar SharePoint vai Exchange.</span><span class="sxs-lookup"><span data-stu-id="f10be-104">If **all alerts from multiple files or libraries are delayed**, visit the [Service Health dashboard](https://portal.office.com/adminportal/home?ref=/servicehealth) to check for any advisories/incidents that may be occurring with SharePoint or Exchange.</span></span> <span data-ttu-id="f10be-105">Šī problēma var būt saistīta ar SharePoint brīdinājumu iespējām vai kavējumiem e-pasta ziņojumos, izmantojot Exchange.</span><span class="sxs-lookup"><span data-stu-id="f10be-105">The issue might be with the SharePoint alert capability or delays in emails through Exchange.</span></span> <span data-ttu-id="f10be-106">Ņemiet arī vērā, vai tiek piegādāts cits e-pasta ziņojums — ja tā nav, problēma ir iespējama ar Exchange kavējumiem.</span><span class="sxs-lookup"><span data-stu-id="f10be-106">Also note whether other email is being delivered—if not, the issue is likely with Exchange delays.</span></span>
- <span data-ttu-id="f10be-107">Ja **atsevišķa faila vai bibliotēkas brīdinājums nav piegādāts**, mēģiniet to izdzēst un izveidot no jauna.</span><span class="sxs-lookup"><span data-stu-id="f10be-107">If **an individual alert from a specific file or library is not delivered**, attempt to delete and recreate it.</span></span> <span data-ttu-id="f10be-108">Lai atkārtoti izveidotu brīdinājumu, skatiet rakstu [SharePoint brīdinājumu pārvaldība, skatīšana un dzēšana](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) .</span><span class="sxs-lookup"><span data-stu-id="f10be-108">See [Manage, view, or delete SharePoint alerts](https://support.microsoft.com/office/99dfb19c-9a90-4a8c-aba1-aa8c8afb0de2) to recreate the alert.</span></span>

> [!NOTE]
> - <span data-ttu-id="f10be-109">Brīdinājumus nevar nosūtīt uz adresātu grupu.</span><span class="sxs-lookup"><span data-stu-id="f10be-109">Alerts cannot be sent to a Distribution Group.</span></span> <span data-ttu-id="f10be-110">Tiek atbalstītas tikai drošības un O365 grupas.</span><span class="sxs-lookup"><span data-stu-id="f10be-110">Only Security and O365 groups are supported.</span></span>
> - <span data-ttu-id="f10be-111">Jūs nevarat pielāgot brīdinājuma e-pasta veidnes.</span><span class="sxs-lookup"><span data-stu-id="f10be-111">You cannot customize alert email templates.</span></span> <span data-ttu-id="f10be-112">Lai sasniegtu šos pakalpojumus, ir jāizmanto Microsoft Flow vai SharePoint Designer darbplūsma.</span><span class="sxs-lookup"><span data-stu-id="f10be-112">You must use Microsoft Flow or SharePoint Designer Workflow to achieve those.</span></span>
