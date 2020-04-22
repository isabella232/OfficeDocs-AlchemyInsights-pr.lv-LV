---
title: DLP var būt nepieciešams pielāgots tips
ms.author: pebaum
author: pebaum
manager: laurawi
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.prod: office-online-server
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "1647"
- "3200001"
ms.assetid: ''
ms.openlocfilehash: b83bb77383e2ae7e78c31f35c972182c54487c60
ms.sourcegitcommit: 55eff703a17e500681d8fa6a87eb067019ade3cc
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43704496"
---
# <a name="dlp-might-need-a-custom-type"></a><span data-ttu-id="6ae9e-102">DLP var būt nepieciešams pielāgots tips</span><span class="sxs-lookup"><span data-stu-id="6ae9e-102">DLP might need a custom type</span></span>

<span data-ttu-id="6ae9e-103">**Svarīgi**: šo bezprecedenta laiku mēs veicam darbības, lai nodrošinātu, ka SharePoint Online un OneDrive pakalpojumi joprojām ir plaši pieejami. Lai iegūtu papildinformāciju, apmeklējiet [SharePoint Online pagaidu līdzekļu pielāgojumi](https://aka.ms/ODSPAdjustments).</span><span class="sxs-lookup"><span data-stu-id="6ae9e-103">**Important**: During these unprecedented times, we are taking steps to ensure that SharePoint Online and OneDrive services remain highly available – Please visit [SharePoint Online Temporary Feature Adjustments](https://aka.ms/ODSPAdjustments) for more information.</span></span>

<span data-ttu-id="6ae9e-104">**DLP var būt nepieciešams pielāgots informācijas tips**</span><span class="sxs-lookup"><span data-stu-id="6ae9e-104">**DLP may require a custom information type**</span></span>

<span data-ttu-id="6ae9e-105">Ar datu zuduma novēršanas (DLP) politiku jūs varat identificēt un aizsargāt sensitīvus datus savā organizācijā.</span><span class="sxs-lookup"><span data-stu-id="6ae9e-105">With a data loss prevention (DLP) policy, you can identify and protect sensitive data in your organization.</span></span> <span data-ttu-id="6ae9e-106">Dažos gadījumos, lai aizsargātu savas organizācijas datus, iespējams, vajadzēs izveidot **pielāgotu** sensitīvo informācijas tipu.</span><span class="sxs-lookup"><span data-stu-id="6ae9e-106">In some scenarios, you might need to create your own **custom** sensitive information type to protect your organization's data.</span></span>

<span data-ttu-id="6ae9e-107">Piemēram, jūsu organizācijai var būt nepieciešams identificēt un aizsargāt darbinieku ID vai citus datus noteiktā formātā, kas specifisks jūsu organizācijai. Ja tā ir, skatiet šos rakstus, lai iegūtu papildinformāciju.</span><span class="sxs-lookup"><span data-stu-id="6ae9e-107">For example, your organization might need to identify and protect employee IDs or other data in some format specific to your org. If so, see the following articles for more information.</span></span>
  
 <span data-ttu-id="6ae9e-108">**Iebūvēta sensitīva informācijas tipa pielāgošana**</span><span class="sxs-lookup"><span data-stu-id="6ae9e-108">**Customize a built-in sensitive information type**</span></span>
  
<span data-ttu-id="6ae9e-109">Ja iebūvētais sensitīvo informācijas tips atbilst jūsu vajadzībām, izmantojot tikai dažas tweaks, varat [pielāgot iebūvēto sensitīvo informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span><span class="sxs-lookup"><span data-stu-id="6ae9e-109">If a built-in sensitive information type would meet your needs with just a few tweaks, you can [customize a built-in sensitive information type](https://docs.microsoft.com/office365/securitycompliance/customize-a-built-in-sensitive-information-type).</span></span> <span data-ttu-id="6ae9e-110">Piemēram, varat pievienot vai noņemt atslēgvārdus vai pievienot vai noņemt apstiprinošus pierādījumus, piemēram, datumu vai adresi.</span><span class="sxs-lookup"><span data-stu-id="6ae9e-110">For example, you can add or remove keywords, or add or remove supporting evidence such as a date or address.</span></span>
  
 <span data-ttu-id="6ae9e-111">**Pielāgota sensitīva informācijas tipa izveide**</span><span class="sxs-lookup"><span data-stu-id="6ae9e-111">**Create a custom sensitive information type**</span></span>
  
<span data-ttu-id="6ae9e-112">Tomēr, ja jums ir jāidentificē un jāaizsargā cita veida sensitīva informācija, varat [izveidot pielāgotu sensitīvo informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) drošības & atbilstības centra lietotāja interfeisā.</span><span class="sxs-lookup"><span data-stu-id="6ae9e-112">But if you need to identify and protect a different type of sensitive information altogether, you can [create a custom sensitive information type](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type) in the UI of the Security & Compliance Center.</span></span>
  
<span data-ttu-id="6ae9e-113">**Pielāgota sensitīva informācijas tipa izveide drošības & atbilstības centra PowerShell**</span><span class="sxs-lookup"><span data-stu-id="6ae9e-113">**Create a custom sensitive information type in Security & Compliance Center PowerShell**</span></span>

<span data-ttu-id="6ae9e-114">Visbeidzot, ja UI nesniedz visas jums nepieciešamo opciju, [drošības & atbilstības centra PowerShell var izveidot pielāgotu sensitīvu informācijas tipu](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span><span class="sxs-lookup"><span data-stu-id="6ae9e-114">Finally, if the UI doesn't provide all the options you need, you can [create a custom sensitive information type in Security & Compliance Center PowerShell](https://docs.microsoft.com/office365/securitycompliance/create-a-custom-sensitive-information-type-in-scc-powershell).</span></span> <span data-ttu-id="6ae9e-115">Sākot ar XML failu, var izmantot visas pieejamās opcijas.</span><span class="sxs-lookup"><span data-stu-id="6ae9e-115">By starting with an XML file, you can use every option available.</span></span>
