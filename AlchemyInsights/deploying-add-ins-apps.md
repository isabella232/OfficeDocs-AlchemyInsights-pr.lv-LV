---
title: Pievienojumprogrammu izvietošana Microsoft 365 programmas
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/30/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "11107"
- "9005477"
ms.openlocfilehash: e55d8e5453f60b5993500dae1eb6efce11a8aa1a
ms.sourcegitcommit: d74039304002e526ba6f8ca02e76e4ce7e1aa743
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/30/2021
ms.locfileid: "52125679"
---
# <a name="deploying-add-ins-for-microsoft-365-apps"></a><span data-ttu-id="10922-102">Pievienojumprogrammu izvietošana Microsoft 365 programmas</span><span class="sxs-lookup"><span data-stu-id="10922-102">Deploying add-ins for Microsoft 365 Apps</span></span>

<span data-ttu-id="10922-103">Centralizētā izvietošana ir ieteicamais veids, Office pievienojumprogrammas izvietot lietotājiem un grupām jūsu organizācijā.</span><span class="sxs-lookup"><span data-stu-id="10922-103">Centralized Deployment is the recommended way for deploying Office add-ins to users and groups within your organization.</span></span> <span data-ttu-id="10922-104">Lai izvietotu pievienojumprogrammas, veiciet tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="10922-104">To deploy add-ins, follow the steps below:</span></span>

