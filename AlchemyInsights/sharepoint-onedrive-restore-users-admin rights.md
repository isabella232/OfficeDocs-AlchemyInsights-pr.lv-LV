---
title: Problēmu novēršanas pieeja liegta ziņojumus OneDrive darba vietām
ms.author: efrene
author: efrene
manager: pamgreen
ms.date: 11/14/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.assetid: cebb7a4a-33e1-474e-a5d0-dbd02a80b1e9
ms.openlocfilehash: d47ce80bdd07a25d9724057edf0289808a00a3db
ms.sourcegitcommit: 8a83b508785c96c19648ed574f442bbef2c2dff9
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 08/07/2019
ms.locfileid: "36232537"
---
# <a name="troubleshooting-access-denied-messages-to-onedrive-for-business-sites"></a><span data-ttu-id="abbcf-102">Problēmu novēršanas pieeja liegta ziņojumus OneDrive darba vietām</span><span class="sxs-lookup"><span data-stu-id="abbcf-102">Troubleshooting Access denied messages to OneDrive for Business sites</span></span>

<span data-ttu-id="abbcf-103">Šī problēma visbiežāk rodas, ja lietotājs ir dzēsta un izveidota atkārtoti, izmantojot vienu un to pašu lietotāja pamatnosaukums (UPN).</span><span class="sxs-lookup"><span data-stu-id="abbcf-103">This issue most frequently occurs when a user is deleted and re-created with the same user principal name (UPN).</span></span> <span data-ttu-id="abbcf-104">Jaunais konts ir izveidots, izmantojot citu PUID (pases unikālo ID) vērtību.</span><span class="sxs-lookup"><span data-stu-id="abbcf-104">The new account is created by using a different PUID (Passport Unique ID) value.</span></span> <span data-ttu-id="abbcf-105">Ja lietotājs mēģina piekļūt vietņu kolekcijā vai to OneDrive, lietotājam ir nepareiza PUID.</span><span class="sxs-lookup"><span data-stu-id="abbcf-105">When the user tries to access a site collection or their OneDrive, the user has an incorrect PUID.</span></span> <span data-ttu-id="abbcf-106">Otrais scenārijs ietver directory sinhronizācija ar Active Directory organizācijas vienību (OU).</span><span class="sxs-lookup"><span data-stu-id="abbcf-106">A second scenario involves directory synchronization with an Active Directory organizational unit (OU).</span></span> <span data-ttu-id="abbcf-107">Ja lietotāji jau pieslēdzās SharePoint, un tad ir pārvietots uz citu OU un resynced ar SharePoint, viņiem šī problēma var rasties.</span><span class="sxs-lookup"><span data-stu-id="abbcf-107">If users have already signed in to SharePoint, and then are moved to a different OU and resynced with SharePoint, they may experience this problem.</span></span>

1. <span data-ttu-id="abbcf-108">Lai atrisinātu šo jautājumu vajadzētu atjaunot sākotnējo UPN ar rakstu,[atjaunot Office 365 lietotāja](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide)darbības.</span><span class="sxs-lookup"><span data-stu-id="abbcf-108">To resolve this issue you should restore the original UPN with the steps in the article,[Restore a user in Office 365](https://docs.microsoft.com/office365/admin/add-users/restore-user?view=o365-worldwide).</span></span>
2. <span data-ttu-id="abbcf-109">Ja sākotnējais lietotājs nevar atjaunot vecās lietotāja vajadzētu noņemt no OneDrive vietā, izmantojot šos norādījumus, [noņemtu kādu lietotāju, sarakstā lietotāja info]().</span><span class="sxs-lookup"><span data-stu-id="abbcf-109">If you cannot restore the original user you should remove the old user from the OneDrive site using these steps, [Remove a user from the user info list]().</span></span> 
3. <span data-ttu-id="abbcf-110">Pēc tam, kad tas ir izdarīts, jūs varat pārbaudīt lietotājam nav administratora tiesības vietnē OneDrive, veiciet norādītās darbības, lai [pievienot admin lietotāja OneDrive kundzes](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span><span class="sxs-lookup"><span data-stu-id="abbcf-110">After this is done, you can verify the user has admin rights to the OneDrive site by following the steps to [Add admin's for a user's OneDrive](https://docs.microsoft.com/sharepoint/manage-user-profiles?redirectSourcePath=%252fen-us%252farticle%252fmanage-user-profiles-in-the-sharepoint-admin-center-494bec9c-6654-41f0-920f-f7f937ea9723#add-and-remove-admins-for-a-users-onedrive)</span></span>

<span data-ttu-id="abbcf-111">Plašāku informāciju par atļauju līmeņiem, skatiet rakstā, [izpratne atļauju līmeņus koplietošanas vidē SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span><span class="sxs-lookup"><span data-stu-id="abbcf-111">For more information on permission levels, see the article, [Understanding permission levels in SharePoint](https://docs.microsoft.com/sharepoint/understanding-permission-levels).</span></span>
