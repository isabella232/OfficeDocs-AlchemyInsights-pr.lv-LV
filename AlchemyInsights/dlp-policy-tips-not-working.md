---
title: DLP politikas padomi nedarbojas
ms.author: deniseb
author: denisebmsft
manager: laurawims
ms.date: 11/7/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: c03d30be-474a-4a34-b3c0-240eb2a2c466
ms.custom:
- "1428"
- "3200001"
ms.openlocfilehash: 51b4472fa721443192eb542cac45965df67634df
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932593"
---
# <a name="dlp-policy-tip-issues"></a><span data-ttu-id="a7a6c-102">DLP politikas Padoms problēmas</span><span class="sxs-lookup"><span data-stu-id="a7a6c-102">DLP Policy Tip issues</span></span>

<span data-ttu-id="a7a6c-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="a7a6c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="a7a6c-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="a7a6c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="a7a6c-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="a7a6c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="a7a6c-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="a7a6c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="a7a6c-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="a7a6c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="a7a6c-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="a7a6c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="a7a6c-109">**DLP politikas padomi**</span><span class="sxs-lookup"><span data-stu-id="a7a6c-109">**DLP policy tips**</span></span>

<span data-ttu-id="a7a6c-110">Izmantojot **DLP politiku**, lietotājiem var tikt paziņots par politikas pārkāpumu ar **politikas padomiem**.</span><span class="sxs-lookup"><span data-stu-id="a7a6c-110">When using **DLP policies**, users can be notified of a policy violation with **policy tips**.</span></span> <span data-ttu-id="a7a6c-111">Administratori var konfigurēt politikas padomus, kas tiek rādīti, pārbaudot to DLP politiku vai kad politika ir pilnā izpildes režīmā.</span><span class="sxs-lookup"><span data-stu-id="a7a6c-111">Admins can configure policy tips to display while testing their DLP policy or when the policy is in full enforcement mode.</span></span>
  
<span data-ttu-id="a7a6c-112">Lai konfigurētu politikas padomus DLP politikā drošības un atbilstības centrā pilnā izpildes režīmā, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="a7a6c-112">To configure policy tips on your DLP policy in the Security and Compliance center in full enforcement mode, do the following:</span></span>
  
- <span data-ttu-id="a7a6c-113">Nodrošināt politikas padomi ir **iespējoti** DLP kārtulu, izmantojot darbības [šeit](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span><span class="sxs-lookup"><span data-stu-id="a7a6c-113">Ensure policy tips have been **enabled** on the DLP rule using the steps [here](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips).</span></span>

- <span data-ttu-id="a7a6c-114">Pārliecinieties, ka jūsu **saturs atbilst** kas ir **nepieciešams** , lai izraisītu noteikumu, kas izklāstīti šajā rakstā [šeit](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span><span class="sxs-lookup"><span data-stu-id="a7a6c-114">Ensure your **content matches** what is **required** to trigger the rule outlined in this article [here](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for).</span></span>

- <span data-ttu-id="a7a6c-115">Politikas padomi parādīt gan OWA un Outlook.</span><span class="sxs-lookup"><span data-stu-id="a7a6c-115">Policy tips display in both OWA and Outlook.</span></span> <span data-ttu-id="a7a6c-116">Tomēr, izmantojot **Outlook 2013 vai jaunāku versiju**, politikas padomi tiek parādīti tikai konkrētos apstākļos.</span><span class="sxs-lookup"><span data-stu-id="a7a6c-116">However, when using **Outlook 2013 or later**, policy tips are only displayed under certain conditions.</span></span> <span data-ttu-id="a7a6c-117">Šie nosacījumi ir norādīti šeit: [atbalstītie nosacījumi programmai Outlook 2013 vai jaunākai versijai par politikas padomu parādīšanu](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span><span class="sxs-lookup"><span data-stu-id="a7a6c-117">These conditions are listed here: [Supported conditions for Outlook 2013 or later for displaying Policy Tips](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips#outlook-2013-and-later-supports-showing-policy-tips-for-only-some-conditions)</span></span>

<span data-ttu-id="a7a6c-118">Lai iegūtu papildinformāciju par DLP politikas tips, skatiet: [Rādīt politikas padomi DLP politikas](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span><span class="sxs-lookup"><span data-stu-id="a7a6c-118">For additional information on DLP policy tips, see: [Show policy tips for DLP Policies](https://docs.microsoft.com/office365/securitycompliance/use-notifications-and-policy-tips)</span></span>
  