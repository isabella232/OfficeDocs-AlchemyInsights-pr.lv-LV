---
title: SharePoint migrācijas ierobežošana ar 503 kļūdas
ms.author: pebaum
author: pebaum
ms.date: 8/8/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: ''
ms.custom:
- "9000136"
- "2541"
ms.openlocfilehash: 7e12c74d33e3cee7c626ad899a4e7f2f0a409bca
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931665"
---
# <a name="sharepoint-migration-throttling-with-503-errors"></a><span data-ttu-id="b791c-102">SharePoint migrācijas ierobežošana ar 503 kļūdas</span><span class="sxs-lookup"><span data-stu-id="b791c-102">SharePoint migration throttling with 503 errors</span></span>

<span data-ttu-id="b791c-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="b791c-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="b791c-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="b791c-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="b791c-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="b791c-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="b791c-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="b791c-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="b791c-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="b791c-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="b791c-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="b791c-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="b791c-109">**503 kļūdas, migrējot uz SharePoint Online**</span><span class="sxs-lookup"><span data-stu-id="b791c-109">**503 errors when migrating to SharePoint Online**</span></span>

<span data-ttu-id="b791c-110">Šķiet, jums ir migrācija uz SharePoint Online un saņem 503 kļūdas.</span><span class="sxs-lookup"><span data-stu-id="b791c-110">It appears you are migrating to SharePoint Online and receiving 503 errors.</span></span> <span data-ttu-id="b791c-111">Lūdzu, veiciet tālāk norādītās darbības, lai mēs varētu jums palīdzēt pēc iespējas ātrāk.</span><span class="sxs-lookup"><span data-stu-id="b791c-111">Please follow the steps below so we may assist you as soon as possible.</span></span> 

1. <span data-ttu-id="b791c-112">Noklikšķiniet uz **sazināties ar atbalsta dienestu**un pēc tam uz **Jauns pakalpojuma pieprasījums**.</span><span class="sxs-lookup"><span data-stu-id="b791c-112">Click **Contact Support**, and then **New Service Request**.</span></span>
2. <span data-ttu-id="b791c-113">Nosaukumu un aprakstu, ierakstiet **SharePoint migrācijas ierobežošana ar 503**.</span><span class="sxs-lookup"><span data-stu-id="b791c-113">For the title and description, type **SharePoint Migration Throttling with 503**.</span></span>
3. <span data-ttu-id="b791c-114">Kad biļete ir iesniegta, lūdzu, atjauniniet to ar šādu informāciju:</span><span class="sxs-lookup"><span data-stu-id="b791c-114">Once the ticket has been submitted, please update it with the following information:</span></span>
    - <span data-ttu-id="b791c-115">Cik kreisi no migrācijas (piemēram, cik TBs?).</span><span class="sxs-lookup"><span data-stu-id="b791c-115">How much left of migration (for example, how many TBs?).</span></span>
    - <span data-ttu-id="b791c-116">Migrācijas sākuma un beigu datumu.</span><span class="sxs-lookup"><span data-stu-id="b791c-116">Migration start and end date.</span></span>
    - <span data-ttu-id="b791c-117">Aprakstiet, kur jūs migrējat saturu no, piemēram, SharePoint Server, Box, GDrive, failu koplietojumos utt.</span><span class="sxs-lookup"><span data-stu-id="b791c-117">Describe where you are migrating your content from, such as SharePoint Server, Box, GDrive, File shares, etc..</span></span>
    - <span data-ttu-id="b791c-118">Novērtēt ierobežošanas kļūdu skaitu (piemēram, x droseli stundā?) un kad notika ierobežošana.</span><span class="sxs-lookup"><span data-stu-id="b791c-118">Estimate the number of throttling errors (for example, x throttle per hour?) and when did the throttling happen.</span></span>
    - <span data-ttu-id="b791c-119">Kuru migrācijas rīku lietojat (piemēram, SPMT vai ShareGate).</span><span class="sxs-lookup"><span data-stu-id="b791c-119">Which migration tool you are using (for example, SPMT or ShareGate).</span></span>


