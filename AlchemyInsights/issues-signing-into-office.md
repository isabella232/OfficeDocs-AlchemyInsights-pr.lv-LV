---
title: Problēmas ar pierakstīšanos Microsoft 365 programmās
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 02841a1b4e92eec94fc6409941d91618f02518c1
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51836610"
---
# <a name="issues-signing-into-microsoft-365-apps"></a><span data-ttu-id="00832-102">Problēmas ar pierakstīšanos Microsoft 365 programmās</span><span class="sxs-lookup"><span data-stu-id="00832-102">Issues signing into Microsoft 365 Apps</span></span>

<span data-ttu-id="00832-103">Lai novērstu pierakstīšanās problēmas ar Microsoft 365 programmām, attiecīgajā datorā izmēģiniet šādas opcijas:</span><span class="sxs-lookup"><span data-stu-id="00832-103">To fix sign-in issues with Microsoft 365 apps, try the following options on the affected machine:</span></span>  

- <span data-ttu-id="00832-104">Operētājsistēmai Windows skatiet [rakstu Ieteikumi bieži sastopamu pierakstīšanās problēmu novēršanai](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span><span class="sxs-lookup"><span data-stu-id="00832-104">For Windows, see [Recommendations on resolving common sign-in issues](https://docs.microsoft.com/office365/troubleshoot/administration/disabling-adal-wam-not-recommended#recommendations-on-resolving-common-sign-in-issues)</span></span>
- <span data-ttu-id="00832-105">Ja jums ir Mac dators,  [skatiet rakstu Nevar pierakstīties lietojumprogrammā Office 2016 for Mac](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span><span class="sxs-lookup"><span data-stu-id="00832-105">For Mac, see  [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail)</span></span>

<span data-ttu-id="00832-106">**Padoms** Windows datoros mēs varam diagnosticēt un automātiski risināt vairākas bieži sastopamas Office pierakstīšanās problēmas.</span><span class="sxs-lookup"><span data-stu-id="00832-106">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="00832-107">Lejupielādējiet un palaidiet  **[Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA-OfficeSignInScenario)**, lai izmantotu mūsu automatizēto rīku.</span><span class="sxs-lookup"><span data-stu-id="00832-107">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="00832-108">**Piezīme.** Nav ieteicams atspējot moderno autentifikāciju (ADAL) vai tīmekļa konta pārvaldību (Web Account Management — WAM), lai labotu pierakstīšanās **vai aktivizācijas problēmas.**</span><span class="sxs-lookup"><span data-stu-id="00832-108">**Note:** Disabling Modern Authentication (ADAL) or Web Account Management (WAM) for fixing sign-in or activation issues  **is not recommended**.</span></span> <span data-ttu-id="00832-109">Ja, veidojot savienojumu ar Microsoft 365, izmantojot Office 2013, rodas kļūdas, pārliecinieties, vai [Office](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  klientam iespējojat moderno autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="00832-109">If the errors occur while connecting to Microsoft 365 using Office 2013, ensure that you [enable modern authentication](https://docs.microsoft.com/microsoft-365/admin/security-and-compliance/enable-modern-authentication)  for Office client.</span></span>

<span data-ttu-id="00832-110">Konkrētas problēmu novēršanas darbības skatiet tālāk redzamajā rakstā.</span><span class="sxs-lookup"><span data-stu-id="00832-110">For specific troubleshooting actions, see:</span></span>

[<span data-ttu-id="00832-111">Savienojuma problēmas pierakstoties pēc atjaunināšanas uz Office 2016 būvējumu 16.0.7967 operētājsistēmā Windows 10</span><span class="sxs-lookup"><span data-stu-id="00832-111">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)  

[<span data-ttu-id="00832-112">Nevarat pierakstīties savā organizācijas kontā, piemēram, Office 365, Azure vai Intune</span><span class="sxs-lookup"><span data-stu-id="00832-112">You can't sign in to your organizational account such as Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)

[<span data-ttu-id="00832-113">Kā novērst problēmas, kas nav saistītas ar lietojumprogrammām, kas nav pārlūkprogrammas un nevar pierakstīties pakalpojumā Office 365, Azure vai Intune</span><span class="sxs-lookup"><span data-stu-id="00832-113">How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune</span></span>](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1?ui=en-US&rs=en-US&ad=US)

[<span data-ttu-id="00832-114">Atkārtoti tiek prasīti akreditācijas dati sistēmā Office</span><span class="sxs-lookup"><span data-stu-id="00832-114">Repeatedly prompted for credentials in Office</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/access-denied-when-connect-to-office-365)