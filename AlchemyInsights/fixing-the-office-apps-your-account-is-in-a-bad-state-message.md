---
title: Office lietojumprogrammu labošana jūsu konts ir sliktā stāvoklī ziņojums
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "2558"
- "9000571"
ms.openlocfilehash: e591c56dd207a5bcb3979be3f66052121100b162
ms.sourcegitcommit: 2572c4e5a981d5f3f556835061c568cfd08b78da
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 12/27/2019
ms.locfileid: "41969605"
---
# <a name="fixing-the-office-apps-your-account-is-in-a-bad-state-error"></a><span data-ttu-id="70214-102">Labošana Office Apps "jūsu konts ir sliktā stāvoklī" kļūda</span><span class="sxs-lookup"><span data-stu-id="70214-102">Fixing the Office apps "Your account is in a bad state" error</span></span>

<span data-ttu-id="70214-103">Lai novērstu šo kļūdu, mēģiniet šīs opcijas attiecīgajā datorā:</span><span class="sxs-lookup"><span data-stu-id="70214-103">To fix this error, try the following options on the affected computer:</span></span>

- <span data-ttu-id="70214-104">Atveriet Office programmu, atlasiet **failu** > **konta** > **Izrakstīties no visiem kontiem**.</span><span class="sxs-lookup"><span data-stu-id="70214-104">Open an Office app, select **File** > **Account** > **Sign Out of all accounts**.</span></span> <span data-ttu-id="70214-105">Pierakstieties vēlreiz, izmantojot lietotāja kontu ar derīgu licenci.</span><span class="sxs-lookup"><span data-stu-id="70214-105">Sign in again using a user account with a valid license.</span></span> <span data-ttu-id="70214-106">Lai iegūtu detalizētu informāciju, skatiet [Office konti](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span><span class="sxs-lookup"><span data-stu-id="70214-106">For detailed information, see [Accounts in Office](https://support.office.com/article/accounts-in-office-628ea040-f265-49de-b986-be09c3ebf8a9).</span></span>
- <span data-ttu-id="70214-107">[Notīrīt Office akreditācijas datus](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) , izmantojot Windows akreditācijas datu pārvaldnieku.</span><span class="sxs-lookup"><span data-stu-id="70214-107">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/error-messages/another-account-already-signed-in#step-3-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br>
  <span data-ttu-id="70214-108">**Piezīme:** Office 2016 reģistra ceļi ir mainījušies 16,0.</span><span class="sxs-lookup"><span data-stu-id="70214-108">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="70214-109">Piemēram, \Software\Microsoft\Office\16.0\Common\Identity</span><span class="sxs-lookup"><span data-stu-id="70214-109">For example, \Software\Microsoft\Office\16.0\Common\Identity</span></span>\
- <span data-ttu-id="70214-110">Attiecīgajā datorā, iestatiet EnableADAL = 0, izmantojot šādas darbības:</span><span class="sxs-lookup"><span data-stu-id="70214-110">On the affected computer, set the EnableADAL = 0 using the following steps:</span></span>  
     1. <span data-ttu-id="70214-111">Ar peles labo pogu noklikšķiniet uz pogas Windows un atlasiet **palaist**.</span><span class="sxs-lookup"><span data-stu-id="70214-111">Right-click the Windows button and select **Run**.</span></span> <span data-ttu-id="70214-112">Lodziņā **Atvērt** ierakstiet **regedit**un pēc tam atlasiet **Labi**.</span><span class="sxs-lookup"><span data-stu-id="70214-112">In the **Open** box, type **regedit**, and then select **OK**.</span></span>
     2. <span data-ttu-id="70214-113">Atlasiet **Jā** , kad tiek piedāvāts atļaut reģistra redaktoram veikt izmaiņas ierīcē.</span><span class="sxs-lookup"><span data-stu-id="70214-113">Select **Yes** when prompted to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="70214-114">Reģistra redaktorā pievienojiet DWORD vērtību EnableADAL ar iestatījumu 0 sadaļā HKEY_CURRENT_USER \Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="70214-114">In the Registry Editor, add a DWORD value of EnableADAL with a setting of 0 under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>
- <span data-ttu-id="70214-115">Ja kļūda rodas, veidojot savienojumu ar Office 365, izmantojot Office 2013, [Iespējot mūsdienu autentifikācijas](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) Office klienta.</span><span class="sxs-lookup"><span data-stu-id="70214-115">If the error occurs while connecting to Office 365 using Office 2013, [enable modern authentication](https://docs.microsoft.com/office365/admin/security-and-compliance/enable-modern-authentication) for the Office client.</span></span>

<span data-ttu-id="70214-116">Lai iegūtu papildinformāciju, skatiet [kā novērst-pārlūka lietojumprogrammas, kas nevar pierakstīties Office 365, Azure vai InTune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span><span class="sxs-lookup"><span data-stu-id="70214-116">For more information, see [How to troubleshoot non-browser apps that can't sign in to Office 365, Azure, or Intune](https://support.office.com/article/how-to-troubleshoot-non-browser-apps-that-can-t-sign-in-to-office-365-azure-or-intune-3ba1b268-66f6-462c-b0e5-070f5c2603c1).</span></span>

