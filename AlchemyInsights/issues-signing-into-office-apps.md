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
- "2559"
ms.openlocfilehash: c64cf2c9dbf63caad22e54ae801adc3ed8ff0f62
ms.sourcegitcommit: 8bc60ec34bc1e40685e3976576e04a2623f63a7c
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/15/2021
ms.locfileid: "51833010"
---
# <a name="fixing-the-microsoft-365-apps-your-computers-trusted-platform-module-is-not-functioning-properly-message"></a><span data-ttu-id="d5291-102">Microsoft 365 programmu labošana: ziņojums "Jūsu datora uzticamās platformas modulis nedarbojas pareizi"</span><span class="sxs-lookup"><span data-stu-id="d5291-102">Fixing the Microsoft 365 apps "Your computer's Trusted Platform module is not functioning properly" message</span></span>

<span data-ttu-id="d5291-103">Lai novērstu šo kļūdu, izmēģiniet tālāk norādīto:</span><span class="sxs-lookup"><span data-stu-id="d5291-103">To fix this error, try the following:</span></span>

- <span data-ttu-id="d5291-104">Instalējiet jaunākos [Windows un](https://support.microsoft.com/help/4027667/windows-10-update) [Office atjauninājumus.](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5)</span><span class="sxs-lookup"><span data-stu-id="d5291-104">Install the latest updates for [Windows](https://support.microsoft.com/help/4027667/windows-10-update) and [Office](https://support.office.com/article/update-office-and-your-computer-with-microsoft-update-2ab296f3-7f03-43a2-8e50-46de917611c5).</span></span>
- <span data-ttu-id="d5291-105">[Notīriet Office akreditācijas](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) datus, izmantojot Windows akreditācijas datu pārvaldnieku.</span><span class="sxs-lookup"><span data-stu-id="d5291-105">[Clear Office credentials](https://docs.microsoft.com/office/troubleshoot/office-suite-issues/another-account-already-signed-in#step-4-clear-cached-credentials-on-the-computer) using Windows Credential Manager.</span></span><br/>
    <span data-ttu-id="d5291-106">**Piezīme.** Office 2016 reģistra ceļi ir mainīti uz 16.0.</span><span class="sxs-lookup"><span data-stu-id="d5291-106">**Note:** The registry paths for Office 2016 have changed to 16.0.</span></span> <span data-ttu-id="d5291-107">(Piemēram, \Software\Microsoft\Office\16.0\Common\Identity\)</span><span class="sxs-lookup"><span data-stu-id="d5291-107">(Ex: \Software\Microsoft\Office\16.0\Common\Identity\)</span></span>
- <span data-ttu-id="d5291-108">Mēģiniet lietotāja [atkopšanas procesu,](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) lai izlabotu uzticamā platformas moduļa (TPM) kļūmes.</span><span class="sxs-lookup"><span data-stu-id="d5291-108">Try the [user recovery process](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016#symptom-2) to fix Trusted Platform Module (TPM) failures.</span></span>
- <span data-ttu-id="d5291-109">Iestatiet EnableADAL = 0, veicot tālāk norādītās darbības.</span><span class="sxs-lookup"><span data-stu-id="d5291-109">Set the EnableADAL = 0 using the following steps:</span></span>  
    1. <span data-ttu-id="d5291-110">Ar peles labo pogu noklikšķiniet uz Windows sākuma pogas, **izvēlieties Palaist,** ierakstiet **regedit** un pēc tam izvēlieties **Labi**.</span><span class="sxs-lookup"><span data-stu-id="d5291-110">Right-click the Windows Start button, choose **Run**, type **regedit**, and then choose **OK**.</span></span>
    2. <span data-ttu-id="d5291-111">Atlasiet **Jā,** lai atļautu reģistra redaktoram veikt izmaiņas jūsu ierīcē.</span><span class="sxs-lookup"><span data-stu-id="d5291-111">Select **Yes** to allow Registry Editor to make changes to your device.</span></span>
    3. <span data-ttu-id="d5291-112">Reģistra redaktorā pievienojiet **EnableADAL** DWORD vērtību ar iestatījumu **0** sadaļā HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span><span class="sxs-lookup"><span data-stu-id="d5291-112">In Registry Editor, add a DWORD value of **EnableADAL** with a setting of **0** under HKEY_CURRENT_USER\Software\Microsoft\Office\16.0\Common\Identity.</span></span>

<span data-ttu-id="d5291-113">Papildinformāciju skatiet rakstā Savienojuma problēmas pierakstoties pēc atjaunināšanas uz [Office 2016 būvējumu 16.0.7967 operētājsistēmā Windows 10.](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016)</span><span class="sxs-lookup"><span data-stu-id="d5291-113">For more information, see [Connection issues in sign-in after update to Office 2016 build 16.0.7967 on Windows 10](https://docs.microsoft.com/office365/troubleshoot/administration/connection-issue-when-sign-in-office-2016).</span></span>