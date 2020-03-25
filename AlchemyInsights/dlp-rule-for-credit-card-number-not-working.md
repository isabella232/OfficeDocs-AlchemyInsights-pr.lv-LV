---
title: Nedarbojas DLP kārtula kredītkartes numurs
ms.author: deniseb
author: denisebmsft
manager: laurawi
ms.date: 11/5/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1270"
- "3200001"
ms.assetid: 30496c79-c8b4-4337-a46d-abed12864209
ms.openlocfilehash: 6b28534d072c024a98a9b05f6cb55bfdc3435db6
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932450"
---
# <a name="dlp-issues-with-credit-card-numbers"></a><span data-ttu-id="91cb0-102">DLP problēmas ar kredītkaršu numuriem</span><span class="sxs-lookup"><span data-stu-id="91cb0-102">DLP issues with credit card numbers</span></span>

<span data-ttu-id="91cb0-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="91cb0-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="91cb0-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="91cb0-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="91cb0-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="91cb0-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="91cb0-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="91cb0-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="91cb0-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="91cb0-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="91cb0-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="91cb0-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="91cb0-109">**DLP problēmas ar kredītkaršu numuriem**</span><span class="sxs-lookup"><span data-stu-id="91cb0-109">**DLP issues with credit card numbers**</span></span>

<span data-ttu-id="91cb0-110">Vai jums ir problēmas ar **datu zuduma novēršana (DLP)** nedarbojas saturu, kas satur **kredītkartes numuru** , izmantojot DLP konfidenciālu informācijas tipu O365?</span><span class="sxs-lookup"><span data-stu-id="91cb0-110">Are you having problems with **Data Loss Prevention (DLP)** not working for content containing a **Credit Card Number** when using a DLP sensitive information type in O365?</span></span> <span data-ttu-id="91cb0-111">Ja tā ir, pārliecinieties, vai saturs satur nepieciešamo informāciju, lai izraisītu DLP politiku, kad tā tiek novērtēta.</span><span class="sxs-lookup"><span data-stu-id="91cb0-111">If so, make sure your content contains the needed information to trigger the the DLP policy when it is evaluated.</span></span> <span data-ttu-id="91cb0-112">Piemēram, **kredītkartes politikai** , kas konfigurēta ar ticamības līmeni 85%, tiek novērtēti tālāk minētie un ir jānosaka, lai kārtula izraisītu:</span><span class="sxs-lookup"><span data-stu-id="91cb0-112">For example, for a **Credit Card policy** configured with a confidence level of 85%, the following are evaluated and must be detected for the rule to trigger:</span></span>
  
- <span data-ttu-id="91cb0-113">**[Formāts:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 cipari, kurus var formatēt vai Neformatēt (dddddddddddddd), un ir jānokārto Luhn tests.</span><span class="sxs-lookup"><span data-stu-id="91cb0-113">**[Format:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#format-19)** 16 digits which can be formatted or unformatted (dddddddddddddddd) and must pass the Luhn test.</span></span>

- <span data-ttu-id="91cb0-114">**[Modelis:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Ļoti sarežģīts un spēcīgs modelis, kas atrod kārtis no visiem lielākajiem zīmoliem visā pasaulē, ieskaitot visa, MasterCard, Discover Card, JCB, American Express, dāvanu kartes un pusdienotājs kartes.</span><span class="sxs-lookup"><span data-stu-id="91cb0-114">**[Pattern:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#pattern-19)** Very complex and robust pattern that detects cards from all major brands worldwide, including Visa, MasterCard, Discover Card, JCB, American Express, gift cards, and diner cards.</span></span>

- <span data-ttu-id="91cb0-115">**[Kontrolsumma:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Jā, Luhn kontrolsumma</span><span class="sxs-lookup"><span data-stu-id="91cb0-115">**[Checksum:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#checksum-19)** Yes, the Luhn checksum</span></span>

- <span data-ttu-id="91cb0-116">**[Definīcija:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** DLP politika ir 85% pārliecināta, ka tā tiek atklāta šāda veida sensitīva informācija, ja tuvums 300 rakstzīmes:</span><span class="sxs-lookup"><span data-stu-id="91cb0-116">**[Definition:](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#definition-19)** A DLP policy is 85% confident that it's detected this type of sensitive information if, within a proximity of 300 characters:</span></span>

  - <span data-ttu-id="91cb0-117">Funkcija Func_credit_card atrod saturu, kas atbilst paraugam.</span><span class="sxs-lookup"><span data-stu-id="91cb0-117">The function Func_credit_card finds content that matches the pattern.</span></span>

  - <span data-ttu-id="91cb0-118">Ir spēkā kāds no šiem:</span><span class="sxs-lookup"><span data-stu-id="91cb0-118">One of the following is true:</span></span>

  - <span data-ttu-id="91cb0-119">Tiek atrasts atslēgvārds no Keyword_cc_verification.</span><span class="sxs-lookup"><span data-stu-id="91cb0-119">A keyword from Keyword_cc_verification is found.</span></span>

  - <span data-ttu-id="91cb0-120">Tiek atrasts atslēgvārds no Keyword_cc_name</span><span class="sxs-lookup"><span data-stu-id="91cb0-120">A keyword from Keyword_cc_name is found</span></span>

  - <span data-ttu-id="91cb0-121">Funkcija Func_expiration_date atrod datumu pareizajā datuma formātā.</span><span class="sxs-lookup"><span data-stu-id="91cb0-121">The function Func_expiration_date finds a date in the right date format.</span></span>

  - <span data-ttu-id="91cb0-122">Kontrolsumma iet</span><span class="sxs-lookup"><span data-stu-id="91cb0-122">The checksum passes</span></span>

    <span data-ttu-id="91cb0-123">Piemēram, šādu paraugu izraisīs DLP kredītkartes numuru politika:</span><span class="sxs-lookup"><span data-stu-id="91cb0-123">For example, the following sample would trigger for a DLP Credit Card Number Policy:</span></span>

  - <span data-ttu-id="91cb0-124">Vīza: 4485 3647 3952 7352</span><span class="sxs-lookup"><span data-stu-id="91cb0-124">Visa: 4485 3647 3952 7352</span></span>
  
  - <span data-ttu-id="91cb0-125">Beidzas: 2/2009</span><span class="sxs-lookup"><span data-stu-id="91cb0-125">Expires: 2/2009</span></span>

<span data-ttu-id="91cb0-126">Lai iegūtu papildinformāciju par to, kas ir nepieciešams, lai jūsu saturam tiktu noteikts **kredītkartes numurs** , skatiet tālāk minēto sadaļu šajā rakstā: [kādas sensitīvās informācijas veidi](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number) tiek atrasti, izmantojot kredītkarti #</span><span class="sxs-lookup"><span data-stu-id="91cb0-126">For more information on what is required for a **Credit Card Number** to be detected for your content, see the following section in this article: [What the Sensitive Information Types look for Credit Card#](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for#credit-card-number)</span></span>
  
<span data-ttu-id="91cb0-127">Izmantojot citu iebūvētu sensitīvo informācijas tipu, skatiet šo rakstu, lai iegūtu informāciju par to, kas ir nepieciešams citiem tipiem: [, kāda veida sensitīvo informācijas veidu meklē](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span><span class="sxs-lookup"><span data-stu-id="91cb0-127">Using a different built-in sensitive information type, see the following article for information on what is required for other types: [What the Sensitive Information Types look for](https://docs.microsoft.com/office365/securitycompliance/what-the-sensitive-information-types-look-for)</span></span>
  