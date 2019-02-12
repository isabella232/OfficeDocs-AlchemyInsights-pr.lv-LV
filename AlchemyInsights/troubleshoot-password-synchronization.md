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
ms.custom: Adm_O365
ms.assetid: 1cba32c4-37ce-4ec1-9e58-8d3440b53d57
ms.openlocfilehash: d346cf97fb2fd08a9132904517192d8728ffa941
ms.sourcegitcommit: dd43cc0a9470f98b8ef2a3787c823801d674c666
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 02/12/2019
ms.locfileid: "29924703"
---
# <a name="troubleshoot-password-synchronization"></a><span data-ttu-id="6ff73-102">Problēmu novēršana darbā ar paroles sinhronizācija</span><span class="sxs-lookup"><span data-stu-id="6ff73-102">Troubleshoot password synchronization</span></span>

<span data-ttu-id="6ff73-103">Novērst problēmas, kur bez paroles tiek sinhronizēti ar Azure AD savienot versiju 1.1.614.0 vai jaunāka versija:</span><span class="sxs-lookup"><span data-stu-id="6ff73-103">To troubleshoot issues where no passwords are synchronized with Azure AD Connect version 1.1.614.0 or later:</span></span>
  
1. <span data-ttu-id="6ff73-104">Atvērt jaunu Windows PowerShell sesijā Azure AD savienojumu servera opciju **Palaist kā administratoram** .</span><span class="sxs-lookup"><span data-stu-id="6ff73-104">Open a new Windows PowerShell session on your Azure AD Connect server with the **Run as Administrator** option.</span></span> 
    
2. <span data-ttu-id="6ff73-105">Palaist **Set ExecutionPolicy RemoteSigned** vai **neierobežotu kopu ExecutionPolicy**.</span><span class="sxs-lookup"><span data-stu-id="6ff73-105">Run **Set-ExecutionPolicy RemoteSigned** or **Set-ExecutionPolicy Unrestricted**.</span></span> 
    
3. <span data-ttu-id="6ff73-106">Startēt vedni Azure AD savienojumu.</span><span class="sxs-lookup"><span data-stu-id="6ff73-106">Start the Azure AD Connect wizard.</span></span>
    
4. <span data-ttu-id="6ff73-107">Naviģējiet uz \* papilduzdevumus \* \* lapu, izvēlieties \* \* novēršana \* \*, un noklikšķiniet uz **Next (tālāk**).</span><span class="sxs-lookup"><span data-stu-id="6ff73-107">Navigate to the \*\* Additional Tasks \*\* page, select \*\* Troubleshoot \*\*, and click **Next**.</span></span> 
    
5. <span data-ttu-id="6ff73-108">Problēmu novēršana lapā noklikšķiniet uz **Sākt startēt problēmrisināšanas** menu PowerShell.</span><span class="sxs-lookup"><span data-stu-id="6ff73-108">On the Troubleshooting page, click **Launch to start the troubleshooting** menu in PowerShell.</span></span> 
    
6. <span data-ttu-id="6ff73-109">Galvenajā izvēlnē izvēlieties **Paroli sinhronizācijas problēmu novēršana**.</span><span class="sxs-lookup"><span data-stu-id="6ff73-109">In the main menu, select **Troubleshoot Password Synchronization**.</span></span> 
    
7. <span data-ttu-id="6ff73-110">Apakšizvēlnes, izvēlieties **Paroles sinhronizācija nedarbojas vispār**.</span><span class="sxs-lookup"><span data-stu-id="6ff73-110">In the sub menu, select **Password Synchronization does not work at all**.</span></span> 
    
 <span data-ttu-id="6ff73-111">**Izprast problēmu novēršanas uzdevumu rezultāti**</span><span class="sxs-lookup"><span data-stu-id="6ff73-111">**Understand the results of the troubleshooting task**</span></span>
  
<span data-ttu-id="6ff73-112">Problēmu novēršanas uzdevumu veic šādas pārbaudes:</span><span class="sxs-lookup"><span data-stu-id="6ff73-112">The troubleshooting task performs the following checks:</span></span>
  
- <span data-ttu-id="6ff73-113">Apstiprina, ka parole sinhronizācijas līdzeklis ir iespējots debeszils AD īrnieks.</span><span class="sxs-lookup"><span data-stu-id="6ff73-113">Validates that the password synchronization feature is enabled for your Azure AD tenant.</span></span>
    
- <span data-ttu-id="6ff73-114">Apstiprina, ka Azure AD savienojumu servera nav inscenējums režīmā.</span><span class="sxs-lookup"><span data-stu-id="6ff73-114">Validates that the Azure AD Connect server is not in staging mode.</span></span>
    
- <span data-ttu-id="6ff73-115">Par katru esošo lokālā Active Directory savienotāju (kas atbilst esošās Active Directory mežā):</span><span class="sxs-lookup"><span data-stu-id="6ff73-115">For each existing on-premises Active Directory connector (which corresponds to an existing Active Directory forest):</span></span>
    
- 
  - <span data-ttu-id="6ff73-116">Apstiprina, ka parole sinhronizācijas līdzeklis ir iespējots.</span><span class="sxs-lookup"><span data-stu-id="6ff73-116">Validates that the password synchronization feature is enabled.</span></span>
    
  - <span data-ttu-id="6ff73-117">Meklē paroles sinhronizācija sirdsdarbība notikumi Windows programmu notikumu žurnālos.</span><span class="sxs-lookup"><span data-stu-id="6ff73-117">Searches for password synchronization heartbeat events in the Windows Application Event logs.</span></span>
    
  - <span data-ttu-id="6ff73-118">Katra domēna Active Directory sadaļā lokālā Active Directory savienotāju:</span><span class="sxs-lookup"><span data-stu-id="6ff73-118">For each Active Directory domain under the on-premises Active Directory connector:</span></span>
    
  - <span data-ttu-id="6ff73-119">Apstiprina, ka domēns ir sasniedzams no Azure AD savienojumu servera.</span><span class="sxs-lookup"><span data-stu-id="6ff73-119">Validates that the domain is reachable from the Azure AD Connect server.</span></span>
    
  - <span data-ttu-id="6ff73-120">Apstiprina, ka Active Directory domēna pakalpojumus (AD DS) kontus izmanto lokālā Active Directory savienotājs ir pareizais lietotājvārds, parole un atļauju parole sinhronizācijai nepieciešamos.</span><span class="sxs-lookup"><span data-stu-id="6ff73-120">Validates that the Active Directory Domain Services (AD DS) accounts used by the on-premises Active Directory connector has the correct username, password, and permissions required for password synchronization.</span></span>
    
<span data-ttu-id="6ff73-121">Papildu palīdzību problēmu novēršana sinhronizācijas paroli, skatiet [novēršana paroles sinhronizācija ar Azure AD pievienot sinhronizācijas](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span><span class="sxs-lookup"><span data-stu-id="6ff73-121">For more help troubleshooting password sync, see [Troubleshoot password synchronization with Azure AD Connect sync](https://docs.microsoft.com/azure/active-directory/connect/active-directory-aadconnectsync-troubleshoot-password-synchronization).</span></span>
  

