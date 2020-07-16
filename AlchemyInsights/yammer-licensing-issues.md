---
title: Yammer licencēšanas problēmas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/14/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "5900"
- "9003071"
ms.openlocfilehash: 6d9b2126dc1ed90968738ddb2e249dce9857f1db
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148313"
---
# <a name="yammer-licensing-issues"></a><span data-ttu-id="2f87f-102">Yammer licencēšanas problēmas</span><span class="sxs-lookup"><span data-stu-id="2f87f-102">Yammer licensing issues</span></span>

<span data-ttu-id="2f87f-103">Visiem lietotājiem ir jābūt licencei izmantot Pakalpojumu Yammer Enterprise, bet pēc noklusējuma Yammer nepieprasa lietotājiem ir licence, lai piekļūtu pakalpojumam.</span><span class="sxs-lookup"><span data-stu-id="2f87f-103">All users must have a license to use the Yammer Enterprise service, but by default Yammer does not require that users have a license to access the service.</span></span> <span data-ttu-id="2f87f-104">Kad administrators maina iestatījumu, lai bloķētu Microsoft 365 lietotājiem bez Yammer licences, lietotājiem nav piešķirta Yammer uzņēmuma licence nevar piekļūt Yammer pakalpojumu.</span><span class="sxs-lookup"><span data-stu-id="2f87f-104">When an administrator changes the setting to block Microsoft 365 users without Yammer licenses, users not assigned a Yammer Enterprise license can't access the Yammer service.</span></span> <span data-ttu-id="2f87f-105">Papildinformāciju skatiet rakstā [Yammer lietotāju licenču pārvaldība pakalpojumā Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span><span class="sxs-lookup"><span data-stu-id="2f87f-105">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365)</span></span> 

<span data-ttu-id="2f87f-106">Kad licences tiek noņemtas no lietotājiem, Yammer elements vairs netiek rādīts un citi pakalpojumi var izmantot licences noņemšanas paslēpt līdzekļus.</span><span class="sxs-lookup"><span data-stu-id="2f87f-106">When licenses are removed from users, the Yammer tile is no longer displayed, and other services can use license removal to hide features.</span></span> <span data-ttu-id="2f87f-107">Citos gadījumos funkcijas joprojām var parādīties, bet pieprasīt licences piešķiršanu, lai darbotos.</span><span class="sxs-lookup"><span data-stu-id="2f87f-107">In other cases, features can still appear but require licence assignment to operate.</span></span>  

<span data-ttu-id="2f87f-108">**Licence nesaņem lietotājam atjauninātu**</span><span class="sxs-lookup"><span data-stu-id="2f87f-108">**License is not getting updated for the user**</span></span>  

<span data-ttu-id="2f87f-109">Reizēm lietotājam tiek piešķirta licence, bet joprojām nevar piekļūt Yammer.</span><span class="sxs-lookup"><span data-stu-id="2f87f-109">Occasionally, a user is assigned a license but is still unable to access Yammer.</span></span> <span data-ttu-id="2f87f-110">Aizkaves, visticamāk, radīsies, ja notiek masveida licences piešķiršana.</span><span class="sxs-lookup"><span data-stu-id="2f87f-110">Delays are more likely to occur when a mass license assignment is in progress.</span></span> <span data-ttu-id="2f87f-111">Yammer lietotāji, iespējams, netiks atjaunināti tādā pašā secībā kā licences tiek mainīti Azure AD, jo sistēma darbojas asinhroni.</span><span class="sxs-lookup"><span data-stu-id="2f87f-111">Yammer users might not be updated in the same order as licenses are changed in Azure AD because the system runs asynchronously.</span></span> <span data-ttu-id="2f87f-112">Uzgaidiet līdz 24 stundām pirms atbalsta pieteikuma atvēršanas, lai ziņotu par licences sinhronizācijas problēmām.</span><span class="sxs-lookup"><span data-stu-id="2f87f-112">Wait up to 24 hours before opening a support case to report license sync issues.</span></span>  

<span data-ttu-id="2f87f-113">**Lielapjoma licenču piešķiršana**</span><span class="sxs-lookup"><span data-stu-id="2f87f-113">**Bulk licence assignment**</span></span>  

<span data-ttu-id="2f87f-114">Licences var piešķirt, izmantojot administrēšanas centru vai PowerShell skriptu.</span><span class="sxs-lookup"><span data-stu-id="2f87f-114">Licenses can be assigned through the admin center or PowerShell scripting.</span></span> <span data-ttu-id="2f87f-115">Papildinformāciju skatiet rakstā [Licenču piešķiršana lietotājiem un Licenču](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) [piešķiršana lietotāju kontiem pakalpojumā Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span><span class="sxs-lookup"><span data-stu-id="2f87f-115">For more info, see [Assign licenses to users](https://docs.microsoft.com/microsoft-365/admin/manage/assign-licenses-to-users) and [Assign licenses to user accounts with Office 365 PowerShell](https://docs.microsoft.com/office365/enterprise/powershell/assign-licenses-to-user-accounts-with-office-365-powershell).</span></span> 

<span data-ttu-id="2f87f-116">Microsoft atbalsts nenodrošina palīdzību skriptu izveidei, bet ir pieejama dokumentācija par Yammer licences piešķiršanu.</span><span class="sxs-lookup"><span data-stu-id="2f87f-116">Microsoft Support does not provide assistance with creating scripts, but documentation on Yammer license assignment is available.</span></span> <span data-ttu-id="2f87f-117">Papildinformāciju skatiet rakstā [Yammer licenču pārvaldība, izmantojot programmu Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span><span class="sxs-lookup"><span data-stu-id="2f87f-117">For more info, see [Manage Yammer licenses by using Windows PowerShell](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365#manage-yammer-licenses-by-using-windows-powershell).</span></span>