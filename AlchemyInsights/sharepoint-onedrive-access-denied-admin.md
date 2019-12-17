---
title: Ziņojumu par piekļuvi liegta problēmu novēršana
ms.author: pebaum
author: pebaum
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 57919e6dbd81a5bf3b17fb067485e8eec23b7d4c
ms.sourcegitcommit: 0f0186044a3597e42ad14c32ca58e7224344dcfa
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/15/2019
ms.locfileid: "40051432"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="16204-102">Piekļuve liegta ziņojumu novēršana programmā SharePoint/OneDrive administrēšanas centrs</span><span class="sxs-lookup"><span data-stu-id="16204-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="16204-103">Ja saņemat ziņojumu par liegtu piekļuvi, mēģinot pārlūkot SharePoint/OneDrive administrēšanas centrs, lūdzu, pārliecinieties, vai [piešķirt licenci lietotājam](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="16204-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="16204-104">Ja lietotājam ir licence, pārliecinieties, ka viņiem ir [piešķirta administratora loma](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , kas var piekļūt administrēšanas centriem.</span><span class="sxs-lookup"><span data-stu-id="16204-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="16204-105">Šī problēma var rasties arī tad, ja lietotājs ir izdzēsts un atkārtoti izveidots ar pašu lietotāja pamatnosaukums (UPN).</span><span class="sxs-lookup"><span data-stu-id="16204-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="16204-106">Jaunais konts ir izveidots, izmantojot citu PUID (Passport unikālo ID) vērtību.</span><span class="sxs-lookup"><span data-stu-id="16204-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="16204-107">Kad lietotājs mēģina piekļūt vietņu kolekcijas vai to OneDrive, lietotājam ir nepareiza PUID.</span><span class="sxs-lookup"><span data-stu-id="16204-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="16204-108">Otrs scenārijs ietver direktorija sinhronizēšana ar Active Directory organizatoriskajai vienībai (OU).</span><span class="sxs-lookup"><span data-stu-id="16204-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="16204-109">Ja lietotāji jau ir pierakstījies SharePoint un pēc tam tiek pārvietoti uz citu OU un resynced ar SharePoint, tās var rasties šī problēma.</span><span class="sxs-lookup"><span data-stu-id="16204-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="16204-110">Lai novērstu šo problēmu, jums vajadzētu atjaunot sākotnējā UPN ar šajā rakstā aprakstītās darbības, [atjaunojiet lietotāja Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span><span class="sxs-lookup"><span data-stu-id="16204-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="16204-111">Piezīme: ja OneDrive vai SharePoint administrēšanas centrs nav pieejams vairākiem lietotājiem, kuriem iepriekš bija piekļuve, var būt pagaidu pakalpojumu problēma.</span><span class="sxs-lookup"><span data-stu-id="16204-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="16204-112">[Pārbaudiet pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="16204-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


