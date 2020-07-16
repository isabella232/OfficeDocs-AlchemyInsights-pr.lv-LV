---
title: Par identitāti pakalpojumā Yammer
ms.author: pebaum
author: pebaum
manager: scotv
ms.date: 07/15/2020
ms.audience: Admin
ms.topic: article
ROBOTS: NOINDEX, NOFOLLOW
localization_priority: Priority
ms.collection: Adm_O365
ms.custom:
- "6039"
- "9003111"
ms.openlocfilehash: 2c4c2c836d18d2ab45e2368e778c793277b18aa0
ms.sourcegitcommit: b677b85395b7244b2bf2b753468b696b4cf27c8d
ms.translationtype: MT
ms.contentlocale: lv-LV
ms.lasthandoff: 07/16/2020
ms.locfileid: "45148310"
---
# <a name="about-identity-in-yammer"></a><span data-ttu-id="f9ac2-102">Par identitāti pakalpojumā Yammer</span><span class="sxs-lookup"><span data-stu-id="f9ac2-102">About identity in Yammer</span></span>

<span data-ttu-id="f9ac2-103">Ieteicams visiem tīkliem veikt šādas darbības, lai izvairītos no problēmām, kas saistītas ar identitāti:</span><span class="sxs-lookup"><span data-stu-id="f9ac2-103">It is recommended that all networks take the following steps to avoid identity-related issues:</span></span>

1. <span data-ttu-id="f9ac2-104">Ieviest Office 365 identitāti pēc microsoft 365 kontu nodrošināšanas lietotājiem Azure AD, lai nodrošinātu, ka visi lietotāji pierakstās, izmantojot savu primāro Microsoft 365 kontu.</span><span class="sxs-lookup"><span data-stu-id="f9ac2-104">Enforce Office 365 identity after provisioning Microsoft 365 accounts for users in Azure AD to ensure that all users sign in by using their primary Microsoft 365 account.</span></span> <span data-ttu-id="f9ac2-105">Papildinformāciju skatiet rakstā [Office 365 identitātes ieviešana Yammer lietotājiem](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span><span class="sxs-lookup"><span data-stu-id="f9ac2-105">For more info, see [Enforce Office 365 identity for Yammer users](https://docs.microsoft.com/yammer/configure-your-yammer-network/enforce-office-365-identity).</span></span>
2. <span data-ttu-id="f9ac2-106">Konsolidēt vairākus Yammer tīklus.</span><span class="sxs-lookup"><span data-stu-id="f9ac2-106">Consolidate multiple Yammer networks.</span></span> <span data-ttu-id="f9ac2-107">Legacy Yammer konfigurācijas ļauj vairākiem Yammer tīkliem izveidot savienojumu ar vienu nomnieku.</span><span class="sxs-lookup"><span data-stu-id="f9ac2-107">Legacy Yammer configurations permit multiple Yammer networks to be connected to one tenant.</span></span> <span data-ttu-id="f9ac2-108">Papildinformāciju skatiet sadaļā Tīkla [migrācija — vairāku Yammer tīklu konsolidēšana](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span><span class="sxs-lookup"><span data-stu-id="f9ac2-108">For more info, see [Network migration - Consolidate multiple Yammer networks](https://docs.microsoft.com/yammer/configure-your-yammer-network/consolidate-multiple-yammer-networks).</span></span>
3. <span data-ttu-id="f9ac2-109">Pēc izvēles ieviest yammer licencēšanu, lai bloķētu lietotājus no Yammer, ja viņiem nav licences.</span><span class="sxs-lookup"><span data-stu-id="f9ac2-109">Optionally, enforce licensing for Yammer to block users from Yammer if they don't have a license.</span></span> <span data-ttu-id="f9ac2-110">Papildinformāciju skatiet rakstā [Yammer lietotāju licenču pārvaldība pakalpojumā Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span><span class="sxs-lookup"><span data-stu-id="f9ac2-110">For more info, see [Manage Yammer user licenses in Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/manage-yammer-licenses-in-office-365).</span></span>
4. <span data-ttu-id="f9ac2-111">Visbeidzot, auditējiet lietotāju sarakstu vecākiem Yammer tīkliem un aizturēt mantotos lietotājus.</span><span class="sxs-lookup"><span data-stu-id="f9ac2-111">Finally, audit the user list for older Yammer networks and suspend legacy users.</span></span> <span data-ttu-id="f9ac2-112">Ieteicams aizturēt (deaktivizēt) lietotājus, nevis dzēst tos, jo dzēšana ir neatgriezeniska.</span><span class="sxs-lookup"><span data-stu-id="f9ac2-112">It is recommended that you suspend (deactivate) users instead of deleting them, because deletion is irreversible.</span></span> <span data-ttu-id="f9ac2-113">Papildinformāciju skatiet rakstā Yammer [lietotāju audits tīklos, kas savienoti ar Office 365, un](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) [Lietotāju noņemšana](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span><span class="sxs-lookup"><span data-stu-id="f9ac2-113">For more info, see [Audit Yammer users in networks connected to Office 365](https://docs.microsoft.com/yammer/manage-yammer-users/audit-users-connected-to-office-365) and [Remove users](https://docs.microsoft.com/yammer/manage-yammer-users/add-block-or-remove-users#remove-users).</span></span>

<span data-ttu-id="f9ac2-114">Konfigurējot Yammer, veicot šīs darbības, varat arī konfigurēt Yammer tīklu microsoft 365 vietējais režīms.</span><span class="sxs-lookup"><span data-stu-id="f9ac2-114">By configuring Yammer using these steps, you'll also be ready to configure your Yammer network for Native Mode for Microsoft 365.</span></span> <span data-ttu-id="f9ac2-115">Papildinformāciju skatiet rakstā [Yammer tīkla konfigurēšana microsoft 365 vietējais režīms](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span><span class="sxs-lookup"><span data-stu-id="f9ac2-115">For more info, see [Configure your Yammer network for Native Mode for Microsoft 365](https://docs.microsoft.com/yammer/configure-your-yammer-network/native-mode).</span></span>