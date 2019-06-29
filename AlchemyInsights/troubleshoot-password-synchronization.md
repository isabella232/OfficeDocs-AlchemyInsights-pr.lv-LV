---
title: Problēmu novēršana darbā ar paroles sinhronizācija
ms.author: pebaum
author: pebaum
manager: mnirkhe
ms.date: 3/20/2018
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Normal
ms.collection: Adm_O365
ms.custom:
- "579"
- "1300006"
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: 165e0ff4b2136b727450946d2c47756ebee7d393
ms.sourcegitcommit: 5fb7a4b28859690020efdea630d03e70cc0e6334
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 06/28/2019
ms.locfileid: "35353112"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="cbb9f-102">Problēmu novēršana darbā ar paroles sinhronizācija</span><span class="sxs-lookup"><span data-stu-id="cbb9f-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="cbb9f-103">Novērst problēmas, kur bez paroles tiek sinhronizēti ar Azure AD savienot versiju 1.1.614.0 vai jaunāka versija:</span><span class="sxs-lookup"><span data-stu-id="cbb9f-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="cbb9f-104">Atvērt jaunu Windows PowerShell sesijā Azure AD savienojumu servera opciju **Palaist kā administratoram** .</span><span class="sxs-lookup"><span data-stu-id="cbb9f-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="cbb9f-105">Palaist **Set ExecutionPolicy RemoteSigned** vai **neierobežotu kopu ExecutionPolicy**.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="cbb9f-106">Startēt vedni Azure AD savienojumu.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="cbb9f-107">Naviģējiet uz lapu **Papildu uzdevumus** , atlasiet **problēmu novēršana**un noklikšķiniet uz **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="cbb9f-108">Problēmu novēršana lapā noklikšķiniet uz **Sākt startēt problēmrisināšanas** menu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="cbb9f-109">Galvenajā izvēlnē izvēlieties **Paroli sinhronizācijas problēmu novēršana**.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="cbb9f-110">Apakšizvēlnes, izvēlieties **Paroles sinhronizācija nedarbojas vispār**.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="cbb9f-111">**Izprast problēmu novēršanas uzdevumu rezultāti**</span><span class="sxs-lookup"><span data-stu-id="cbb9f-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="cbb9f-112">Problēmu novēršanas uzdevumu veic šādas pārbaudes:</span><span class="sxs-lookup"><span data-stu-id="cbb9f-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="cbb9f-113">Apstiprina, ka parole sinhronizācijas līdzeklis ir iespējots debeszils AD īrnieks.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="cbb9f-114">Apstiprina, ka Azure AD savienojumu servera nav inscenējums režīmā.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="cbb9f-115">Par katru esošo lokālā Active Directory savienotāju (kas atbilst esošās Active Directory mežā):</span><span class="sxs-lookup"><span data-stu-id="cbb9f-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="cbb9f-116">Apstiprina, ka parole sinhronizācijas līdzeklis ir iespējots.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="cbb9f-117">Meklē paroles sinhronizācija sirdsdarbība notikumi Windows programmu notikumu žurnālos.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="cbb9f-118">Katra domēna Active Directory sadaļā lokālā Active Directory savienotāju:</span><span class="sxs-lookup"><span data-stu-id="cbb9f-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="cbb9f-119">Apstiprina, ka domēns ir sasniedzams no Azure AD savienojumu servera.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="cbb9f-120">Apstiprina, ka Active Directory domēna pakalpojumus (AD DS) kontus izmanto lokālā Active Directory savienotājs ir pareizais lietotājvārds, parole un atļauju parole sinhronizācijai nepieciešamos.</span><span class="sxs-lookup"><span data-stu-id="cbb9f-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="cbb9f-121">Papildu palīdzību problēmu novēršana sinhronizācijas paroli, skatiet [novēršana paroles sinhronizācija ar Azure AD pievienot sinhronizācijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="cbb9f-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  