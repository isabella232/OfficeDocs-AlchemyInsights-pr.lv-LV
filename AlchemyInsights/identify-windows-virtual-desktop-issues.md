---
title: Windows virtuālās darbvirsmas problēmu identificēšana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O364
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: 1e55d9d579c389dfe731f887a2a08c6234de2787
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595852"
---
# <a name="identify-windows-virtual-desktop-issues"></a><span data-ttu-id="57efb-102">Windows virtuālās darbvirsmas problēmu identificēšana</span><span class="sxs-lookup"><span data-stu-id="57efb-102">Identify Windows Virtual Desktop issues</span></span>

<span data-ttu-id="57efb-103">Windows virtuālās darbvirsmas diagnostika izmanto tikai vienu PowerShell cmdlet, bet tajā ir daudz neobligātu parametru, lai sašaurinātu un izolētu problēmas.</span><span class="sxs-lookup"><span data-stu-id="57efb-103">Windows Virtual Desktop Diagnostics uses just one PowerShell cmdlet but contains many optional parameters to help narrow down and isolate issues.</span></span> <span data-ttu-id="57efb-104">Lai sāktu darbu:</span><span class="sxs-lookup"><span data-stu-id="57efb-104">To get started:</span></span> 

1. <span data-ttu-id="57efb-105">Lejupielādējiet un importējiet Windows virtuālās darbvirsmas PowerShell moduli.</span><span class="sxs-lookup"><span data-stu-id="57efb-105">Download and import the Windows Virtual Desktop PowerShell module.</span></span> <span data-ttu-id="57efb-106">Detalizētu informāciju skatiet rakstā [Windows virtuālās darbvirsmas cmdlet čaulai Windows PowerShell.](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview)</span><span class="sxs-lookup"><span data-stu-id="57efb-106">For details, see [Windows Virtual Desktop Cmdlets for Windows PowerShell](https://docs.microsoft.com/powershell/windows-virtual-desktop/overview).</span></span>

1. <span data-ttu-id="57efb-107">Lai pierakstītos savā kontā, palaidiet šādu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="57efb-107">Run the following cmdlet to sign in to your account:</span></span>
    
    <span data-ttu-id="57efb-108">Piemērs: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span><span class="sxs-lookup"><span data-stu-id="57efb-108">Example: `Add-RdsAccount -DeploymentUrl 'https://rdbroker.wvd.microsoft.com'`</span></span>

<span data-ttu-id="57efb-109">**PIEZĪME.** Visos vaicājumos, izmantojot PowerShell, ir jāiekļauj parametri -UserName vai -ActivityID.</span><span class="sxs-lookup"><span data-stu-id="57efb-109">**NOTE:** All queries using PowerShell must include either the -UserName or -ActivityID parameters.</span></span> <span data-ttu-id="57efb-110">Informāciju par pārraudzības iespējām skatiet rakstā [Žurnālu analīzes izmantošana diagnostikas līdzeklim.](https://go.microsoft.com/fwlink/?linkid=2126847)</span><span class="sxs-lookup"><span data-stu-id="57efb-110">For monitoring capabilities, see Use [Log Analytics for the diagnostics feature](https://go.microsoft.com/fwlink/?linkid=2126847).</span></span>

<span data-ttu-id="57efb-111">Lai filtrētu diagnostikas darbības pēc lietotāja, palaidiet šādu cmdlet:</span><span class="sxs-lookup"><span data-stu-id="57efb-111">To filter diagnostic activities by user, run the following cmdlet:</span></span>

<span data-ttu-id="57efb-112">Piemērs: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span><span class="sxs-lookup"><span data-stu-id="57efb-112">Example: `Get-RdsDiagnosticActivities -TenantName < tenantName > -UserName < UserUPN >`</span></span>

<span data-ttu-id="57efb-113">Ir pieejams saraksts ar filtriem, kurus varat palaist, lai diagnosticētu problēmas.</span><span class="sxs-lookup"><span data-stu-id="57efb-113">There is a list of filters you can run to diagnose issues.</span></span> <span data-ttu-id="57efb-114">Papildinformāciju par problēmu diagnosticēšanu skatiet rakstā [Windows virtuālās darbvirsmas problēmu identificēšana un diagnosticēšana.](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell)</span><span class="sxs-lookup"><span data-stu-id="57efb-114">To learn more about diagnosing issues, see [Identify and diagnose Windows Virtual Desktop issues](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#diagnose-issues-with-powershell).</span></span>

<span data-ttu-id="57efb-115">Papildinformāciju par biežāk sastopamajām kļūdām skatiet [rakstā Bieži sastopamās kļūdas](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span><span class="sxs-lookup"><span data-stu-id="57efb-115">To learn more about common errors, see [Common errors senarios](https://docs.microsoft.com/azure/virtual-desktop/diagnostics-role-service#common-error-scenarios).</span></span>
