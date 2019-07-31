---
title: Pierakstīšanās pakalpojumā Office apps jautājumiem
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
ms.openlocfilehash: 3622a3408b25b43090e9414ae5ffcfc2760264ee
ms.sourcegitcommit: 699ac3b0d66e0640f8e933eba3c2a4ba1cfcf3c7
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/30/2019
ms.locfileid: "35938270"
---
# <a name="issues-signing-in-to-office-apps"></a><span data-ttu-id="1402b-102">Pierakstīšanās pakalpojumā Office apps jautājumiem</span><span class="sxs-lookup"><span data-stu-id="1402b-102">Issues signing in to Office apps</span></span>

<span data-ttu-id="1402b-103">Lai labotu pierakstīšanās problēmas ar Office apps, mēģiniet veikt šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="1402b-103">To fix sign-in issues with Office apps, try the following:</span></span>

- <span data-ttu-id="1402b-104">Noņemt visu darbu konti, izņemot skarto kontā, izmantojot Windows iestatījumos > **pieeja darbā vai skolā**.</span><span class="sxs-lookup"><span data-stu-id="1402b-104">Remove all work accounts, except the affected account, using Windows Settings > **Access work or school**.</span></span>
- <span data-ttu-id="1402b-105">[Notīrīt biroja akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows Credential Manager.</span><span class="sxs-lookup"><span data-stu-id="1402b-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="1402b-106">**Piezīme:** Ir mainījušies 16,0 Office 2016 reģistra ceļus.</span><span class="sxs-lookup"><span data-stu-id="1402b-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="1402b-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="1402b-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="1402b-108">Atveriet Office app, izvēlieties **failu** > **konta** > **Sign Out**. Pierakstieties, izmantojot lietotāja kontu ar derīgu licenci.</span><span class="sxs-lookup"><span data-stu-id="1402b-108">Open an Office app, choose **File** > **Account** > **Sign Out**. Then sign in using a user account with a valid license.</span></span> <span data-ttu-id="1402b-109">Detalizētu informāciju skatiet [Accounts birojā](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="1402b-109">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="1402b-110">Mac, skatiet sadaļā [nevar pierakstīties Office 2016 Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span><span class="sxs-lookup"><span data-stu-id="1402b-110">For Mac, see [Can't sign in to an Office 2016 for Mac app](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-2016-for-mac-fail).</span></span>
- <span data-ttu-id="1402b-111">Ja kļūdas rodas, savienojoties Office 365, izmantojot Office 2013, iespējot mūsdienu Office klienta autentifikāciju.</span><span class="sxs-lookup"><span data-stu-id="1402b-111">If the errors occurs while connecting to Office 365 using Office 2013, enable modern authentication for Office client.</span></span>

<span data-ttu-id="1402b-112">Papildinformāciju skatiet sadaļā</span><span class="sxs-lookup"><span data-stu-id="1402b-112">For more information, see:</span></span>
- [<span data-ttu-id="1402b-113">Nevar pierakstīties Office 365, Azure vai Intune</span><span class="sxs-lookup"><span data-stu-id="1402b-113">You can't sign in to Office 365, Azure, or Intune</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-to-office-365-azure-intune)
- [<span data-ttu-id="1402b-114">Pierakstīšanās pēc atjauninājums Office 2016 savienojuma problēmas pamatā Windows 10 16.0.7967</span><span class="sxs-lookup"><span data-stu-id="1402b-114">Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10</span></span>](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)
- [<span data-ttu-id="1402b-115">"Atvainojiet, citam kontam no uzņēmuma jau pierakstījies šajā datorā" birojā</span><span class="sxs-lookup"><span data-stu-id="1402b-115">"Sorry, another account from your organization is already signed in on this computer" in Office</span></span>](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in)
- [<span data-ttu-id="1402b-116">Novērst Office modernās autentifikācijas pierakstīšanās problēmas, kad lietojat ADF</span><span class="sxs-lookup"><span data-stu-id="1402b-116">Troubleshoot sign-in issues with Office modern authentication when you use ADFS</span></span>](https://docs.microsoft.com/office365/troubleshoot/authentication/sign-in-issue-with-modern-auth)