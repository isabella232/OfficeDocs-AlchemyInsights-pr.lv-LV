---
title: 126 Vai programmā OWA nevar atrast pastkastes iegūšanas kļūdu?
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "126"
- "1600020"
ms.assetid: e85bffec-e5ad-418a-8561-dab6257e1864
ms.openlocfilehash: 6bab821aaa3b50c365ef5d25a61bca195c76d7ce
ms.sourcegitcommit: e552d65aac79433a911723412bf1252d20d3f0da
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 03/30/2021
ms.locfileid: "51426669"
---
# <a name="getting-a-mailbox-not-found-error-in-outlook-on-the-web"></a><span data-ttu-id="161f3-102">Vai programmā Outlook tīmeklī tiek atrasta kļūda pastkastē?</span><span class="sxs-lookup"><span data-stu-id="161f3-102">Getting a mailbox not found error in Outlook on the web?</span></span>

<span data-ttu-id="161f3-103">Ja izmantojat Outlook tīmeklī un saņemat  kļūdas ziņojumu par pastkasti, kontam, kuru izmantojāt, lai izveidotu savienojumu ar Outlook tīmeklī, nav Exchange Online licences un tāpēc ar kontu nav saistīta neviena pastkaste.</span><span class="sxs-lookup"><span data-stu-id="161f3-103">If you're using Outlook on the web and you get a **Mailbox couldn't be found for** error, the account that you used to connect to Outlook on the web doesn't have an Exchange Online license and therefore, no mailbox is associated with the account.</span></span> <span data-ttu-id="161f3-104">Administrators var piešķirt licenci jūsu kontam, veicot tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="161f3-104">Your admin can assign a license to your account by following these steps:</span></span>

1. <span data-ttu-id="161f3-105">Atveriet [Microsoft 365 administrēšanas centru,](https://portal.office.com/adminportal/home#/homepage) sadaļā  Lietotāji dodieties uz sadaļu Aktīvie lietotāji un atlasiet lietotāju, kuram tiek rādīta kļūda. </span><span class="sxs-lookup"><span data-stu-id="161f3-105">Open the [Microsoft 365 admin center](https://portal.office.com/adminportal/home#/homepage) and go to **Active users** under the **Users** section, and select the user who is seeing the error.</span></span>

2. <span data-ttu-id="161f3-106">Atvērtajā lietotāja lapā dodieties uz sadaļu Licences un  programmas, atlasiet atbilstošo vērtību **Atrašanās** vieta un piešķiriet licenci, kas satur Exchange Online (izvērsiet licenci, lai skatītu detalizētu informāciju par to).</span><span class="sxs-lookup"><span data-stu-id="161f3-106">In the user page that opens, go to the **Licenses and Apps** section, select the appropriate **Location** value, and assign a license that contains Exchange Online (expand the license to see its details).</span></span> <span data-ttu-id="161f3-107">Kad esat pabeidzis, noklikšķiniet uz **Saglabāt izmaiņas.**</span><span class="sxs-lookup"><span data-stu-id="161f3-107">When you're finished, click **Save changes**.</span></span>

<span data-ttu-id="161f3-108">Dažos gadījumos, ja licence jau ir piešķirta lietotāja kontam, licences noņemšana un atkārtota piešķiršana palīdz novērst problēmu un nodrošināt to pareizi sistēmā:</span><span class="sxs-lookup"><span data-stu-id="161f3-108">In some cases, if the license is already assigned to a user account, removing and reassigning the license helps to resolve the issue and get it properly provisioned in the system:</span></span> 

- <span data-ttu-id="161f3-109">Pārbaudiet, vai jūsu M365 Exchange Online (un citi, ja jums ir) abonementi ir pašreizējie un nav nesen beidzies derīgums.</span><span class="sxs-lookup"><span data-stu-id="161f3-109">Check to see if your M365 Exchange Online (and other, if you have any) subscriptions are current and have not recently expired.</span></span>

<span data-ttu-id="161f3-110">Kad esat pārliecināts, ka jūsu abonementa derīgums nav beidzies un lietotāja kontam ir piešķirta derīga licence, var paiet līdz pat 24 stundām, līdz licence tiek nodrošināta, tāpēc, iespējams, būs jāgaida, līdz problēma tiks atrisināta.</span><span class="sxs-lookup"><span data-stu-id="161f3-110">Once you have made sure that your subscription has not expired and a valid license has been assigned to the user account, it can take up to 24 hours for license to get provisioned, so you might have to wait for your issue to resolve.</span></span> <span data-ttu-id="161f3-111">Papildinformāciju skatiet [rakstā Licenču piešķiršana un pārvaldība.](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses)</span><span class="sxs-lookup"><span data-stu-id="161f3-111">For more info, see [Assign and manage licenses](https://docs.microsoft.com/deployoffice/overview-licensing-activation-microsoft-365-apps#assign-and-manage-licenses).</span></span>