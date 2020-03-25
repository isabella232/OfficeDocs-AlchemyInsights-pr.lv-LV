---
title: DLP noteikums ASV/Lielbritānijas pases numurs nedarbojas
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1319"
- "3200001"
ms.assetid: fc178b8b-943b-4346-a2bd-a75c6af6f80f
ms.openlocfilehash: c63e814059c897531109aa78725e9811b311fb27
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42931269"
---
# <a name="problems-with-dlp---usuk-passport-numbers"></a><span data-ttu-id="64f6a-102">Problēmas ar DLP-US/UK pases numuru</span><span class="sxs-lookup"><span data-stu-id="64f6a-102">Problems with DLP - US/UK passport numbers</span></span>

<span data-ttu-id="64f6a-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="64f6a-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="64f6a-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="64f6a-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="64f6a-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="64f6a-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="64f6a-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="64f6a-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="64f6a-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="64f6a-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="64f6a-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="64f6a-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="64f6a-109">**DLP jautājumi ar ASV/Lielbritānijas pases numuriem**</span><span class="sxs-lookup"><span data-stu-id="64f6a-109">**DLP issues with US/UK passport numbers**</span></span>

<span data-ttu-id="64f6a-110">Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nestrādā par saturu, kas satur **ASV/UK pases numuru** , izmantojot DLP konfidenciālu informāciju tipa O365?</span><span class="sxs-lookup"><span data-stu-id="64f6a-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **US/UK passport number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="64f6a-111">Ja tā ir, pārliecinieties, ka jūsu saturs satur nepieciešamo informāciju par to, ko DLP politika meklē, kad tas ir novērtēts.</span><span class="sxs-lookup"><span data-stu-id="64f6a-111">If so, make sure your content contains the needed information for what the DLP policy is looking for when it is evaluated.</span></span>
  
<span data-ttu-id="64f6a-112">Piemēram, **ASV/Apvienotās Karalistes pases numuru** politikai, kas konfigurēta ar ticamības līmeni 75%, tiek novērtēti tālāk minētie, un tie ir jānosaka, lai kārtula izraisītu</span><span class="sxs-lookup"><span data-stu-id="64f6a-112">For example, for a **US/UK passport number** policy configured with a confidence level of 75%, the following are evaluated and must be detected for the rule to trigger</span></span>
  
- <span data-ttu-id="64f6a-113">**[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Deviņi cipari</span><span class="sxs-lookup"><span data-stu-id="64f6a-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-77)** Nine digits</span></span>

- <span data-ttu-id="64f6a-114">**[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Deviņus secīgus ciparus</span><span class="sxs-lookup"><span data-stu-id="64f6a-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-77)** Nine consecutive digits</span></span>

- <span data-ttu-id="64f6a-115">**[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** Nē, nav kontrolsummas</span><span class="sxs-lookup"><span data-stu-id="64f6a-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-76)** No, there is no Checksum</span></span>

- <span data-ttu-id="64f6a-116">**[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** DLP politika ir 75% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:</span><span class="sxs-lookup"><span data-stu-id="64f6a-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-77)** A DLP policy is 75% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="64f6a-117">Funkcija Func_usa_uk_passport atrod saturu, kas atbilst paraugam.</span><span class="sxs-lookup"><span data-stu-id="64f6a-117">The function Func_usa_uk_passport finds content that matches the pattern.</span></span>

  - <span data-ttu-id="64f6a-118">Tiek atrasts atslēgvārds no Keyword_passport.</span><span class="sxs-lookup"><span data-stu-id="64f6a-118">A keyword from Keyword_passport is found.</span></span>

    <span data-ttu-id="64f6a-119">Piemēram, šādu paraugu izraisītu **ASV/Lielbritānijas pases numuru** politika: ASV pases numurs 123456789</span><span class="sxs-lookup"><span data-stu-id="64f6a-119">For example, the following sample would trigger for the **US/UK passport number** policy: U.S. Passport number 123456789</span></span>

<span data-ttu-id="64f6a-120">Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai jūsu saturam tiktu noteikts ASV/Apvienotās Karalistes pases numurs, skatiet šajā rakstā minēto sadaļu: [kādas sensitīvās informācijas veidi meklē US/UK pases numuru](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span><span class="sxs-lookup"><span data-stu-id="64f6a-120">For more information on what is required for a US/UK Passport Number to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for US/UK Passport Number](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#us--uk-passport-number)</span></span>
  
<span data-ttu-id="64f6a-121">Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="64f6a-121">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  