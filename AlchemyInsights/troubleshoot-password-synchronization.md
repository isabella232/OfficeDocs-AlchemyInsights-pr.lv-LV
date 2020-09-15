---
title: Paroļu sinhronizēšanas problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 96f63f2ae8e5de246bce7fc15a9b2c3d604f2eb8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/14/2020
ms.locfileid: "47664933"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="3f966-102">Paroļu sinhronizēšanas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="3f966-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="3f966-103">Lai novērstu paroļu sinhronizēšanas problēmas, vispirms izmantojiet šo AAD Connect problēmu novēršanas uzdevumu, lai noskaidrotu, kāpēc paroles netiek sinhronizētas.</span><span class="sxs-lookup"><span data-stu-id="3f966-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="3f966-104">Lai sāktu, dodieties uz [Pārvaldīt tiešo sinhronizāciju](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="3f966-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="3f966-105">Azure AD Connect serverī atveriet jaunu Windows PowerShell sesiju un atlasiet opciju **Palaist kā administratoram** .</span><span class="sxs-lookup"><span data-stu-id="3f966-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="3f966-106">Palaidiet Set-ExecutionPolicy RemoteSigned vai Set-ExecutionPolicy neierobežoti.</span><span class="sxs-lookup"><span data-stu-id="3f966-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="3f966-107">Startējiet Azure AD Connect vedni.</span><span class="sxs-lookup"><span data-stu-id="3f966-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="3f966-108">Dodieties uz lapu papildu **uzdevumi >** tālāk norādītās darbības  >  **Next**.</span><span class="sxs-lookup"><span data-stu-id="3f966-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="3f966-109">Atlasiet **palaist** , lai atvērtu PowerShell problēmu novēršanas izvēlni.</span><span class="sxs-lookup"><span data-stu-id="3f966-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="3f966-110">Atlasiet **paroļu sinhronizēšanas problēmu novēršana**.</span><span class="sxs-lookup"><span data-stu-id="3f966-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="3f966-111">Šī problēma parasti ir tā, ka parole netiek sinhronizēta noteiktam lietotāja kontam.</span><span class="sxs-lookup"><span data-stu-id="3f966-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="3f966-112">**Piezīmju** veikšana Paroļu sinhronizēšana neizdodas, ja pēdējā veiksmīgā paroļu sinhronizācija bija pirms kāda laika.</span><span class="sxs-lookup"><span data-stu-id="3f966-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="3f966-113">Papildu palīdzību par paroļu sinhronizācijas problēmu novēršanu skatiet rakstā [paroļu jaukšanas sinhronizācijas problēmu novēršana, izmantojot AZURE ad Connect sinhronizāciju](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="3f966-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>