---
title: Problēmas saistībā ar pierakstīšanos Office programmās
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2574"
ms.openlocfilehash: 695d449a876c22ff441da2367ef67aaea470eb66
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43763008"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="55841-102">Problēmas saistībā ar pierakstīšanos Office programmās</span><span class="sxs-lookup"><span data-stu-id="55841-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="55841-103">Lai novērstu pierakstīšanās problēmas ar Office lietojumprogrammām, rīkojieties šādi:</span><span class="sxs-lookup"><span data-stu-id="55841-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="55841-104">Noņemiet visus darba kontus, izņemot ietekmēto kontu, izmantojot Windows iestatījumus > **piekļuvi darbam vai skolai**.</span><span class="sxs-lookup"><span data-stu-id="55841-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="55841-105">[Notīrīt Office akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows akreditācijas datu pārvaldnieku.</span><span class="sxs-lookup"><span data-stu-id="55841-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="55841-106">**Piezīme:** Office 2016 reģistra ceļi ir mainījušies 16,0.</span><span class="sxs-lookup"><span data-stu-id="55841-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="55841-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="55841-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="55841-108">Atveriet Office programmu, izvēlieties **failu** > **konta** > **Izrakstīties**. Pēc tam pierakstieties, izmantojot lietotāja kontu ar derīgu licenci.</span><span class="sxs-lookup"><span data-stu-id="55841-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="55841-109">Lai uzzinātu vairāk, lasiet [Office konti](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="55841-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="55841-110">Darbam ar Mac, skatiet rakstu [nevarat pierakstīties Office 2016 for Mac lietojumprogrammu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="55841-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="55841-111">Ja rodas kļūdas, veidojot savienojumu ar Microsoft 365, izmantojot Office 2013, iespējot mūsdienu autentifikācijas Office klienta.</span><span class="sxs-lookup"><span data-stu-id="55841-111">If the errors occurs while connecting to Microsoft 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="55841-112">Papildinformāciju skatiet rakstā:</span><span class="sxs-lookup"><span data-stu-id="55841-112">For more information, see:</span></span>
- [<span data-ttu-id="55841-113">Nevar pierakstīties Microsoft 365, Azure vai InTune</span><span class="sxs-lookup"><span data-stu-id="55841-113">You can't sign in to Microsoft 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="55841-114">Savienojuma problēmas pierakstīšanās pēc atjauninājuma Office 2016 veidot 16.0.7967 Windows 10</span><span class="sxs-lookup"><span data-stu-id="55841-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="55841-115">"Atvainojiet, citu kontu no jūsu uzņēmums jau ir pierakstījies šajā datorā" Office</span><span class="sxs-lookup"><span data-stu-id="55841-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="55841-116">Pierakstīšanās problēmu novēršana, izmantojot Office moderno autentifikāciju, izmantojot ADFS</span><span class="sxs-lookup"><span data-stu-id="55841-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)