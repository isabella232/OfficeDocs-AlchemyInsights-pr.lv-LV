---
title: Risinājumi problēmām, kas saistītas ar Office instalēšanu termināļa serverī
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: 85f24284-af6f-4624-b6be-901a4a9206eb
ms.openlocfilehash: df1a50031196fbd79662cee620fc41c7be14e179
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47738464"
---
# <a name="solutions-for-issues-around-installing-office-on-a-terminal-server"></a><span data-ttu-id="e4d2d-102">Risinājumi problēmām, kas saistītas ar Office instalēšanu termināļa serverī</span><span class="sxs-lookup"><span data-stu-id="e4d2d-102">Solutions for issues around installing office on a Terminal Server</span></span>

<span data-ttu-id="e4d2d-103">Lai izmantotu koplietotu datora aktivizāciju, ir nepieciešams abonements, kurā iekļautas Microsoft 365 lietojumprogrammas darbam ar Enterprise.</span><span class="sxs-lookup"><span data-stu-id="e4d2d-103">To use shared computer activation, you must have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>
  
- <span data-ttu-id="e4d2d-104">Pārbaudiet, vai ir iespējota koplietojamā datora aktivizācija</span><span class="sxs-lookup"><span data-stu-id="e4d2d-104">Verify that shared computer activation is enabled</span></span>
- <span data-ttu-id="e4d2d-105">Pārbaude, vai aktivizēšana bija sekmīga</span><span class="sxs-lookup"><span data-stu-id="e4d2d-105">Verify that activation succeeded</span></span>
- <span data-ttu-id="e4d2d-106">Pārskatiet koplietojamā datora aktivizēšanas kļūdu ziņojumus:</span><span class="sxs-lookup"><span data-stu-id="e4d2d-106">Review error messages for shared computer activation:</span></span>
- <span data-ttu-id="e4d2d-107">"Jūsu kontā pieejamos produktus nevar izmantot, lai aktivizētu Office koplietojamās datora scenārijos"</span><span class="sxs-lookup"><span data-stu-id="e4d2d-107">"The products we found in your account cannot be used to activate Office in shared computer scenarios"</span></span>
  
<span data-ttu-id="e4d2d-108">Šī kļūda nozīmē, ka jums nav abonementa, kurā iekļautas Microsoft 365 lietojumprogrammas darbam ar Enterprise.</span><span class="sxs-lookup"><span data-stu-id="e4d2d-108">This error means that you don't have a subscription that includes Microsoft 365 Apps for enterprise.</span></span>

<span data-ttu-id="e4d2d-109">"Nelicencēts produkts"</span><span class="sxs-lookup"><span data-stu-id="e4d2d-109">"Unlicensed Product"</span></span>

- <span data-ttu-id="e4d2d-110">Pārbaudiet, vai lietotājam ir piešķirta licence Microsoft 365 lietojumprogrammām darbam ar Enterprise.</span><span class="sxs-lookup"><span data-stu-id="e4d2d-110">Check that the user is assigned a license for Microsoft 365 Apps for enterprise.</span></span>
- <span data-ttu-id="e4d2d-111">Pārbaudiet, vai lietotājs pierakstās ar lietotāja kontu.</span><span class="sxs-lookup"><span data-stu-id="e4d2d-111">Check that the user signs in with their user account.</span></span>
- <span data-ttu-id="e4d2d-112">Pārbaudiet, vai pastāv savienojamība starp koplietotu datoru un internetu.</span><span class="sxs-lookup"><span data-stu-id="e4d2d-112">Check that there is connectivity between the shared computer and the Internet.</span></span>

<span data-ttu-id="e4d2d-113">Citus problēmu novēršanas padomus skatiet rakstā [problēmu novēršana saistībā ar koplietojamu datora aktivizāciju](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span><span class="sxs-lookup"><span data-stu-id="e4d2d-113">For other troubleshooting tips, please see: [Troubleshoot issues with shared computer activation](https://docs.microsoft.com/DeployOffice/troubleshoot-shared-computer-activation)</span></span>