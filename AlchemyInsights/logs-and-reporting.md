---
title: Žurnāli un ziņošana
ms.author: v-jmathew
author: v-jmathew
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9004331"
- "7727"
ms.openlocfilehash: 7349efb02f8d6ac5d73f6d6cd06eef6308ffe9be
ms.sourcegitcommit: 117c64e1fbcb5eec04f94eadad71423b974e7b14
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 01/27/2021
ms.locfileid: "50036005"
---
# <a name="logs-and-reporting"></a><span data-ttu-id="23635-102">Žurnāli un ziņošana</span><span class="sxs-lookup"><span data-stu-id="23635-102">Logs and Reporting</span></span>

<span data-ttu-id="23635-103">[Azure Active Directory atskaišu izveides biežāk](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) uzdotie jautājumi par pakalpojumu Azure Active Directory (Azure AD).</span><span class="sxs-lookup"><span data-stu-id="23635-103">[Azure Active Directory reporting FAQ](https://docs.microsoft.com/azure/active-directory/active-directory-reporting-faq) answers frequently asked questions about Azure Active Directory (Azure AD) reporting.</span></span> <span data-ttu-id="23635-104">Papildinformāciju skatiet rakstā [Azure Active Directory atskaišu](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports)izveide.</span><span class="sxs-lookup"><span data-stu-id="23635-104">For more information, see [Azure Active Directory reporting](https://docs.microsoft.com/azure/active-directory/reports-monitoring/overview-reports).</span></span>

<span data-ttu-id="23635-105">**Problēmu novēršana saistībā ar auditu**</span><span class="sxs-lookup"><span data-stu-id="23635-105">**Troubleshooting issues with Audit**</span></span>

1. <span data-ttu-id="23635-106">Ja rodas problēmas saistībā ar audita darbībām un trūkstošajām darbībām ir šajā [sarakstā](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), lūdzu, iesniedziet atbalsta biļeti.</span><span class="sxs-lookup"><span data-stu-id="23635-106">If you are having issues seeing some audit activities and the missing Activity is in this [list](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-audit-activities), please file a support ticket.</span></span>
2. <span data-ttu-id="23635-107">Ja jums ir problēmas ar visiem jūsu nomnieka audita žurnāliem, lūdzu, iesniedziet atbalsta biļeti.</span><span class="sxs-lookup"><span data-stu-id="23635-107">If you are having issues seeing any Audit logs in your tenant, please file a support ticket.</span></span>
3. <span data-ttu-id="23635-108">Ja jūsu audita darbības neparādās tieši Azure portālā, skatiet mūsu [latentuma informāciju](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) un iesniedziet atbalsta biļeti, ja aizkave pārsniedz dokumentēto latentumu.</span><span class="sxs-lookup"><span data-stu-id="23635-108">If your audit activities are not showing up immediately in the Azure Portal, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. [<span data-ttu-id="23635-109">Azure AD darbību žurnālu saglabāšana</span><span class="sxs-lookup"><span data-stu-id="23635-109">Azure AD Activity Logs Retention</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-data-retention)
5. <span data-ttu-id="23635-110">Ja neredzat visu atlasīto datumu diapazona auditu, varat lejupielādēt līdz pat 250 000 rindu (kārtotas pēc pēdējiem) no Azure portāla pierakstīšanās.</span><span class="sxs-lookup"><span data-stu-id="23635-110">If you don't see all the audit for the date range you selected, you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="23635-111">Papildinformāciju skatiet rakstā [audita darbību lejupielāde](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span><span class="sxs-lookup"><span data-stu-id="23635-111">For more information, see [Audit activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/quickstart-download-audit-report).</span></span>

<span data-ttu-id="23635-112">**Ar pierakstīšanos saistītu problēmu novēršana**</span><span class="sxs-lookup"><span data-stu-id="23635-112">**Troubleshooting issues with Sign-ins**</span></span>

1. <span data-ttu-id="23635-113">Jūs varat redzēt tikai pēdējo 30 datu dienu, ja jums ir jūsu nomnieka Azure AD Premium (P1 vai P2) licence.</span><span class="sxs-lookup"><span data-stu-id="23635-113">You can only see the last 30 days of data if you have an Azure AD Premium (P1 or P2) license for your tenant.</span></span>
2. <span data-ttu-id="23635-114">Pierakstīšanās programmas ir pieejamas tikai Azure AD Premium nomniekiem.</span><span class="sxs-lookup"><span data-stu-id="23635-114">Sign-ins are available only for Azure AD Premium tenants.</span></span> <span data-ttu-id="23635-115">Tas nav pieejams bezmaksas vai pamata licencētiem nomniekiem.</span><span class="sxs-lookup"><span data-stu-id="23635-115">It's not available for Free or Basic licensed tenants.</span></span>
3. <span data-ttu-id="23635-116">Ja jūsu nomniekam ir Premium P1 licence un jūs nevarat redzēt pierakstīšanās iespējas, skatiet mūsu [latentuma informāciju](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) un iesniedziet atbalsta biļeti, ja aizkave pārsniedz dokumentēto latentumu.</span><span class="sxs-lookup"><span data-stu-id="23635-116">If your tenant has a Premium P1 license and you can't see the sign-ins, check out our [latency information](https://docs.microsoft.com/azure/active-directory/reports-monitoring/reference-reports-latencies) and file a support ticket if the delay exceeds the documented latency.</span></span>
4. <span data-ttu-id="23635-117">Ja neredzat visus pierakstīšanās datus atlasītajā datumu diapazonā, ņemiet vērā, ka jūs varat lejupielādēt līdz 250 000 rindu (tiek kārtots pēc pēdējiem) no Azure portāla pierakstīšanās.</span><span class="sxs-lookup"><span data-stu-id="23635-117">If you don't see all the sign-ins for the date range you selected, note that you can download up to 250K rows (sorted by most recent) of sign-ins from Azure portal.</span></span> <span data-ttu-id="23635-118">Papildinformāciju skatiet rakstā [pierakstīšanās darbību lejupielāde](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span><span class="sxs-lookup"><span data-stu-id="23635-118">For more information, see [Sign-ins activities download](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-sign-ins#download-sign-in-activities).</span></span>

<span data-ttu-id="23635-119">**Drošības pārskatu problēmu novēršana (lietotāji, kuri ir atzīmēti kā riski, bīstami pierakstīšanās)**</span><span class="sxs-lookup"><span data-stu-id="23635-119">**Troubleshoot Security Reports (Users Flagged at Risk, Risky Sign-In)**</span></span>

1. [<span data-ttu-id="23635-120">Lietotāji, kuriem ir atzīmēts riska drošības pārskats</span><span class="sxs-lookup"><span data-stu-id="23635-120">Users flagged for risk security report</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-user-at-risk)
2. [<span data-ttu-id="23635-121">Bīstamās pierakstīšanās atskaite Azure Active Directory portālā</span><span class="sxs-lookup"><span data-stu-id="23635-121">Risky sign-ins report in the Azure Active Directory portal</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risky-sign-ins)
3. [<span data-ttu-id="23635-122">Azure Active Directory riska notikumi</span><span class="sxs-lookup"><span data-stu-id="23635-122">Azure Active Directory risk events</span></span>](https://docs.microsoft.com/azure/active-directory/reports-monitoring/concept-risk-events)
