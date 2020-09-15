---
title: Piekļuve liegta ziņojumiem pakalpojumā OneDrive darbam vietnes
ms.author: pebaum
author: pebaum
manager: pamgreen
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: 9001cf0b7d9f1f05a2ecedca2c3137dd1b8a1c38
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47670623"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="34e97-102">Piekļuve liegta ziņojumiem pakalpojumā OneDrive darbam vietnes</span><span class="sxs-lookup"><span data-stu-id="34e97-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="34e97-103">Šī problēma visbiežāk rodas, ja lietotājs tiek izdzēsts un atkārtoti izveidots ar vienu un to pašu lietotāja pamatnosaukumu (UPN).</span><span class="sxs-lookup"><span data-stu-id="34e97-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="34e97-104">Jaunais konts ir izveidots, izmantojot citu PUID (pases unikālā ID) vērtību.</span><span class="sxs-lookup"><span data-stu-id="34e97-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="34e97-105">Kad lietotājs mēģina piekļūt vietņu kolekcijai vai to OneDrive, lietotājam ir nepareizs PUID.</span><span class="sxs-lookup"><span data-stu-id="34e97-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="34e97-106">Otrais scenārijs ietver direktorija sinhronizēšanu ar Active Directory organizācijas vienību (OU).</span><span class="sxs-lookup"><span data-stu-id="34e97-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="34e97-107">Ja lietotāji jau ir pierakstījušies pakalpojumā SharePoint, un pēc tam tiek pārvietoti uz citu un sinhronizētu ar SharePoint, šī problēma var rasties.</span><span class="sxs-lookup"><span data-stu-id="34e97-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="34e97-108">Lai atrisinātu šo problēmu, atjaunojiet sākotnējo UPN, veicot šajā rakstā norādītās darbības, [atjaunojiet lietotāju pakalpojumā Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span><span class="sxs-lookup"><span data-stu-id="34e97-108">To resolve this issue you should restore the original UPN with the steps in the article, [Restore a user in Microsoft 365](https://docs.microsoft.com/microsoft-365/admin/add-users/restore-user).</span></span>
2. <span data-ttu-id="34e97-109">Ja nevarat atjaunot oriģinālo lietotāju, no OneDrive vietnes Noņemiet veco lietotāju, veicot šīs darbības, lietotāja [informācijas sarakstā noņemiet lietotāju]().</span><span class="sxs-lookup"><span data-stu-id="34e97-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="34e97-110">Kad tas ir paveikts, varat pārbaudīt, vai lietotājam ir administratora tiesības uz OneDrive vietni, izpildot darbības, kas jāveic, lai [pievienotu administratora atļaujas lietotāja OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span><span class="sxs-lookup"><span data-stu-id="34e97-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles)</span></span>

<span data-ttu-id="34e97-111">Papildinformāciju par atļauju līmeņiem skatiet rakstā informācija par [SharePoint atļauju līmeņiem](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="34e97-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
