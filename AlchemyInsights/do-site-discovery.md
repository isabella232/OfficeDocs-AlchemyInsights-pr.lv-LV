---
title: Veikt vietnes atklāšanu
ms.author: v-smandalika
author: v-smandalika
manager: dansimp
ms.date: 03/08/2021
audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9143"
- "9005291"
ms.openlocfilehash: bdf94220de45d92f63e56501ea4e35389224d25c
ms.sourcegitcommit: 475a9eaa095812091991857df6cf6490a8bbe179
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/08/2021
ms.locfileid: "50693484"
---
# <a name="do-site-discovery"></a><span data-ttu-id="b6816-102">Veikt vietnes atklāšanu</span><span class="sxs-lookup"><span data-stu-id="b6816-102">Do site discovery</span></span>

<span data-ttu-id="b6816-103">Ja jūsu organizācijā joprojām tiek izmantotas mantotās tīmekļa lietojumprogrammas un plāni, lai izmantotu Internet Explorer režīmu (ko lielākā daļa klientu), jums jāveic papildu vietņu noteikšana.</span><span class="sxs-lookup"><span data-stu-id="b6816-103">If your organization still uses legacy web applications and plans to use Internet Explorer mode (which most customers do), then you should do some additional site discovery.</span></span>

<span data-ttu-id="b6816-104">**Jūs jau esat izvietojis vecāku Microsoft Edge versiju**</span><span class="sxs-lookup"><span data-stu-id="b6816-104">**You've already deployed an older version of Microsoft Edge**</span></span>

<span data-ttu-id="b6816-105">Ja jau esat konfigurējis savu uzņēmuma vietnes sarakstu, lai strādātu ar Microsoft Edge mantoto versiju, pēc tam ir gandrīz gatavs vietnes atklāšana.</span><span class="sxs-lookup"><span data-stu-id="b6816-105">If you've already configured your Enterprise Site List to work for the legacy version of Microsoft Edge, then your site discovery is almost done.</span></span> <span data-ttu-id="b6816-106">Tas, kas jums, iespējams, ir jādara, ir jāpievieno neitrālas vietnes.</span><span class="sxs-lookup"><span data-stu-id="b6816-106">The one thing you might need to do is add neutral sites.</span></span>

<span data-ttu-id="b6816-107">Neitrālās vietnes parasti ir vietnes, kas nodrošina vienotās pierakstīšanās (SSO).</span><span class="sxs-lookup"><span data-stu-id="b6816-107">Neutral sites are typically sites that provide single sign-on (SSO).</span></span> <span data-ttu-id="b6816-108">Ja dodaties uz neitrālu vietni no Microsoft Edge, jūs vēlaties saglabāt pārlūkprogrammā Microsoft Edge, lai veiktu autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="b6816-108">If you go to a neutral site from Microsoft Edge, then you want to stay in Microsoft Edge to authenticate.</span></span> <span data-ttu-id="b6816-109">Ja pārlūkprogrammā Internet Explorer režīmā dodaties uz neitrālu vietni, jūs vēlaties, lai autentificētos Internet Explorer režīms.</span><span class="sxs-lookup"><span data-stu-id="b6816-109">If you go to a neutral site in Internet Explorer mode, then you want to stay in Internet Explorer mode to authenticate.</span></span>

<span data-ttu-id="b6816-110">Identificējiet visas SSO vai citas neitrālas vietnes, ko izmantojat, un pievienojiet tās savā uzņēmuma vietnes sarakstā.</span><span class="sxs-lookup"><span data-stu-id="b6816-110">Identify any SSO or other neutral sites that you use and add these to your Enterprise Site List.</span></span>

<span data-ttu-id="b6816-111">**Internet Explorer ir noklusējuma pārlūkprogramma**</span><span class="sxs-lookup"><span data-stu-id="b6816-111">**Internet Explorer is your default browser**</span></span>

<span data-ttu-id="b6816-112">Ja tagad izmantojat tikai Internet Explorer, iespējams, nezināsit, kuras vietnes ir jauninātas uz mūsdienīgiem tīmekļa standartiem un kurām joprojām ir nepieciešama pārlūkprogramma Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="b6816-112">If you're only using Internet Explorer now, you might not know which sites have upgraded to modern web standards and which still require Internet Explorer.</span></span> <span data-ttu-id="b6816-113">Jūs vēlēsities atrast un pievienot šīs vietnes uzņēmuma vietņu sarakstam, lai jūs varētu izmantot Internet Explorer režīmu tikai šīm vietnēm.</span><span class="sxs-lookup"><span data-stu-id="b6816-113">You'll want to find and add these sites to the Enterprise Site List so that you can use Internet Explorer mode only for those sites.</span></span>

