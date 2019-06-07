---
title: Novērst problēmas ziņojumu piekļuve liegta
ms.author: kirks
author: Techwriter40
ms.date: 6/29/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.assetid: d678b57a-53ad-4414-9423-d8726a0c532f
ms.openlocfilehash: c204f1889e03886fdfd3d1c760a4a2beb82b0836
ms.sourcegitcommit: 4b7e478ce700c0b781efec3857ac4dce5bdf00c6
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/07/2019
ms.locfileid: "34760347"
---
# <a name="troubleshoot-access-denied-messages-in-sharepointonedrive-admin-center"></a><span data-ttu-id="63dcf-102">Problēmu novēršana darbā ar Sharepoint/OneDrive administrēšanas centrā ziņojumi Piekļuve liegta</span><span class="sxs-lookup"><span data-stu-id="63dcf-102">Troubleshoot Access Denied messages in Sharepoint/OneDrive Admin Center</span></span>

<span data-ttu-id="63dcf-103">Ja saņemat ziņojumu par liegtu piekļuvi, mēģinot meklēt Sharepoint/OneDrive Admin Center, lūdzu, pārliecinieties, ka jums [piešķirt licenci lietotājam](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span><span class="sxs-lookup"><span data-stu-id="63dcf-103">If you are receiving an access denied message when attempting to browse to a Sharepoint/OneDrive Admin Center, please make sure that you [assign a license to the user](https://docs.microsoft.com/office365/admin/subscriptions-and-billing/assign-licenses-to-users?view=o365-worldwide&amp;tabs=One).</span></span> <span data-ttu-id="63dcf-104">Ja lietotājam ir licence, jums vajadzētu arī pārliecināties tie ir [piešķirta administratora loma](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) , var piekļūt admin centriem.</span><span class="sxs-lookup"><span data-stu-id="63dcf-104">If the user has a license, you should also make sure they are [assigned an administrator role](https://docs.microsoft.com/office365/admin/add-users/about-admin-roles?view=o365-worldwide) that can access the admin centers.</span></span>

<span data-ttu-id="63dcf-105">Šī problēma var arī rasties, ja lietotājs ir dzēsta un izveidota atkārtoti, izmantojot vienu un to pašu lietotāja pamatnosaukums (UPN).</span><span class="sxs-lookup"><span data-stu-id="63dcf-105">This issue can also occur when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="63dcf-106">Jaunais konts ir izveidots, izmantojot citu PUID (pases unikālo ID) vērtību.</span><span class="sxs-lookup"><span data-stu-id="63dcf-106">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="63dcf-107">Ja lietotājs mēģina piekļūt vietņu kolekcijā vai to OneDrive, lietotājam ir nepareiza PUID.</span><span class="sxs-lookup"><span data-stu-id="63dcf-107">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="63dcf-108">Otrais scenārijs ietver directory sinhronizācija ar Active Directory organizācijas vienību (OU).</span><span class="sxs-lookup"><span data-stu-id="63dcf-108">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="63dcf-109">Ja lietotāji jau pieslēdzās SharePoint, un tad ir pārvietots uz citu OU un resynced ar SharePoint, viņiem šī problēma var rasties.</span><span class="sxs-lookup"><span data-stu-id="63dcf-109">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

<span data-ttu-id="63dcf-110">Lai atrisinātu šo problēmu, vajadzētu atjaunot sākotnējo UPN ar rakstu, [atjaunot Office 365 lietotāja](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)darbības.</span><span class="sxs-lookup"><span data-stu-id="63dcf-110">To resolve this issue, you should restore the original UPN with the steps in the article, [Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>

<span data-ttu-id="63dcf-111">Piezīme: Ja OneDrive vai SharePoint administrēšanas centru nav pieejams vairākiem lietotājiem, kas iepriekš bija pieejams, var rasties pagaidu pakalpojumu jautājums.</span><span class="sxs-lookup"><span data-stu-id="63dcf-111">Note: If a OneDrive or SharePoint Admin center is not available to multiple users who previously had access, there may be a temporary service issue.</span></span>  <span data-ttu-id="63dcf-112">[Pārbaudiet pakalpojumu veselības vadības paneli](https://portal.office.com/adminportal/home#/servicehealth).</span><span class="sxs-lookup"><span data-stu-id="63dcf-112">[Check the service health dashboard](https://portal.office.com/adminportal/home#/servicehealth).</span></span>


