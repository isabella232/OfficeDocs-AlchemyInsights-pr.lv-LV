---
title: 932 modernizāciju AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 6/8/2018
ms.audience: ITPro
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 07de6f8df7bfda2060977c7d5bc6a01766bf3c0a
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35365910"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="7f83b-102">Jaunināšanas debeszils AD savienojumu</span><span class="sxs-lookup"><span data-stu-id="7f83b-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="7f83b-103">Pēc noklusējuma ir iespējota automātiska jaunināšana Azure AD savienojumu, kas palīdz nodrošināt jūs lietojat jaunāko versiju.</span><span class="sxs-lookup"><span data-stu-id="7f83b-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="7f83b-104">Lai pārbaudītu automātiskās jaunināšanas iestatījumus, izmantojiet cmdlet **Get ADSyncAutoUpgrade** Azure AD PowerShell.</span><span class="sxs-lookup"><span data-stu-id="7f83b-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="7f83b-105">Cmdlet atgriež vienu no šīm vērtībām:</span><span class="sxs-lookup"><span data-stu-id="7f83b-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="7f83b-106">**Enabled**: automātisks jauninājums ir iespējota.</span><span class="sxs-lookup"><span data-stu-id="7f83b-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="7f83b-107">**Atspējots**: automātisks jauninājums ir atspējota.</span><span class="sxs-lookup"><span data-stu-id="7f83b-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="7f83b-108">**Apturēts**: sistēma vairs nav tiesības saņemt automātisku jaunināšanu.</span><span class="sxs-lookup"><span data-stu-id="7f83b-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="7f83b-109">Nevar konfigurēt šo vērtību; to iestata sistēma.</span><span class="sxs-lookup"><span data-stu-id="7f83b-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="7f83b-110">Papildinformāciju skatiet sadaļā [Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="7f83b-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="7f83b-111">Lai lejupielādētu jaunāko versiju Azure AD savienojumu, dodieties uz [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span><span class="sxs-lookup"><span data-stu-id="7f83b-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
