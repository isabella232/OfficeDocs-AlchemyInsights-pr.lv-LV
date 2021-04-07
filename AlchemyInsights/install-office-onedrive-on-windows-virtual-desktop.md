---
title: Office un OneDrive instalēšana Windows virtuālajā darbvirsmā
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/5/2021
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "9004219"
- "10871"
ms.openlocfilehash: fb38f46cced928e33e16e8e83ad740dd83aea622
ms.sourcegitcommit: 254b25150fa326628084d08479b0e7dd8b7d479a
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/05/2021
ms.locfileid: "51595847"
---
# <a name="install-office-and-onedrive-on-windows-virtual-desktop"></a><span data-ttu-id="92fee-102">Office un OneDrive instalēšana Windows virtuālajā darbvirsmā</span><span class="sxs-lookup"><span data-stu-id="92fee-102">Install Office and OneDrive on Windows Virtual Desktop</span></span>

1. <span data-ttu-id="92fee-103">[Sagatavojiet un pielāgojiet galveno VHD attēlu.](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image)</span><span class="sxs-lookup"><span data-stu-id="92fee-103">[Prepare and customize a master VHD image](https://docs.microsoft.com/azure/virtual-desktop/set-up-customize-master-image).</span></span> <span data-ttu-id="92fee-104">Izveidojiet virtuālo mašīnu (VM), ja tā vēl nav izveidota.</span><span class="sxs-lookup"><span data-stu-id="92fee-104">Create a virtual machine (VM) if it hasn't already been created.</span></span>

1. <span data-ttu-id="92fee-105">[Instalējiet Office koplietojamā datora aktivizācijas režīmā.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode)</span><span class="sxs-lookup"><span data-stu-id="92fee-105">[Install Office in shared computer activation mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-office-in-shared-computer-activation-mode).</span></span> <span data-ttu-id="92fee-106">Koplietojama datora aktivizēšana ļauj vairākiem lietotājiem piekļūt Office.</span><span class="sxs-lookup"><span data-stu-id="92fee-106">Shared computer activation allows multiple users to access Office.</span></span>

1. <span data-ttu-id="92fee-107">[Instalējiet OneDrive katrā datora režīmā.](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode)</span><span class="sxs-lookup"><span data-stu-id="92fee-107">[Install OneDrive in per-machine mode](https://docs.microsoft.com/azure/virtual-desktop/install-office-on-wvd-master-image#install-onedrive-in-per-machine-mode).</span></span> <span data-ttu-id="92fee-108">Parasti katram lietotājam tiek instalēts OneDrive, bet šeit tā ir jāinstalē katrā datorā.</span><span class="sxs-lookup"><span data-stu-id="92fee-108">Normally, OneDrive is installed per user, but here, it should be installed per machine.</span></span>