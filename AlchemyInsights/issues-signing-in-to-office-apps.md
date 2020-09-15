---
title: Problēmas saistībā ar pierakstīšanos Microsoft 365 lietojumprogrammās
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 7d2cfd437bb55804c3b9263428833c10d5caaa47
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47695330"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="b7101-102">Microsoft 365 programmu labošana "Diemžēl cits jūsu organizācijas konts jau ir pierakstījies" ziņojumā</span><span class="sxs-lookup"><span data-stu-id="b7101-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="b7101-103">Lai novērstu šo kļūdu, izmēģiniet tālāk norādīto:</span><span class="sxs-lookup"><span data-stu-id="b7101-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="b7101-104">Noņemiet visus darba kontus, izņemot ietekmēto kontu, izmantojot Windows iestatījumus > **piekļūt darba vai mācību**iestādēm.</span><span class="sxs-lookup"><span data-stu-id="b7101-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="b7101-105">[Notīriet Office akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows akreditācijas datu pārvaldnieku.</span><span class="sxs-lookup"><span data-stu-id="b7101-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="b7101-106">**Piezīme:** Office 2016 reģistra ceļi ir mainīti uz 16,0.</span><span class="sxs-lookup"><span data-stu-id="b7101-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="b7101-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="b7101-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="b7101-108">Atveriet kādu Office lietojumprogrammu, izvēlieties **faila**  >  **konta**  >  **izrakstīšanās**. Pēc tam pierakstieties, izmantojot lietotāja kontu ar derīgu licenci.</span><span class="sxs-lookup"><span data-stu-id="b7101-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="b7101-109">Lai uzzinātu vairāk, lasiet [Office konti](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="b7101-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="b7101-110">Darbam ar Mac, skatiet rakstu [nevarat pierakstīties Office 2016 for Mac lietojumprogrammu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="b7101-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="b7101-111">Lai iegūtu papildinformāciju, skatiet rakstu ["Diemžēl cits jūsu organizācijas konts jau ir pierakstījies šajā datorā" sistēmā Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span><span class="sxs-lookup"><span data-stu-id="b7101-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>