---
title: Ziņojumu piekļuve liegta ziņojumus OneDrive darba vietas
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 95bd46e8b7a6006f3735612d9a5602fb2b2a283b
ms.sourcegitcommit: bc7d6f4f3c9f7060d073f5130e1ec856e248d020
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/02/2020
ms.locfileid: "44511191"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="c5d17-102">Ziņojumu piekļuve liegta ziņojumus OneDrive darba vietas</span><span class="sxs-lookup"><span data-stu-id="c5d17-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="c5d17-103">Visbiežāk šī problēma rodas, ja lietotājs tiek dzēsts un atkārtoti izveidots ar pašu lietotāja pamatnosaukums (UPN).</span><span class="sxs-lookup"><span data-stu-id="c5d17-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="c5d17-104">Jaunais konts ir izveidots, izmantojot citu PUID (Passport unikālo ID) vērtību.</span><span class="sxs-lookup"><span data-stu-id="c5d17-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="c5d17-105">Kad lietotājs mēģina piekļūt vietņu kolekcijas vai to OneDrive, lietotājam ir nepareiza PUID.</span><span class="sxs-lookup"><span data-stu-id="c5d17-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="c5d17-106">Otrs scenārijs ietver direktorija sinhronizēšana ar Active Directory organizatoriskajai vienībai (OU).</span><span class="sxs-lookup"><span data-stu-id="c5d17-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="c5d17-107">Ja lietotāji jau ir pierakstījies SharePoint un pēc tam tiek pārvietoti uz citu OU un resynced ar SharePoint, tās var rasties šī problēma.</span><span class="sxs-lookup"><span data-stu-id="c5d17-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="c5d17-108">Lai novērstu šo problēmu, jums vajadzētu atjaunot sākotnējā UPN ar šajā rakstā aprakstītās darbības, [atjaunot lietotāju Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="c5d17-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="c5d17-109">Ja nevarat atjaunot sākotnējo lietotāju, noņemiet veco lietotāju no vietnes OneDrive, veicot šīs darbības, [lietotāja informācijas sarakstā noņemiet lietotāju]().</span><span class="sxs-lookup"><span data-stu-id="c5d17-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="c5d17-110">Pēc tam, kad tas ir izdarīts, varat pārbaudīt lietotājam ir administratora tiesības uz OneDrive vietni, izpildot darbības, lai [pievienotu admin lietotāja onedrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="c5d17-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="c5d17-111">Papildinformāciju par atļauju līmeņiem skatiet rakstā [atļauju līmeņu izpratne SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="c5d17-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
