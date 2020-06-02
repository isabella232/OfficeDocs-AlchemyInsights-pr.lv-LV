---
title: Ziņojumu par piekļuvi liegta problēmu novēršana
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 9430b9786b35dda9fb2604fb6ae3c39c8c258d6e
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44505386"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="ba999-102">Piekļuve liegta ziņojumu novēršana programmā SharePoint/OneDrive administrēšanas centrs</span><span class="sxs-lookup"><span data-stu-id="ba999-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="ba999-103">Ja saņemat ziņojumu par liegtu piekļuvi, mēģinot pārlūkot SharePoint/OneDrive administrēšanas centrs, lūdzu, pārliecinieties, vai [piešķirt licenci lietotājam](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="ba999-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="ba999-104">Ja lietotājam ir licence, pārliecinieties, ka viņiem ir [piešķirta administratora loma](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , kas var piekļūt administrēšanas centriem.</span><span class="sxs-lookup"><span data-stu-id="ba999-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="ba999-105">Šī problēma var rasties arī tad, ja lietotājs ir izdzēsts un atkārtoti izveidots ar pašu lietotāja pamatnosaukums (UPN).</span><span class="sxs-lookup"><span data-stu-id="ba999-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="ba999-106">Jaunais konts ir izveidots, izmantojot citu PUID (Passport unikālo ID) vērtību.</span><span class="sxs-lookup"><span data-stu-id="ba999-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="ba999-107">Kad lietotājs mēģina piekļūt vietņu kolekcijas vai to OneDrive, lietotājam ir nepareiza PUID.</span><span class="sxs-lookup"><span data-stu-id="ba999-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="ba999-108">Otrs scenārijs ietver direktorija sinhronizēšana ar Active Directory organizatoriskajai vienībai (OU).</span><span class="sxs-lookup"><span data-stu-id="ba999-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="ba999-109">Ja lietotāji jau ir pierakstījies SharePoint un pēc tam tiek pārvietoti uz citu OU un resynced ar SharePoint, tās var rasties šī problēma.</span><span class="sxs-lookup"><span data-stu-id="ba999-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="ba999-110">Lai novērstu šo problēmu, jums vajadzētu atjaunot sākotnējā UPN ar šajā rakstā aprakstītās darbības, [atjaunot lietotāju Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="ba999-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="ba999-111">Piezīme: ja OneDrive vai SharePoint administrēšanas centrs nav pieejams vairākiem lietotājiem, kuriem iepriekš bija piekļuve, var būt pagaidu pakalpojumu problēma.</span><span class="sxs-lookup"><span data-stu-id="ba999-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="ba999-112">[Pārbaudiet pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="ba999-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


