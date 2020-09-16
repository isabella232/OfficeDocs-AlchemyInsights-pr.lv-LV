---
title: Yammer licencēšanas problēmas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: f0a7625c7b77860e5ba0e29f2df47101749aace3
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47657283"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="6cf3c-102">Yammer licencēšanas problēmas</span><span class="sxs-lookup"><span data-stu-id="6cf3c-102">Yammer licensing issues</span></span>

<span data-ttu-id="6cf3c-103">Visiem lietotājiem ir jābūt licencei, lai izmantotu Yammer Enterprise pakalpojumu, bet pēc noklusējuma Yammer neprasa lietotājiem piekļūt pakalpojumam.</span><span class="sxs-lookup"><span data-stu-id="6cf3c-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="6cf3c-104">Ja administrators maina iestatījumu Microsoft 365 lietotāju bloķēšanai bez Yammer licencēm, lietotāji, kuriem nav piešķirtas Yammer Enterprise licences, nevar piekļūt Yammer pakalpojumam.</span><span class="sxs-lookup"><span data-stu-id="6cf3c-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="6cf3c-105">Papildinformāciju skatiet rakstā [Yammer lietotāju licenču pārvaldība pakalpojumā Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="6cf3c-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="6cf3c-106">Ja licences tiek noņemtas no lietotājiem, Yammer elements vairs netiek rādīts, un citi pakalpojumi var izmantot licences noņemšanu, lai paslēptu līdzekļus.</span><span class="sxs-lookup"><span data-stu-id="6cf3c-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="6cf3c-107">Citos gadījumos līdzekļi joprojām var tikt rādīti, taču ir nepieciešama licences piešķiršana darbībai.</span><span class="sxs-lookup"><span data-stu-id="6cf3c-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="6cf3c-108">**Licence lietotājam netiek atjaunināta**</span><span class="sxs-lookup"><span data-stu-id="6cf3c-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="6cf3c-109">Dažkārt lietotājam ir piešķirta licence, bet joprojām nevar piekļūt pakalpojumam Yammer.</span><span class="sxs-lookup"><span data-stu-id="6cf3c-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="6cf3c-110">Aizkaves var rasties, ja notiek masveida licenču piešķiršana.</span><span class="sxs-lookup"><span data-stu-id="6cf3c-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="6cf3c-111">Yammer lietotāji, iespējams, netiek atjaunināti tādā pašā secībā, kā licences tiek mainītas Azure AD, jo sistēma darbojas asinhroni.</span><span class="sxs-lookup"><span data-stu-id="6cf3c-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="6cf3c-112">Pirms atbalsta lietas atvēršanas jāgaida līdz pat 24 stundām, lai ziņotu par licenču sinhronizācijas problēmām.</span><span class="sxs-lookup"><span data-stu-id="6cf3c-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="6cf3c-113">**Lielapjoma licenču piešķiršana**</span><span class="sxs-lookup"><span data-stu-id="6cf3c-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="6cf3c-114">Licences var piešķirt no administrēšanas centra vai PowerShell skriptošanas.</span><span class="sxs-lookup"><span data-stu-id="6cf3c-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="6cf3c-115">Papildinformāciju skatiet rakstā [licenču piešķiršana lietotājiem](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) un [licenču piešķiršana lietotāju kontiem, izmantojot Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="6cf3c-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="6cf3c-116">Microsoft atbalsts nesniedz palīdzību par skriptu izveidi, bet ir pieejama dokumentācija par Yammer licenču piešķiršanu.</span><span class="sxs-lookup"><span data-stu-id="6cf3c-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="6cf3c-117">Papildinformāciju skatiet rakstā [Yammer licenču pārvaldība, izmantojot Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="6cf3c-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>