---
title: Piekļuve liegta ziņojumu novēršana
ms.author: pebaum
author: pebaum
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: 22f5966fdae563c44affb7d0447787a4ee0aca93
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47767669"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="73efa-102">Problēmu novēršana saistībā ar piekļuvi liegti SharePoint/OneDrive administrēšanas centrā</span><span class="sxs-lookup"><span data-stu-id="73efa-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="73efa-103">Ja tiek saņemts ziņojums par liegtu piekļuvi, mēģinot pārlūkot SharePoint/OneDrive administrēšanas centru, pārliecinieties, vai jums ir [piešķirta licence lietotājam](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span><span class="sxs-lookup"><span data-stu-id="73efa-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/microsoft-365/admin/add-users/add-users).</span></span> <span data-ttu-id="73efa-104">Ja lietotājam ir licence, pārliecinieties arī, vai tiem ir [piešķirta administratora loma](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) , kas var piekļūt administrēšanas centriem.</span><span class="sxs-lookup"><span data-stu-id="73efa-104">If the user has a license, you should also make sure they are [assigned an administrator role](hhttps://docs.microsoft.com/microsoft-365/admin/add-users/about-admin-roles) that can access the admin centers.</span></span>

<span data-ttu-id="73efa-105">Šī problēma var rasties arī tad, ja lietotājs tiek izdzēsts un atkārtoti izveidots ar vienu un to pašu lietotāja pamatnosaukumu (UPN).</span><span class="sxs-lookup"><span data-stu-id="73efa-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="73efa-106">Jaunais konts ir izveidots, izmantojot citu PUID (pases unikālā ID) vērtību.</span><span class="sxs-lookup"><span data-stu-id="73efa-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="73efa-107">Kad lietotājs mēģina piekļūt vietņu kolekcijai vai to OneDrive, lietotājam ir nepareizs PUID.</span><span class="sxs-lookup"><span data-stu-id="73efa-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="73efa-108">Otrais scenārijs ietver direktorija sinhronizēšanu ar Active Directory organizācijas vienību (OU).</span><span class="sxs-lookup"><span data-stu-id="73efa-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="73efa-109">Ja lietotāji jau ir pierakstījušies pakalpojumā SharePoint, un pēc tam tiek pārvietoti uz citu un sinhronizētu ar SharePoint, šī problēma var rasties.</span><span class="sxs-lookup"><span data-stu-id="73efa-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="73efa-110">Lai atrisinātu šo problēmu, atjaunojiet oriģinālo UPN, veicot rakstā norādītās darbības, [atjaunojiet lietotāju pakalpojumā Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="73efa-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>

<span data-ttu-id="73efa-111">Piezīme. Ja jūsu OneDrive vai SharePoint administrēšanas centrs nav pieejams vairākiem lietotājiem, kuriem agrāk bija piekļuve, iespējama īslaicīga pakalpojumu problēma.</span><span class="sxs-lookup"><span data-stu-id="73efa-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="73efa-112">[Skatiet pakalpojuma darbspējas informācijas paneli](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="73efa-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


