---
title: 932 jaunināšanas AADConnect
ms.author: chrisda
author: chrisda
manager: dansimp
ms.date: 04/21/2020
ms.audience: ITPro
ms.topic: article
ms.service: o365-administration
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.custom:
- "932"
- "1300025"
ms.assetid: 8f43f36c-9722-43a4-b0de-c5341c06dac5
ms.openlocfilehash: 5c8ec5d9282c53c655e28f5d38fe36fc3ab005b8
ms.sourcegitcommit: c6692ce0fa1358ec3529e59ca0ecdfdea4cdc759
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 09/15/2020
ms.locfileid: "47806046"
---
# <a name="upgrade-azure-ad-connect"></a><span data-ttu-id="9e3e7-102">Azure AD Connect jaunināšana</span><span class="sxs-lookup"><span data-stu-id="9e3e7-102">Upgrade Azure AD Connect</span></span>

<span data-ttu-id="9e3e7-103">Pēc noklusējuma Azure AD Connect ir iespējota automātiskā jaunināšana, kas palīdz nodrošināt, ka izmantojat jaunāko versiju.</span><span class="sxs-lookup"><span data-stu-id="9e3e7-103">By default, automatic upgrade is enabled for Azure AD Connect, which helps to ensure you're running the latest version.</span></span> <span data-ttu-id="9e3e7-104">Lai pārbaudītu automātiskos jaunināšanas iestatījumus, izmantojiet Azure AD PowerShell **Get-ADSyncAutoUpgrade** cmdlet.</span><span class="sxs-lookup"><span data-stu-id="9e3e7-104">To verify the automatic upgrade settings, use the **Get-ADSyncAutoUpgrade** cmdlet in Azure AD PowerShell.</span></span> <span data-ttu-id="9e3e7-105">Cmdlet atgriezīs vienu no tālāk norādītajām vērtībām.</span><span class="sxs-lookup"><span data-stu-id="9e3e7-105">The cmdlet will return one of following values:</span></span>

- <span data-ttu-id="9e3e7-106">**Iespējots**: iespējota automātiskā jaunināšana.</span><span class="sxs-lookup"><span data-stu-id="9e3e7-106">**Enabled**: Automatic upgrade is enabled.</span></span>

- <span data-ttu-id="9e3e7-107">**Atspējots**: Automātiskā jaunināšana ir atspējota.</span><span class="sxs-lookup"><span data-stu-id="9e3e7-107">**Disabled**: Automatic upgrade is disabled.</span></span>

- <span data-ttu-id="9e3e7-108">**Apturēts**: sistēmai vairs nav tiesības saņemt automātiskus jauninājumus.</span><span class="sxs-lookup"><span data-stu-id="9e3e7-108">**Suspended**: The system is no longer eligible to receive automatic upgrades.</span></span> <span data-ttu-id="9e3e7-109">Šo vērtību nevar konfigurēt. to iestata sistēma.</span><span class="sxs-lookup"><span data-stu-id="9e3e7-109">You can't configure this value; it's set by the system.</span></span>

<span data-ttu-id="9e3e7-110">Papildinformāciju skatiet rakstā [Automātiskā jaunināšana](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span><span class="sxs-lookup"><span data-stu-id="9e3e7-110">For more information, see [Automatic upgrade](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnect-feature-automatic-upgrade).</span></span>

<span data-ttu-id="9e3e7-111">Lai lejupielādētu jaunāko Azure AD Connect versiju, dodieties uz [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594) .</span><span class="sxs-lookup"><span data-stu-id="9e3e7-111">To download the latest version of Azure AD Connect, go to [https://www.microsoft.com/download/details.aspx?id=47594](https://www.microsoft.com/download/details.aspx?id=47594).</span></span>