<span data-ttu-id="10922-105">**Piezīme.** Lai instalētu pievienojumprogrammas Office kā atsevišķs lietotājs, skatiet rakstu Pievienojumprogrammu skatīšana, pārvaldība un instalēšana [Office programmās.](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d)</span><span class="sxs-lookup"><span data-stu-id="10922-105">**Note:** To install add-ins for Office as an individual user, see [View, manage, and install add-ins in Office programs](https://support.microsoft.com/topic/view-manage-and-install-add-ins-in-office-programs-16278816-1948-4028-91e5-76dca5380f8d).</span></span> <span data-ttu-id="10922-106">Pārliecinieties arī par to, ka ir iespējota Office veikala pievienojumprogrammu iegāde.</span><span class="sxs-lookup"><span data-stu-id="10922-106">Also, make sure that individual acquisition of Office Store add-ins is enabled.</span></span> 

1. <span data-ttu-id="10922-107">Pārliecinieties, vai jūsu vide atbilst prasībām par pievienojumprogrammu izvietošanu, izmantojot centralizēto izvietošanu.</span><span class="sxs-lookup"><span data-stu-id="10922-107">Ensure that your environment meets the requirements for deployment of add-ins using Centralized Deployment.</span></span> <span data-ttu-id="10922-108">Papildinformāciju skatiet [rakstā Prasības](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span><span class="sxs-lookup"><span data-stu-id="10922-108">For details, see [Requirements](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?#requirements).</span></span>
2. <span data-ttu-id="10922-109">Lai **izvietotu Iestatījumi,** dodieties uz sadaļu  >    >   Integrēto lietojumprogrammu iegūšana Microsoft 365 administrēšanas centrā.</span><span class="sxs-lookup"><span data-stu-id="10922-109">Go to **Settings** > **Integrated Apps** > **Get apps** in the Microsoft 365 admin center to deploy add-ins.</span></span> 

<span data-ttu-id="10922-110">Piezīmes.</span><span class="sxs-lookup"><span data-stu-id="10922-110">Notes:</span></span> 

- <span data-ttu-id="10922-111">Integrētajām lietojumprogrammām nepieciešams, lai administratoram būtu globālā administratora Exchange administratora atļaujas.</span><span class="sxs-lookup"><span data-stu-id="10922-111">Integrated Apps requires that the admin has Global Admin or Exchange Admin permissions.</span></span>

- <span data-ttu-id="10922-112">Izvietojot pievienojumprogrammas vairākiem lietotājiem, ieteicams piešķirt uzdevumus, izmantojot grupas, nevis atsevišķus lietotājus.</span><span class="sxs-lookup"><span data-stu-id="10922-112">When deploying add-ins to multiple users, we recommend making assignments by using groups instead of individual users.</span></span> <span data-ttu-id="10922-113">Papildinformāciju [skatiet rakstā Apsvērumi par pievienojumprogrammas piešķiršanu lietotājiem un grupām.](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups)</span><span class="sxs-lookup"><span data-stu-id="10922-113">For details, see [Considerations when assigning an add-in to users and groups](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins?view=o365-worldwide#considerations-when-assigning-an-add-in-to-users-and-groups).</span></span>

- <span data-ttu-id="10922-114">Centralizētā izvietošana neatbalsta lietotājus ligzdotās grupās vai grupās, kam ir vecākgrupas.</span><span class="sxs-lookup"><span data-stu-id="10922-114">Centralized Deployment doesn't support users in nested groups or groups that have parent groups.</span></span> <span data-ttu-id="10922-115">Detalizētu informāciju skatiet rakstā [Lietotāju un grupu piešķiršana.](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments)</span><span class="sxs-lookup"><span data-stu-id="10922-115">For details, see [User and group assignments](https://docs.microsoft.com/microsoft-365/admin/manage/centralized-deployment-of-add-ins?view=o365-worldwide#user-and-group-assignments).</span></span>

- <span data-ttu-id="10922-116">Pārliecinieties, vai Microsoft 365 programmas pārvaldības pakalpojums (GUID: 0517ffae-825d-4aff-999e-3f2336b8a20a) ir iespējots, lai lietotāji varētu pierakstīties.</span><span class="sxs-lookup"><span data-stu-id="10922-116">Ensure that the Microsoft 365 App Management Service (GUID: '0517ffae-825d-4aff-999e-3f2336b8a20a') is enabled for users to sign in.</span></span> <span data-ttu-id="10922-117">Detalizētu informāciju skatiet rakstā [Programmas rekvizītu konfigurēšana.](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties)</span><span class="sxs-lookup"><span data-stu-id="10922-117">For details, see [Configure app properties](https://docs.microsoft.com/azure/active-directory/manage-apps/add-application-portal-configure#configure-app-properties).</span></span>

- <span data-ttu-id="10922-118">Ja, izvietojot pievienojumprogrammas, rodas problēmas, izmantojot integrētās lietojumprogrammas, mēģiniet izvietot, [izmantojot pievienojumprogrammas.](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns)</span><span class="sxs-lookup"><span data-stu-id="10922-118">If you experience issues deploying add-ins by using Integrated Apps, try deploying by using [Add-Ins](https://admin.microsoft.com/AdminPortal/Home?#/Settings/AddIns).</span></span>

<span data-ttu-id="10922-119">Papildinformāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="10922-119">For more information, see:</span></span>

<span data-ttu-id="10922-120">[Pievienojumprogrammu izvietošana administrēšanas centrā](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins) 
 [Pievienojumprogrammu pārvaldība administrēšanas centrā](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center) 
 [Centralizētās izvietošanas PowerShell cmdlet izmantošana pievienojumprogrammu pārvaldīšanai](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins) 
 [Pievienojumprogrammu Office, izmantojot centralizēto izvietošanu, izmantojot Microsoft 365 centru](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment) 
 [Problēmu novēršana: lietotājam netiek rādītas pievienojumprogrammas](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins) 
 [Ar pievienojumprogrammu Office saistīto lietotāju kļūdu novēršana](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span><span class="sxs-lookup"><span data-stu-id="10922-120">[Deploy add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-deployment-of-add-ins)
[Manage add-ins in the admin center](https://docs.microsoft.com/microsoft-365/admin/manage/manage-addins-in-the-admin-center)
[Use the Centralized Deployment PowerShell cmdlets to manage add-ins](https://docs.microsoft.com/microsoft-365/enterprise/use-the-centralized-deployment-powershell-cmdlets-to-manage-add-ins)
[Publish Office Add-ins using Centralized Deployment via the Microsoft 365 admin center](https://docs.microsoft.com/office/dev/add-ins/publish/centralized-deployment#publish-an-office-add-in-via-centralized-deployment)
[Troubleshoot: User not seeing add-ins](https://docs.microsoft.com/office365/troubleshoot/access-management/user-not-seeing-add-ins)
[Troubleshoot user errors with Office Add-ins](https://docs.microsoft.com/office/dev/add-ins/testing/testing-and-troubleshooting)</span></span>