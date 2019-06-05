---
title: Veiktspējas problēmas-SharePoint vai OneDrive
ms.author: kirks
author: Techwriter40
ms.date: 1/3/2019
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 9225ec0f-771f-4d7a-8157-e188953107aa
ms.openlocfilehash: 3b04e811b69a1f9d652abbd603c3c09df068480c
ms.sourcegitcommit: 6d341637dbb14e90726a1ce1d68f077ace9bb765
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/04/2019
ms.locfileid: "34719523"
---
# <a name="sharepoint-or-onedrive-slow-inaccessible-or-unavailable-for-multiple-users"></a><span data-ttu-id="54232-102">SharePoint vai OneDrive lēni, nav pieejams vai nav pieejams vairākiem lietotājiem</span><span class="sxs-lookup"><span data-stu-id="54232-102">SharePoint or OneDrive Slow, Inaccessible or Unavailable for Multiple Users</span></span>

<span data-ttu-id="54232-103">Ja nav pieejams vairākiem lietotājiem, kas iepriekš bija pieejama OneDrive vai SharePoint vietnē, var būt pagaidu pakalpojumu jautājums.</span><span class="sxs-lookup"><span data-stu-id="54232-103">If a OneDrive or SharePoint site is not available to multiple users who previously had access, there may be a temporary service issue.</span></span> <span data-ttu-id="54232-104">[Pārbaudiet pakalpojumu veselības vadības paneli](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="54232-104">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>

## <a name="add-and-license-the-user"></a><span data-ttu-id="54232-105">Pievienot un licence lietotājam</span><span class="sxs-lookup"><span data-stu-id="54232-105">Add and license the user</span></span>

<span data-ttu-id="54232-106">Nodrošinātu jums [piešķirt licences Office 365 biznesa lietotājiem](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="54232-106">Ensure that you [Assign licenses to users in Office 365 for business](https://docs.microsoft.com/en-us/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span>


## <a name="assign-permissions"></a><span data-ttu-id="54232-107">Piešķirt atļaujas</span><span class="sxs-lookup"><span data-stu-id="54232-107">Assign Permissions</span></span>

<span data-ttu-id="54232-108">Ja lietotājam ir piešķirta Sharepoint licenci un joprojām saņem ziņojumu par liegtu piekļuvi, pārliecinieties, vai tiem ir piešķirts [atbilstošu atļauju līmeni](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) .</span><span class="sxs-lookup"><span data-stu-id="54232-108">If the user has been assigned a Sharepoint license and is still receiving an access denied message, please ensure they have the [appropriate permission level](https://docs.microsoft.com/en-us/sharepoint/understanding-permission-levels) assigned.</span></span>

## <a name="consider-using-the-access-request-feature"></a><span data-ttu-id="54232-109">Apsveriet iespēju izmantot piekļuves pieprasījuma funkcija</span><span class="sxs-lookup"><span data-stu-id="54232-109">Consider using the access request feature</span></span>

<span data-ttu-id="54232-110">[Piekļuves pieprasījuma funkcija](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) ļauj cilvēkiem, lai pieprasītu piekļuvi saturam, kas viņiem pašlaik nav atļaujas skatīt.</span><span class="sxs-lookup"><span data-stu-id="54232-110">The [access request feature](https://support.office.com/en-us/article/Set-up-and-manage-access-requests-94B26E0B-2822-49D4-929A-8455698654B3) allows people to request access to content that they do not currently have permission to see.</span></span>

## <a name="allow-custom-script-may-cause-access-denied-issues"></a><span data-ttu-id="54232-111">Ļautu, pielāgots skripts var izraisīt piekļuves liegšanas problēmas</span><span class="sxs-lookup"><span data-stu-id="54232-111">Allow custom script may cause access denied issues</span></span>

<span data-ttu-id="54232-112">Ir daži scenāriji, kur *Atļaut pielāgota skripta* funkciju var iesniegt par liegtu piekļuvi.</span><span class="sxs-lookup"><span data-stu-id="54232-112">There are certain scenarios where the *Allow custom script* feature may be presenting an access denied.</span></span> <span data-ttu-id="54232-113">Ietekmēto līdzekļu uzskaitījums, drošības apsvērumi un iespēja atspējot šo līdzekli.</span><span class="sxs-lookup"><span data-stu-id="54232-113">For a list of features affected, security considerations and the ability to disable the feature.</span></span> <span data-ttu-id="54232-114">Lūdzu, apmeklējiet [Atļaut vai aizliegt pielāgotu skriptu](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span><span class="sxs-lookup"><span data-stu-id="54232-114">Please visit [Allow or prevent custom script](https://docs.microsoft.com/en-us/sharepoint/allow-or-prevent-custom-script).</span></span>

