---
title: Autentifikācijas programma
ms.author: v-aiyengar
author: AshaIyengar21
manager: dansimp
ms.date: 03/24/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9003252"
- "9909"
ms.openlocfilehash: 67331a9661ee67c4a861feb1a4292255a4d37133
ms.sourcegitcommit: db908b3da2c7a6508a77bf4f2c80afb294fadbd1
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/29/2021
ms.locfileid: "51405065"
---
# <a name="authentication-app"></a><span data-ttu-id="7f863-102">Autentifikācijas programma</span><span class="sxs-lookup"><span data-stu-id="7f863-102">Authentication app</span></span>

<span data-ttu-id="7f863-103">Ja esat globālais administrators, varat ātri uzzināt, kas noticis vai diagnosticētas problēmas saistībā ar lietotāju pierakstīšanu, izmantojot pierakstīšanās [diagnostiku.](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="7f863-103">If you are a Global Admin, you can quickly find out what happened or diagnose problems related to user-sign in by using the [Sign-in Diagnostics](https://ms.portal.azure.com/microsoft.onmicrosoft.com?loginHint=shhada@microsoft.com#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>

1. <span data-ttu-id="7f863-104">Sāciet diagnostiku, noklikšķinot uz[pogas "Palaist diagnostiku".](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="7f863-104">Start the diagnostics by clicking "[Launch Diagnostic](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)" button.</span></span> 
1. <span data-ttu-id="7f863-105">Atrodiet analizējamu notikumu, ievadot detalizētu informāciju par lietotāju, lietojumprogrammu, pierakstīšanās laiku, pieprasījuma ID vai korelācijas ID.</span><span class="sxs-lookup"><span data-stu-id="7f863-105">Find the event to analyze by entering in the details you have about the user, application, time of sign-in, request Id, or correlation Id.</span></span>
1. <span data-ttu-id="7f863-106">Pārskatiet diagnostikas rezultātus, parādot detalizētu informāciju par to, kas noticis, un kādas darbības varat veikt, lai veiktu izmaiņas, ja ir nepieciešamas kādas izmaiņas.</span><span class="sxs-lookup"><span data-stu-id="7f863-106">Review the diagnostic results showing the details of what happened and what actions you can take to make changes, if any changes are needed.</span></span>

<span data-ttu-id="7f863-107">**Skatiet attiecināmo scenāriju:**</span><span class="sxs-lookup"><span data-stu-id="7f863-107">**Check the scenario that is applicable:**</span></span>

1. <span data-ttu-id="7f863-108">Ja lietotājs nesaņem pašpiegādes paziņojumu programmā Microsoft Authenticator, pārbaudiet, vai tie netiek rādīti MFA bloķēto lietotāju sarakstā, kā aprakstīts rakstā Lietotāju bloķēšana [un atbloķēšana.](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom)</span><span class="sxs-lookup"><span data-stu-id="7f863-108">If a user is not getting a push notification in the Microsoft Authenticator app, verify they are not shown under the MFA blocked users as described in [Block and unblock users](https://portal.azure.com/#blade/Microsoft_AAD_IAM/ActiveDirectoryMenuBlade/diagnose/symptomId/ms_aad_dxp_signin_caDiagnoseAndSolveSummarySymptom).</span></span>
1. <span data-ttu-id="7f863-109">Ja lietotājs nav bloķēts MFA, bet nesaņem pašpiegādes paziņojumu, viņš var atvērt programmu Microsoft Authenticator, kas izvilks gaidošos apstiprināšanas pieprasījumus.</span><span class="sxs-lookup"><span data-stu-id="7f863-109">If the user is not blocked for MFA but does not receive a push notification, they can open the Microsoft Authenticator app, which will pull the pending approval requests.</span></span>
1. <span data-ttu-id="7f863-110">Kā alternatīvu pierakstīšanās metodi lietotājs var arī noklikšķināt uz Pierakstīties citā veidā un izvēlēties izmantot pārbaudes kodu manā mobilajā lietojumprogrammā.</span><span class="sxs-lookup"><span data-stu-id="7f863-110">As an alternative sign-in method, the user can also click on Sign in another way and choose use a verification code from my mobile app.</span></span>
1. <span data-ttu-id="7f863-111">Programma Microsoft Authenticator ir vienīgā pieejamā metode daudziem lietotājiem.</span><span class="sxs-lookup"><span data-stu-id="7f863-111">The Microsoft Authenticator App is the only available method for many users.</span></span> <span data-ttu-id="7f863-112">[Uzziniet vairāk par drošības noklusējumus](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults)— skatiet bieži uzdotos jautājumus par autentificētāja lietojumprogrammu — bieži uzdotos jautājumus un to atrisināšanu. [](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq)</span><span class="sxs-lookup"><span data-stu-id="7f863-112">[Learn more about security defaults](https://docs.microsoft.com/azure/active-directory/fundamentals/concept-fundamentals-security-defaults), check [Authenticator App FAQ](https://docs.microsoft.com/azure/active-directory/user-help/user-help-auth-app-faq) for commonly asked questions and how to resolve them.</span></span>
 
<span data-ttu-id="7f863-113">**Ieteicamie video**</span><span class="sxs-lookup"><span data-stu-id="7f863-113">**Recommended Videos**</span></span>

<span data-ttu-id="7f863-114">[Kā iestatīt programmu Authenticator jaunā tālrunī (2min).](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409)</span><span class="sxs-lookup"><span data-stu-id="7f863-114">[How to set up Authenticator App on a new phone (2min)](https://go.microsoft.com/fwlink/?linkid=2158163&clcid=0x409).</span></span>
