---
title: Problēmu novēršana paroļu sinhronizēšana
ms.author: pebaum
author: pebaum
manager: mnirkhe
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
ms.openlocfilehash: edd4f68466296f72c2dc0bafda45e6749d62d942
ms.sourcegitcommit: 631cbb5f03e5371f0995e976536d24e9d13746c3
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 04/22/2020
ms.locfileid: "43732517"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="38672-102">Problēmu novēršana paroļu sinhronizēšana</span><span class="sxs-lookup"><span data-stu-id="38672-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="38672-103">Lai novērstu problēmas, ja nav paroļu sinhronizētas ar Azure AD Connect versiju 1.1.614.0 vai jaunāka versija:</span><span class="sxs-lookup"><span data-stu-id="38672-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="38672-104">Atveriet jaunu Windows PowerShell sesiju savā Azure AD Connect serverī, izmantojot opciju **Palaist kā administratoram** .</span><span class="sxs-lookup"><span data-stu-id="38672-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span>

2. <span data-ttu-id="38672-105">Palaidiet **Set-Executionpolicy RemoteSigned** vai **Set-Executionpolicy neierobežoti**.</span><span class="sxs-lookup"><span data-stu-id="38672-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span>

3. <span data-ttu-id="38672-106">Startējiet vedni Azure AD Connect.</span><span class="sxs-lookup"><span data-stu-id="38672-106">Start the Azure AD Connect wizard.</span></span>

4. <span data-ttu-id="38672-107">Pārejiet uz **papildu uzdevumu** lapu, atlasiet **problēmu novēršana**un noklikšķiniet uz **Tālāk**.</span><span class="sxs-lookup"><span data-stu-id="38672-107">Navigate to the **Additional Tasks** page, select **Troubleshoot**, and click **Next**.</span></span>

5. <span data-ttu-id="38672-108">Problēmu novēršanas lapā, noklikšķiniet uz Sākt, **lai sāktu problēmu novēršanas** izvēlni PowerShell.</span><span class="sxs-lookup"><span data-stu-id="38672-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span>

6. <span data-ttu-id="38672-109">Galvenajā izvēlnē atlasiet **problēmu novēršana paroļu sinhronizēšana**.</span><span class="sxs-lookup"><span data-stu-id="38672-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span>

7. <span data-ttu-id="38672-110">Apakšizvēlnē atlasiet **paroļu sinhronizēšana**nedarbojas vispār.</span><span class="sxs-lookup"><span data-stu-id="38672-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span>

<span data-ttu-id="38672-111">**Izprastu problēmu novēršanas uzdevuma rezultātus**</span><span class="sxs-lookup"><span data-stu-id="38672-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="38672-112">Problēmu novēršanas uzdevums veic šādas pārbaudes:</span><span class="sxs-lookup"><span data-stu-id="38672-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="38672-113">Apstiprina, ka paroļu sinhronizēšana līdzeklis ir iespējots Azure AD nomnieka.</span><span class="sxs-lookup"><span data-stu-id="38672-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>

- <span data-ttu-id="38672-114">Apstiprina, ka Azure AD Connect serveris nav sagatavošanas režīmā.</span><span class="sxs-lookup"><span data-stu-id="38672-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>

- <span data-ttu-id="38672-115">Katram esošajam lokālā Active Directory savienotājs (kas atbilst esošo Active Directory mežā):</span><span class="sxs-lookup"><span data-stu-id="38672-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>

- 
  - <span data-ttu-id="38672-116">Pārbauda, vai paroļu sinhronizēšana līdzeklis ir iespējots.</span><span class="sxs-lookup"><span data-stu-id="38672-116">Validates that the password synchronization feature is enabled.</span></span>

  - <span data-ttu-id="38672-117">Meklē paroļu sinhronizēšana Periodisko kontrolziņojumu notikumus Windows lietojumprogrammu notikumu žurnālos.</span><span class="sxs-lookup"><span data-stu-id="38672-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>

  - <span data-ttu-id="38672-118">Par katru Active Directory domēna lokālā Active Directory savienotājs:</span><span class="sxs-lookup"><span data-stu-id="38672-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>

  - <span data-ttu-id="38672-119">Validē, ka domēns ir sasniedzams no Azure AD savienojumu servera.</span><span class="sxs-lookup"><span data-stu-id="38672-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>

  - <span data-ttu-id="38672-120">Apstiprina, ka Active Directory domēna pakalpojumus (AD DS) kontiem, ko izmanto lokālā Active Directory savienotājs ir pareizs lietotājvārds, parole, un atļaujām, kas nepieciešamas paroļu sinhronizēšana.</span><span class="sxs-lookup"><span data-stu-id="38672-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>

<span data-ttu-id="38672-121">Lai iegūtu palīdzību problēmu novēršana paroļu sinhronizēšana, skatiet [problēmu novēršana paroļu sinhronizēšana ar AZURE ad savienojumu sinhronizācija](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="38672-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  