---
title: DLP var būt nepieciešams pielāgots tips
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: ''
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: 890bba57bc36c034c507e6124cd6593ef4d92af8
ms.sourcegitcommit: b0d5b68366028abcf08610672d5bc9d3b25ac433
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/24/2020
ms.locfileid: "42932665"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="9f048-102">DLP var būt nepieciešams pielāgots tips</span><span class="sxs-lookup"><span data-stu-id="9f048-102">DLP might need a custom type</span></span>

<span data-ttu-id="9f048-103">**Svarīgi**: daudzi SharePoint Online un OneDrive klienti darbojas kritiskās biznesa lietojumprogrammas pret pakalpojumu, kas darbojas fonā.</span><span class="sxs-lookup"><span data-stu-id="9f048-103">**Important**: Many SharePoint Online and OneDrive customers run business-critical applications against the service that run in the background.</span></span> <span data-ttu-id="9f048-104">Tie ietver satura migrācija, datu zuduma novēršana (DLP) un dublēšanas risinājumi.</span><span class="sxs-lookup"><span data-stu-id="9f048-104">These include content migration, Data Loss Prevention (DLP), and backup solutions.</span></span> <span data-ttu-id="9f048-105">Šo bezprecedenta reižu laikā mēs rīkojam, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir ļoti pieejami un uzticami lietotājiem, kuri ir atkarīgi no pakalpojuma vairāk nekā jebkad agrāk attālos darba scenārijos.</span><span class="sxs-lookup"><span data-stu-id="9f048-105">During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available and reliable for your users who depend on the service more than ever in remote work scenarios.</span></span>

<span data-ttu-id="9f048-106">Lai atbalstītu šo mērķi, mēs esam ieviesuši stingrākus ierobežošanas ierobežojumus fona lietotnēs (migrācija, DLP un dublēšanas risinājumi) darba dienās dienas laikā.</span><span class="sxs-lookup"><span data-stu-id="9f048-106">In support of this objective, we have implemented tighter throttling limits on background apps (migration, DLP and backup solutions) during weekday daytime hours.</span></span> <span data-ttu-id="9f048-107">Jums vajadzētu sagaidīt, ka šīs lietojumprogrammas šajā laikā sasniegs ļoti ierobežotu caurlaidspēju.</span><span class="sxs-lookup"><span data-stu-id="9f048-107">You should expect that these apps will achieve very limited throughput during these times.</span></span> <span data-ttu-id="9f048-108">Tomēr reģiona vakara un nedēļas nogales stundās pakalpojums būs gatavs apstrādāt ievērojami lielāku pieprasījumu apjomu no fona lietotnēm.</span><span class="sxs-lookup"><span data-stu-id="9f048-108">However, during evening and weekend hours for the region, the service will be ready to process a significantly higher volume of requests from background apps.</span></span>

<span data-ttu-id="9f048-109">**DLP var būt nepieciešams pielāgots informācijas tips**</span><span class="sxs-lookup"><span data-stu-id="9f048-109">**DLP may require a custom information type**</span></span>

<span data-ttu-id="9f048-110">Ar datu zuduma novēršanas (DLP) politiku jūs varat identificēt un aizsargāt sensitīvus datus savā organizācijā.</span><span class="sxs-lookup"><span data-stu-id="9f048-110">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="9f048-111">Dažos gadījumos, lai aizsargātu savas organizācijas datus, iespējams, vajadzēs izveidot **pielāgotu** sensitīvo informācijas tipu.</span><span class="sxs-lookup"><span data-stu-id="9f048-111">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="9f048-112">Piemēram, jūsu organizācijai var būt nepieciešams identificēt un aizsargāt darbinieku ID vai citus datus noteiktā formātā, kas specifisks jūsu organizācijai. Ja tā ir, skatiet šos rakstus, lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="9f048-112">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="9f048-113">**Iebūvēta sensitīva informācijas tipa pielāgošana**</span><span class="sxs-lookup"><span data-stu-id="9f048-113">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="9f048-114">Ja iebūvētais sensitīvo informācijas tips atbilst jūsu vajadzībām, izmantojot tikai dažas tweaks, varat [pielāgot iebūvēto sensitīvo informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="9f048-114">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="9f048-115">Piemēram, varat pievienot vai noņemt atslēgvārdus vai pievienot vai noņemt apstiprinošus pierādījumus, piemēram, datumu vai adresi.</span><span class="sxs-lookup"><span data-stu-id="9f048-115">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="9f048-116">**Pielāgota sensitīva informācijas tipa izveide**</span><span class="sxs-lookup"><span data-stu-id="9f048-116">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="9f048-117">Tomēr, ja jums ir jāidentificē un jāaizsargā cita veida sensitīva informācija, varat [izveidot pielāgotu sensitīvo informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) drošības & atbilstības centra lietotāja interfeisā.</span><span class="sxs-lookup"><span data-stu-id="9f048-117">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="9f048-118">**Pielāgota sensitīva informācijas tipa izveide drošības & atbilstības centra PowerShell**</span><span class="sxs-lookup"><span data-stu-id="9f048-118">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="9f048-119">Visbeidzot, ja UI nesniedz visas jums nepieciešamo opciju, [drošības & atbilstības centra PowerShell var izveidot pielāgotu sensitīvu informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="9f048-119">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="9f048-120">Sākot ar XML failu, var izmantot visas pieejamās opcijas.</span><span class="sxs-lookup"><span data-stu-id="9f048-120">By starting with an XML file, you can use every option available.</span></span>
