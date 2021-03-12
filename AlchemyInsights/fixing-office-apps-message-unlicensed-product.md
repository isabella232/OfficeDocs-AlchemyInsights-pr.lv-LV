---
title: Nevar aktivizēt Office
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "2000023"
- "3509"
ms.openlocfilehash: 3a42c221047e7be6a173694cd45136baa6bff39a
ms.sourcegitcommit: 0eb4f9bde53395b5fd4b5cd4ffc56ca96db91298
ms.translationtype: HT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/10/2021
ms.locfileid: "50704937"
---
# <a name="unable-to-activate-office"></a><span data-ttu-id="72f9f-102">Nevar aktivizēt Office</span><span class="sxs-lookup"><span data-stu-id="72f9f-102">Unable to activate Office</span></span>

- <span data-ttu-id="72f9f-103">Pārbaudiet, vai nav beidzies jūsu abonements.</span><span class="sxs-lookup"><span data-stu-id="72f9f-103">Check if your subscription status has expired.</span></span>
- <span data-ttu-id="72f9f-104">Pārliecinieties, vai jums ir abonements, kas atļauj klienta licences, piemēram, Office 365 Business vai Business Premium, un [nodrošiniet, ka lietotājam ir piešķirta licence](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="72f9f-104">Ensure you have a subscription that allows client licenses, such as Office 365 Business or Business Premium, and [ensure the user has a license assigned](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users?view=o365-worldwide).</span></span>
- <span data-ttu-id="72f9f-105">Pārliecinieties, ka lietotājs pierakstās Office ar kontu, kuram piešķirta licence.</span><span class="sxs-lookup"><span data-stu-id="72f9f-105">Ensure the user is signing into Office with the same account that has the license assigned.</span></span>
- <span data-ttu-id="72f9f-106">Pārbaudiet lapu [Office 365 pakalpojumu darbspēja](https://docs.microsoft.com/office365/enterprise/view-service-health), lai uzzinātu, vai pastāv zināmas problēmas ar pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="72f9f-106">Check the [Office 365 Service Health page](https://docs.microsoft.com/office365/enterprise/view-service-health) to see if there are any known problems with the service.</span></span>
- <span data-ttu-id="72f9f-107">Pārbaudiet savu ugunsmūri, pretvīrusu programmatūru un starpniekservera iestatījumus, lai pārliecinātos, ka tie nebloķē Microsoft 365 lietojumprogrammu piekļuvi internetam.</span><span class="sxs-lookup"><span data-stu-id="72f9f-107">Check your firewall, antivirus software and proxy settings to confirm that they are not blocking Microsoft 365 apps access to the internet.</span></span> <span data-ttu-id="72f9f-108">Lūdzu, skatiet [Office 365 vietrāžu URL un IP adrešu diapazoni](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 vietrāžu URL un IP adreses diapazoni").</span><span class="sxs-lookup"><span data-stu-id="72f9f-108">Please see [Office 365 URLs and IP address ranges](https://docs.microsoft.com/office365/enterprise/urls-and-ip-address-ranges "Office 365 URLs and IP address ranges").</span></span>

<span data-ttu-id="72f9f-109">**Padoms** Windows datoros mēs varam diagnosticēt un automātiski risināt vairākas bieži sastopamas Office pierakstīšanās problēmas.</span><span class="sxs-lookup"><span data-stu-id="72f9f-109">**Tip** On Windows machines, we can diagnose and automatically fix several common Office sign-in issues for you.</span></span> <span data-ttu-id="72f9f-110">Lejupielādējiet un palaidiet  **[Microsoft atbalsta un atkopšanas palīgu](https://aka.ms/SaRA-OfficeSignInScenario)**, lai izmantotu mūsu automatizēto rīku.</span><span class="sxs-lookup"><span data-stu-id="72f9f-110">Download and run the  **[Microsoft Support and Recovery Assistant](https://aka.ms/SaRA-OfficeSignInScenario)** to use our automated tool.</span></span>

<span data-ttu-id="72f9f-111">Veiciet tālāk aprakstītās darbības problēmu novēršanai.</span><span class="sxs-lookup"><span data-stu-id="72f9f-111">Use the following troubleshooting actions:</span></span>

- <span data-ttu-id="72f9f-112">Atveriet Office lietojumprogrammu un [izrakstieties](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) no visiem lietotāju kontiem.</span><span class="sxs-lookup"><span data-stu-id="72f9f-112">Open an Office app, and [sign out](https://support.office.com/article/5a20dc11-47e9-4b6f-945d-478cb6d92071) of any existing user accounts.</span></span> <span data-ttu-id="72f9f-113">[Noņemiet](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) un [atkārtoti piešķiriet](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office licenci, un pēc tam [pierakstieties Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) ar attiecīgā lietotāja kontu.</span><span class="sxs-lookup"><span data-stu-id="72f9f-113">[Remove](https://docs.microsoft.com/microsoft-365/admin/manage/remove-licenses-from-users) and [re-assign](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) Office license, and then [sign into Office](https://support.office.com/article/628ea040-f265-49de-b986-be09c3ebf8a9) using the affected user account.</span></span>
- <span data-ttu-id="72f9f-114">Palaidiet [aktivācijas problēmu risinātāju](https://aka.ms/SARA-OfficeActivation-Alchemy)</span><span class="sxs-lookup"><span data-stu-id="72f9f-114">Run the [Activation Troubleshooter](https://aka.ms/SARA-OfficeActivation-Alchemy)</span></span>
- [<span data-ttu-id="72f9f-115">Atiestatiet Office aktivācijas stāvokli</span><span class="sxs-lookup"><span data-stu-id="72f9f-115">Reset Office activation state</span></span>](https://docs.microsoft.com/office365/troubleshoot/activation/reset-office-365-proplus-activation-state "Atiestatiet Office aktivācijas stāvokli")
- [<span data-ttu-id="72f9f-116">Veiciet Office tiešsaistes labošanu</span><span class="sxs-lookup"><span data-stu-id="72f9f-116">Perform an Online Repair of Office</span></span>](https://support.office.com/Article/7821d4b6-7c1d-4205-aa0e-a6b40c5bb88b?wt.mc_id=Alchemy_ClientDIA)

<span data-ttu-id="72f9f-117">Papildu problēmu novēršanas risinājumus skatiet šeit:</span><span class="sxs-lookup"><span data-stu-id="72f9f-117">For additional troubleshooting solutions, see:</span></span>  

- [<span data-ttu-id="72f9f-118">Nelicencēts produkts un aktivizācijas kļūdas sistēmā Office</span><span class="sxs-lookup"><span data-stu-id="72f9f-118">Unlicensed Product and activation errors in Office</span></span>](https://support.office.com/Article/0d23d3c0-c19c-4b2f-9845-5344fedc4380?wt.mc_id=Alchemy_ClientDIA)
- [<span data-ttu-id="72f9f-119">Office aktivācijas laikā tiek parādīts kļūdas ziņojums: “Atvainojamies, bet mēs nevaram pieslēgties jūsu kontam. Lūdzu, mēģiniet vēlāk."kļūda, aktivizējot Office”</span><span class="sxs-lookup"><span data-stu-id="72f9f-119">"Sorry, we can't connect to your account. Please try again later" error when you activate Office</span></span>](https://docs.microsoft.com/office/troubleshoot/activation-installation/issue-when-activate-office-from-office-365)