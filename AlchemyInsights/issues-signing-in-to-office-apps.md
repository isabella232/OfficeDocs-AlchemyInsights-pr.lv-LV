---
title: Problēmas ar pierakstīšanos Microsoft 365 programmās
ms.author: pebaum
author: pebaum
manager: scotv
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "9000571"
- "2560"
ms.openlocfilehash: 8065a49c42953013ccfae9c5c1714d10ee0b4d49
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833082"
---
# <a name="fixing-the-microsoft-365-apps-sorry-another-account-from-your-organization-is-already-signed-in-message"></a><span data-ttu-id="d6db4-102">Tiek izlabota Microsoft 365 lietojumprogrammu kļūda "Diemžēl cits jūsu organizācijas konts jau ir pierakstījies"</span><span class="sxs-lookup"><span data-stu-id="d6db4-102">Fixing the Microsoft 365 apps "Sorry, another account from your organization is already signed in" message</span></span>

<span data-ttu-id="d6db4-103">Lai novērstu šo kļūdu, izmēģiniet tālāk norādīto:</span><span class="sxs-lookup"><span data-stu-id="d6db4-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="d6db4-104">Noņemiet visus darba kontus, izņemot ietekmēto kontu, izmantojot Windows > **Piekļūt darbam vai mācībām.**</span><span class="sxs-lookup"><span data-stu-id="d6db4-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="d6db4-105">[Notīriet Office akreditācijas](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) datus, izmantojot Windows akreditācijas datu pārvaldnieku.</span><span class="sxs-lookup"><span data-stu-id="d6db4-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d6db4-106">**Piezīme.** Office 2016 reģistra ceļi ir mainīti uz 16.0.</span><span class="sxs-lookup"><span data-stu-id="d6db4-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d6db4-107">(Piemēram, \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d6db4-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d6db4-108">Atveriet kādu Office lietojumprogrammu, **izvēlieties**  >  **Faila konts**  >  **Izrakstīties**. Pēc tam pierakstieties, izmantojot lietotāja kontu ar derīgu licenci.</span><span class="sxs-lookup"><span data-stu-id="d6db4-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="d6db4-109">Lai uzzinātu vairāk, lasiet [Office konti](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="d6db4-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="d6db4-110">Darbam ar Mac, skatiet rakstu [nevarat pierakstīties Office 2016 for Mac lietojumprogrammu](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="d6db4-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>

<span data-ttu-id="d6db4-111">Papildinformāciju skatiet Office sadaļā "Diemžēl jūsu organizācijas konts jau ir [pierakstījies šajā datorā".](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)</span><span class="sxs-lookup"><span data-stu-id="d6db4-111">For more information, see ["Sorry, another account from your organization is already signed in on this computer" in Office](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in).</span></span>