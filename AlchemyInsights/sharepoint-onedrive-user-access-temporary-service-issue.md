---
title: Veiktspējas problēmas — SharePoint vai OneDrive
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 39ec9b746c47414f1cfaad1342491b8f33a47d6f
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47771251"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="4fd3d-102">SharePoint vai OneDrive lēna, nepieejama vai nepieejama vairākiem lietotājiem</span><span class="sxs-lookup"><span data-stu-id="4fd3d-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="4fd3d-103">Ja OneDrive vai SharePoint vietne nav pieejama vairākiem lietotājiem, kuriem agrāk bija piekļuve, iespējama īslaicīga pakalpojumu problēma.</span><span class="sxs-lookup"><span data-stu-id="4fd3d-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="4fd3d-104">[Skatiet pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="4fd3d-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

<span data-ttu-id="4fd3d-105">**Pievienojiet lietotāju un licencējiet to.**</span><span class="sxs-lookup"><span data-stu-id="4fd3d-105">**Add and license the user**</span></span>

<span data-ttu-id="4fd3d-106">Pārliecinieties, vai jums ir [piešķirtas licences lietotājiem pakalpojumā Microsoft 365 darbam](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="4fd3d-106">Ensure that you [Assign licenses to users in Microsoft 365 for business](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span>


<span data-ttu-id="4fd3d-107">**Atļauju piešķiršana**</span><span class="sxs-lookup"><span data-stu-id="4fd3d-107">**Assign Permissions**</span></span>

<span data-ttu-id="4fd3d-108">Ja lietotājam ir piešķirta SharePoint licence un joprojām tiek saņemts ziņojums par liegtu piekļuvi, pārliecinieties, vai tiem ir piešķirts [atbilstošs atļauju līmenis](https://docs.microsoft.com/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="4fd3d-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/sharepoint/understanding-permission-levels) assigned.</span></span>

<span data-ttu-id="4fd3d-109">**Piekļuves pieprasījuma līdzekļa izmantošanas apsvēršana**</span><span class="sxs-lookup"><span data-stu-id="4fd3d-109">**Consider using the access request feature**</span></span>

<span data-ttu-id="4fd3d-110">[Piekļuves pieprasījuma līdzeklis](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) ļauj lietotājiem pieprasīt piekļuvi saturam, kuram pašlaik nav atļaujas skatīt.</span><span class="sxs-lookup"><span data-stu-id="4fd3d-110">The [access request feature](https://support.office.com/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

<span data-ttu-id="4fd3d-111">**Atļaut pielāgotā skripta var izraisīt Access denied problēmas**</span><span class="sxs-lookup"><span data-stu-id="4fd3d-111">**Allow custom script may cause access denied issues**</span></span>

<span data-ttu-id="4fd3d-112">Ir daži scenāriji, kuros *Atļaut pielāgotā skripta* līdzekli var būt piekļuve liegta.</span><span class="sxs-lookup"><span data-stu-id="4fd3d-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="4fd3d-113">Attiecīgo līdzekļu saraksts, drošības apsvērumi un iespēja atspējot šo līdzekli.</span><span class="sxs-lookup"><span data-stu-id="4fd3d-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="4fd3d-114">Lūdzu, apmeklējiet sadaļu [Atļaut vai neļaut pielāgot skriptu](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="4fd3d-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/sharepoint/allow-or-prevent-custom-script).</span></span>