> [!NOTE]
> <span data-ttu-id="b6816-114">[Uzņēmuma vietnes noteikšana](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) atklāj vietnes, kurām, iespējams, ir jāatver Internet Explorer režīms.</span><span class="sxs-lookup"><span data-stu-id="b6816-114">[Enterprise Site Discovery](https://docs.microsoft.com/internet-explorer/ie11-deploy-guide/collect-data-using-enterprise-site-discovery) discovers sites that might need Internet Explorer mode.</span></span> <span data-ttu-id="b6816-115">Tas var vākt datus datoros, kuros darbojas Windows Internet Explorer 8, izmantojot Internet Explorer 11 operētājsistēmā Windows 10, Windows 8,1 vai Windows 7.</span><span class="sxs-lookup"><span data-stu-id="b6816-115">It can collect data on computers running Windows Internet Explorer 8 through Internet Explorer 11 on Windows 10, Windows 8.1, or Windows 7.</span></span>

<span data-ttu-id="b6816-116">**Datu analīze**</span><span class="sxs-lookup"><span data-stu-id="b6816-116">**Analyze the data**</span></span>

<span data-ttu-id="b6816-117">Pēc tam, kad esat savācis vietnes datus, iesakām veikt tālāk norādītās četru soļu procesa datu analizēšanai.</span><span class="sxs-lookup"><span data-stu-id="b6816-117">After you've collected site data, we recommend the following four-step process to analyze the data:</span></span>
1. <span data-ttu-id="b6816-118">Kārtojiet datus pēc domēna un pēc tam pēc vietrāža URL.</span><span class="sxs-lookup"><span data-stu-id="b6816-118">Sort the data by domain, and then by URL.</span></span>
2. <span data-ttu-id="b6816-119">Definējiet programmas robežas, lai konfigurētu Internet Explorer režīmu.</span><span class="sxs-lookup"><span data-stu-id="b6816-119">Define the boundaries of an app to configure for Internet Explorer mode.</span></span> <span data-ttu-id="b6816-120">Vēlaties iekļaut visas vietnes un tīmekļa vadīklas, kas definē programmu, taču nevēlaties iekļaut papildu vietnes un vadīklas.</span><span class="sxs-lookup"><span data-stu-id="b6816-120">You want to include all the sites and web controls that define the app, but you don't want to include extra sites and controls.</span></span> <span data-ttu-id="b6816-121">Dažas vietnes var būt tik vienkāršas, cik *https://contoso.com/app1* savukārt citiem lietotājiem var būt nepieciešams definēt vairākas vietnes un lapas.</span><span class="sxs-lookup"><span data-stu-id="b6816-121">Some sites might be as simple as *https://contoso.com/app1* while others might require you to define multiple sites and pages.</span></span>
3. <span data-ttu-id="b6816-122">Testējiet lietojumprogrammu, lai pārliecinātos, vai tā nav nevainojama.</span><span class="sxs-lookup"><span data-stu-id="b6816-122">Test the app to verify that it doesn't work natively.</span></span> <span data-ttu-id="b6816-123">Daudzās vietnēs tiks piedāvāts mūsdienīgs saturs, kad tie atklāj mūsdienīgu pārlūkprogrammu un piedāvā mantotu saturu tikai tad, kad tie atklāj Internet Explorer.</span><span class="sxs-lookup"><span data-stu-id="b6816-123">Many sites will offer modern content when they detect a modern browser and only offer legacy content when they detect Internet Explorer.</span></span>
4. <span data-ttu-id="b6816-124">Pievienojiet programmu sarakstam uzņēmuma vietne, ja tā neveic testēšanu.</span><span class="sxs-lookup"><span data-stu-id="b6816-124">Add the app to your Enterprise Site List if it fails testing.</span></span>

> [!NOTE]
> <span data-ttu-id="b6816-125">Kā paraugpraksi grupējiet visas vietnes, kurās ietilpst programma.</span><span class="sxs-lookup"><span data-stu-id="b6816-125">As a best practice, group all of the sites that comprise an app.</span></span> <span data-ttu-id="b6816-126">Šādā veidā, jauninot programmu, ir vieglāk noņemt visu vietni no Internet Explorer režīma un sākt izmantot šīs lietojumprogrammas mūsdienīgu pārlūkprogrammu.</span><span class="sxs-lookup"><span data-stu-id="b6816-126">This way, when you upgrade an app, it's easier to remove the entire site from Internet Explorer mode and start using a modern browser for that app.</span></span>

<span data-ttu-id="b6816-127">Kad esat pabeidzis vietnes atklāšanu un esat analizējis datus, esat gatavs sākt meklēt savā kanālu stratēģijā.</span><span class="sxs-lookup"><span data-stu-id="b6816-127">Once you're done with site discovery and you've analyzed the data, you're ready to start looking at your channel strategy.</span></span>

