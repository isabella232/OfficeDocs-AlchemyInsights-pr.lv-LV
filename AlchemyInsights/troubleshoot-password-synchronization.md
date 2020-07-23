---
title: Paroļu sinhronizācijas problēmu novēršana
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 04/21/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 54b5a033b7cbb99520425b31800364ed4a99a4e6
ms.sourcegitcommit: 1d01b8b48eef2d5d10c375dcf802cd36e9d6bf61
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/23/2020
ms.locfileid: "45387884"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="9136b-102">Paroļu sinhronizācijas problēmu novēršana</span><span class="sxs-lookup"><span data-stu-id="9136b-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="9136b-103">Lai novērstu paroļu sinhronizēšanas problēmas, sāciet ar šo AAD savienojumu problēmu novēršanas uzdevumu, lai noteiktu, kāpēc paroles netiek sinhronizētas.</span><span class="sxs-lookup"><span data-stu-id="9136b-103">To troubleshoot password synchronization issues, start by using this AAD Connect troubleshooting task to determine why passwords are not syncing.</span></span> <span data-ttu-id="9136b-104">Lai sāktu, dodieties uz [Pārvaldīt tiešo sinhronizāciju](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span><span class="sxs-lookup"><span data-stu-id="9136b-104">To begin, go to [Manage direct sync](https://admin.microsoft.com/AdminPortal/Home#/dirsyncmanagement).</span></span>  

1. <span data-ttu-id="9136b-105">Azure AD savienojumu serverī atveriet jaunu Windows PowerShell sesiju un atlasiet opciju **Palaist kā** administratoram.</span><span class="sxs-lookup"><span data-stu-id="9136b-105">Open a new Windows PowerShell session on your Azure AD Connect server, and select the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="9136b-106">Palaidiet Set-ExecutionPolicy RemoteSigned vai Set-ExecutionPolicy neierobežots.</span><span class="sxs-lookup"><span data-stu-id="9136b-106">Run Set-ExecutionPolicy RemoteSigned or Set-ExecutionPolicy Unrestricted.</span></span>

3. <span data-ttu-id="9136b-107">Azure AD savienojumu izveides vedņa startēšana.</span><span class="sxs-lookup"><span data-stu-id="9136b-107">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="9136b-108">Dodieties uz lapu Papildu uzdevumi > **Problēmu**  >  **novēršana Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="9136b-108">Go to the Additional Tasks page > **Troubleshoot** > **Next**.</span></span>

5. <span data-ttu-id="9136b-109">Atlasiet **Palaist,** lai atvērtu PowerShell problēmu novēršanas izvēlni.</span><span class="sxs-lookup"><span data-stu-id="9136b-109">Select **Launch** to open the PowerShell troubleshooting menu.</span></span>

6. <span data-ttu-id="9136b-110">Atlasiet **Problēmu novēršana par paroļu sinhronizāciju**.</span><span class="sxs-lookup"><span data-stu-id="9136b-110">Select **Troubleshoot Password Synchronization**.</span></span>

    <span data-ttu-id="9136b-111">Problēma parasti ir parole nav sinhronizēta konkrētu lietotāja kontu.</span><span class="sxs-lookup"><span data-stu-id="9136b-111">The issue is usually that a password is not synchronized for a specific user account.</span></span>

    <span data-ttu-id="9136b-112">**Piezīmes** Paroļu sinhronizēšana neizdodas, ja pēdējā veiksmīgā paroles sinhronizēšana bija pirms kāda laika.</span><span class="sxs-lookup"><span data-stu-id="9136b-112">**Notes** Password synchronization fails if the last successful password sync was some time ago.</span></span>

<span data-ttu-id="9136b-113">Lai saņemtu papildu palīdzību paroļu sinhronizēšanas problēmu novēršanu, [skatiet rakstu Paroļu jaucējprogramma sinhronizēšanas problēmu novēršana ar Azure AD Connect sinhronizāciju](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span><span class="sxs-lookup"><span data-stu-id="9136b-113">For more help troubleshooting password synchronization, see [Troubleshoot password hash synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/hybrid/tshoot-connect-password-hash-synchronization).</span></span>