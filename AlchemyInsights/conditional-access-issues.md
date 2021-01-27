---
title: Ierobežotas piekļuves problēmas
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 01/25/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004349"
- "7768"
ms.openlocfilehash: 7c20b26e3a038dc4392684ca410eba97cec2df30
ms.sourcegitcommit: eb685eea3ab312d404d55bfd5594a5d6d68811d1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/27/2021
ms.locfileid: "50014885"
---
# <a name="conditional-access-issues"></a><span data-ttu-id="bca35-102">Ierobežotas piekļuves problēmas</span><span class="sxs-lookup"><span data-stu-id="bca35-102">Conditional access issues</span></span>

<span data-ttu-id="bca35-103">**Problēmu novēršana saistībā ar pierakstīšanās diagnostiku**</span><span class="sxs-lookup"><span data-stu-id="bca35-103">**Resolve problems with the Sign-in Diagnostic**</span></span>

<span data-ttu-id="bca35-104">Varat ātri noskaidrot, kas notika vai diagnosticēt problēmas, kas saistītas ar lietotāja pierakstīšanos, izmantojot [pierakstīšanās diagnostiku](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span><span class="sxs-lookup"><span data-stu-id="bca35-104">You can quickly find out what happened or diagnose problems related to user sign-in by using the [Sign-in Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom):</span></span>

1. <span data-ttu-id="bca35-105">Palaidiet pierakstīšanās diagnostiku.</span><span class="sxs-lookup"><span data-stu-id="bca35-105">Launch the Sign-in Diagnostic.</span></span>
1. <span data-ttu-id="bca35-106">Meklēšanas notikuma atrašana, ievadot detalizētu informāciju par lietotāju, lietojumprogrammu, pierakstīšanās, pieprasījuma ID vai korelācijas ID.</span><span class="sxs-lookup"><span data-stu-id="bca35-106">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="bca35-107">Pārskatiet diagnostikas rezultātus, parādot detalizētu informāciju par to, kas noticis un kādas darbības varat veikt, lai veiktu izmaiņas (ja nepieciešamas izmaiņas).</span><span class="sxs-lookup"><span data-stu-id="bca35-107">Review the diagnostic results showing the details of what happened and what actions you can take to make changes (if any changes are needed).</span></span>

<span data-ttu-id="bca35-108">**Darbības, kas jāveic, lai novērstu pierakstīšanos**</span><span class="sxs-lookup"><span data-stu-id="bca35-108">**Steps to Troubleshoot a Sign-In**</span></span> 

1. <span data-ttu-id="bca35-109">Pārejiet uz Azure AD pierakstīšanās lapu.</span><span class="sxs-lookup"><span data-stu-id="bca35-109">Navigate to the Azure AD Sign-in page.</span></span>
1. <span data-ttu-id="bca35-110">Filtrējiet pierakstīšanās pēc lietotāja, laika diapazona, lietojumprogrammas, statusa, klienta lietojumprogrammas un tā tālāk.</span><span class="sxs-lookup"><span data-stu-id="bca35-110">Filter sign-ins by user, time range, application, status, client app, and so on.</span></span>
1. <span data-ttu-id="bca35-111">Atlasiet pierakstīšanās notikumu un skatiet cilni nosacījuma piekļuve, lai skatītu, kuras politikas ir novērtētas.</span><span class="sxs-lookup"><span data-stu-id="bca35-111">Select a sign-in event and view the Conditional Access tab to see which policies were evaluated.</span></span>
1. <span data-ttu-id="bca35-112">Noklikšķiniet uz politikas rindas, lai skatītu detalizētu informāciju par politiku un saprastu, kāpēc tā tiek lietota.</span><span class="sxs-lookup"><span data-stu-id="bca35-112">Click on the row of a policy to view the policy details and understand why it applied.</span></span>

<span data-ttu-id="bca35-113">**Rīki, kas novērš nosacījuma piekļuves politiku**</span><span class="sxs-lookup"><span data-stu-id="bca35-113">**Tools to troubleshoot a Conditional Access policy**</span></span>

- <span data-ttu-id="bca35-114">Tikai atskaišu režīms ļauj novērtēt politiku, neietekmējot lietotājus.</span><span class="sxs-lookup"><span data-stu-id="bca35-114">Report-only mode lets you evaluate a policy without impacting users.</span></span>
- <span data-ttu-id="bca35-115">Iespēju rīks ļauj simulēt pierakstīšanās notikumus un skatīt, kuras politikas tiek lietotas.</span><span class="sxs-lookup"><span data-stu-id="bca35-115">What-if tool lets you simulate sign-in events and see which policies apply.</span></span>
- <span data-ttu-id="bca35-116">Ieskatu un ziņošanas darbgrāmatā parāda katras politikas reāllaika ietekmi.</span><span class="sxs-lookup"><span data-stu-id="bca35-116">Insights and reporting workbook displays real-time impact of each policy.</span></span>

<span data-ttu-id="bca35-117">**Bāzlīnijas aizsardzības politikas**</span><span class="sxs-lookup"><span data-stu-id="bca35-117">**Baseline Protection Policies**</span></span>

<span data-ttu-id="bca35-118">Pamata aizsardzības politika ir novecojusi.</span><span class="sxs-lookup"><span data-stu-id="bca35-118">Baseline Protection policies have been deprecated.</span></span> <span data-ttu-id="bca35-119">Tie vairs netiek ieviesti un drīzumā tiks noņemti no Azure portāla.</span><span class="sxs-lookup"><span data-stu-id="bca35-119">They are no longer being enforced and will soon be removed from Azure portal.</span></span> <span data-ttu-id="bca35-120">Iesakām iespējot [drošības noklusējumus](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span><span class="sxs-lookup"><span data-stu-id="bca35-120">We recommend enabling [security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults).</span></span>

<span data-ttu-id="bca35-121">Papildinformāciju par ierobežotu piekļuvi skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="bca35-121">For more information on Conditional Access see:</span></span>

<span data-ttu-id="bca35-122">[Labākā prakse nosacījuma piekļuvei Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Nosacījuma piekļuves nosacījumi](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices)  
 [Ierobežotas piekļuves vadīklas](https://docs.microsoft.com/azure/active-directory/conditional-access/controls)  
 [Ierobežotas piekļuves atrašanās vietas](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span><span class="sxs-lookup"><span data-stu-id="bca35-122">[Best practices for conditional access in Azure Active Directory](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Conditions in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/best-practices) 
[Controls in Conditional Access](https://docs.microsoft.com/azure/active-directory/conditional-access/controls) 
[Locations in Conditional Access ](https://docs.microsoft.com/azure/active-directory/conditional-access/location-condition)</span></span>
